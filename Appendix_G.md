[Home](/index.md)

## MPLAB MCC Configuration

## System Module

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/3ce426fe-a275-4e9e-831a-47ddd471d6f8)


## MSSP1

![Screenshot 2024-04-29 203336](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/b5ee66cc-98e0-4dfe-a5cd-fb54ea7c7bcb)


## MSSP2

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/b96310f1-3d84-4be2-b79e-6f73de121501)


## EUSART1

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/d5c0165a-7db5-4bec-b5f9-e70c1b83aada)


## TMR2

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/696d9ea4-a799-4f3d-889a-36d2da2cc8fc)


## Pin Module Grid View

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/603fd168-7161-4a8f-8ba9-2e3fbd0a88b0)


## Pin Module & Microcontroller Pinout View

![image](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/59342383-a389-4522-b9b3-0e313361b209)



## MQTT Topic Table
![Screenshot 2024-04-29 202700](https://github.com/Team-309-Hydro-Pro/EGR314-Spring2024-Team309.github.io/assets/157083379/bacc0f36-e72c-4a56-a981-8d4f0df064f6)

## main.c Code

#include "mcc_generated_files/mcc.h"
#include "mcc_generated_files/eusart2.h"
#include "mcc_generated_files/i2c1_master.h"
#include "mcc_generated_files/examples/i2c1_master_example.h"
#include "mcc_generated_files/spi2.h"
#define I2C_ADDR_TC74 0x4C
#define I2C_ADDR_SHT 0x44
#define HUM_ZERO 0xE0
#define TEMP_ZERO 0x00
#include <string.h>

uint8_t FORWARD = 0b11101111;
uint8_t STOP = 0b11101100;
uint8_t data;
uint8_t ReadTemperature = 0x0;
uint8_t ReadHumidity = 0x0;
uint8_t timer_ms = 0;
uint8_t time_s = 0;
float time = 0;
int led_toggle_flag = 0;


void timer_callback(void)
{
    timer_ms = timer_ms + 1;
    if(timer_ms>1000)
    {
        timer_ms = timer_ms - 1000;
        time_s = time_s + 1;
    }
    if (time_s % 10 == 0)
    {
        led_toggle_flag = 1; 
    }
}


void main(void)
{

        SYSTEM_Initialize();
    

        EUSART1_Initialize();
        EUSART2_Initialize();
        TMR2_Initialize();
        I2C1_Initialize();
        SPI2_Initialize();

        SPI2_Open(SPI2_DEFAULT);
        
        INTERRUPT_GlobalInterruptEnable();

        INTERRUPT_PeripheralInterruptEnable();
    
        TMR2_SetInterruptHandler(timer_callback);
        TMR2_Start();
    
    int i = 0 ; 

    float read_hum; 

    int ii = 0 ; 

    float read_temp;
    
    int iii = 0 ; 

    float read_time;
    
    while(1)
    {

       ReadTemperature = I2C1_Read1ByteRegister(I2C_ADDR_TC74,TEMP_ZERO );       
       printf("!Temperature = %u \r\n", ReadTemperature);
          if ( ReadTemperature >= 27 ){
        
        IO_RB4_SetLow();

        data = SPI2_ExchangeByte(FORWARD);

        IO_RB4_SetHigh();
        __delay_ms(2000);
        
        }        
        
           else{

        
        IO_RB4_SetLow();

        data = SPI2_ExchangeByte(STOP);  

        IO_RB4_SetHigh();

        __delay_ms(500);
          
         }
        
       
            

        ReadHumidity = I2C1_Read2ByteRegister( I2C_ADDR_SHT, HUM_ZERO );
         float Humidity_Value = 100 * (float) ReadHumidity/255;
         printf("-Humidity = %f \r\n", Humidity_Value);
       
           
           if ( Humidity_Value <= 30 ){
        IO_RA0_SetHigh();
        IO_RB4_SetLow();
        
        data = SPI2_ExchangeByte(FORWARD);
   
        IO_RB4_SetHigh();
        __delay_ms(2000);
       
         
           }else{
 
        IO_RA0_SetLow();
        IO_RB4_SetHigh();

        data = SPI2_ExchangeByte(STOP);  

        IO_RB4_SetHigh();

        __delay_ms(500);
        timer_callback();
        float time= time_s +timer_ms / 1000.0f;
        printf("+t= %2.3f \r\n", time);

       if(i<100)
       {
           i++;
           read_hum=i/10;
          
       }    
       else 
       {
           i=0;
       }
       if (ii < 100)
       {
          ii++;
          read_temp= ii/10;
          
       }
       else
       {
           ii =0;
       }
        if(iii <100)
       {
           iii++;
           read_time=iii/10;
          
       }    
       else 
       {
           iii=0;
       }
        if (led_toggle_flag)
        {
            IO_RA1_Toggle(); 
            led_toggle_flag = 0; 
        }
      }
      }
      }

<br>

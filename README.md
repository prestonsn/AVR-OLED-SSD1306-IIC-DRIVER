# AVR-OLED-SSD1306-IIC-DRIVER

This library contains code to drive the SSD1306 OLED displays using AVR ATmega series of microcontrollers. 
The default font size is set to 5.

Using the library is really simple, here is initialization code for the OLED:

```C
int main(void) {
	  
    OLED_Init();  //initialize the OLED
    OLED_Clear(); //clear the display (for good measure)
    
    while (1) {
        
        OLED_SetCursor(0, 0);        //set the cursor position to (0, 0)
        OLED_Printf("Hello World!"); //Print out some text

    }
    
	return 0; // never reached
}
```

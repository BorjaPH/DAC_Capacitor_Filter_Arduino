# DAC_Condenser_Filter_Arduino

A DAC using a PWM signal through OC2A's pin and a condenser filter. To choose the condenser filter needed on my board, I used the following equation:

                                              C > nperiods * T/5*R = T/500 Faradios
                                              
Being "nperiods" the periods needed to chrage the condenser, "T" the period of the PWM signal and "R" the resistance's value

the analog value obtained in voltage in relation to the duty cycle of PWM signal comes by the following equation:

                                                        V media≈ Ton/T*V
                                                        
Being "V" the maximum voltage (5000 mV) of PWM signal and T it's period.

It has a command "output [milivolts]" (through serial monitor) to modify the output signal.

The hardware montage is the same as described in the schematic below:

![Esquemático_2](https://user-images.githubusercontent.com/68208538/135024749-e73995a0-2d64-4052-92b3-c0034c61d2ff.PNG)

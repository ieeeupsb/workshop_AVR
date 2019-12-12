Exercise 4: Using a servo motor

Connect the Vcc and GND to the breadboard. Connect the Pin PB1 to the PWM of the motor. The motor's Vcc and GND connect to the breadboard.


TCCR1A |= (1 << WGM11);
TCCR1B |= (1 << WGM12)|(1 << WGM13) | (1<<CS11);
// set Fast PWM mode using ICR1 as TOP to free OCR1A to be used to generate the PWM 
// START the timer with no prescaler


Use the following commands to define the PWM output:
DDRB |= (1 << DDB1); //PB1 is now an output


To define the duty-cycle you'l need to use:
OCR1B and OCR1A

Determine the values to which the engine is moving forward at full speed, backward at full speed and completely stopped.

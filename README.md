# lab2b-feedback

Outline:
- 01_registers I use gpio to get the boot pin first, and it is hard to understand what is the register for the LED light.
- 02_repl This part is good.
- 03_sequencer Me and my teammates use array in c firstly to fetch the sequencer part, and we finally use python serial to do the sequencer. The instrcution is not clear for the sequencer part.
- 04_slow_motion I did not understand if we are slowing down the speed by slowing down the clock speed or register speed, or it is just a larger delay time for each steps sequencer. 
- 05_i2c_traffic
this part is good.
- 06_pioscope
I don't know if we are suppoed to use a python serial to get a nice picture of the clk and data diagram. 
- 07_pio_sequencer
i don't know if we should use the pio as the input and output for the sequencer.
- 08_adps_protocol
- 09_lab_on_a_chip
- 10_protoboard
- EC_analog_knob
- EC_ansi_escapes
- EC_asm_registers
- EC_dma_i2c
- EC_hardware_i2c
- EC_interrupt_i2c
- EC_lovr_viz
- EC_pwm_scope
- EC_socket_server
- EC_speaker
Which parts of the lab specification have you found most confusing or difficult to understand? Be specific, and quote any parts of the lab description relevant to your answer (e.g., "modify the PIO/DMA logic analyzer example to record a timestamped trace of an RP2040-ADPS9960 exchange while the BOOT button is pressed.") I will make particular notice of anything that seems underspecified (e.g., words whose meaning is not clear from context, or conflicting interpretations of a deliverable).

part 9 is the most confusing part, since the description is not very clear about what we should do and what kind of code should we use?
Run this experiment in both dark and light room settings (record initial ambient brightness in each case). The Neopixel should start 'off' and the ADPS9960 should be initialized with your preferred sampling rate (you may want to try a few different rates). Run the experiment for at least 100 samples at brightness settings of 0%, 25%, 50%, 75%, 100% (making sure to give the ADPS reading enough time to 'settle' each time Neopixel is turned off).

Which lab topics have you found most confusing or difficult to understand? E.g., "serial communication with Python," "aliased bitwise operations," "programming the PIO," etc. Be specific, and describe any lingering areas of confusion and/or anything that has helped you navigate them.

The ADPS portocal 
Run this experiment in both dark and light room settings (record initial ambient brightness in each case). The Neopixel should start 'off' and the ADPS9960 should be initialized with your preferred sampling rate (you may want to try a few different rates). Run the experiment for at least 100 samples at brightness settings of 0%, 25%, 50%, 75%, 100% (making sure to give the ADPS reading enough time to 'settle' each time Neopixel is turned off). 
What do we need to do for 100 samples at different brightness setting?, and since every time the ADPS9960 is initialized, why should we start the neopixel off at first. 


Which parts of the lab have you found most difficult to implement? Again, be specific, citing any parts of the lab materials & your own code that are relevant to your answer.
part 8 is most diffcult to implement, since I don't know how to use I2C to communicate with sensor, and I don't understand read and write function of I2C and how to find the register for proximity and r g b for the sensor. 

What steps have you taken to resolve these difficulties? Any other barriers you have faced to completing this assignment? Mention any students, repos, or other resources you have found helpful in completing the lab so far.

My teammate and I works really hard to figure it out, we use the APDS9600 data sheet, the code from other students inspires us a lot and somehow lead to the right path to some of the problems. 

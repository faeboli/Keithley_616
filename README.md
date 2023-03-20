# Keithley_616
Modification to Keithley 616 input buffer:
My keithkey 616 had the input mosfet Q101 broken,
I lately was not happy with it's performance, current leakage was 0.3pA, zero was drifty.
So my idea was to replace the input circuitry with a modern opamp, reading around the
perfect candidate was the LMC6081, a low leakage mosfet opamp.
In order to replace the input buffer, the zero circuit need to be reimplemented.
I have posted some pics in this eevblog thread:

https://www.eevblog.com/forum/repair/keithley-616-electrometer-input-stage-replacement/

The schematic is very simple, this part (PC361 in the box below):

![616_Buf](https://user-images.githubusercontent.com/50676392/225948453-17ec0acf-9ab4-45ff-bf26-65b1070dc738.PNG)

will be replaced by this, C5 R6 need to be tuned manually:

![image](https://user-images.githubusercontent.com/50676392/226322915-b127753d-e61b-4509-9898-5abb66d03c72.png)

I have also created a PCB project:

![image](https://user-images.githubusercontent.com/50676392/226322805-dd7ab08d-3f4e-4727-a882-326e89a26b4c.png)

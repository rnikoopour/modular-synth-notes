# Sample and Hold
This works by using the gate being passed through Channel 2 to
slow the rate of change happening in Channel 1's input. The slowed
rate of change on Channel 1 while the gate is open creates sample
effect. 

It is worth noting that this isn't a real sample and hold as 
Channel 1 is continuously chaning.

In this example only Channel 1 and Channel 2 are used.

## Channel 1 Settings
### Input Channel
This is used as the input signal for the sample and hold. Using an
LFO is recommended.

This input signal could also be replaced by a clock into the 
trigger input.

### Rise, Fall, and Shape
By setting the rise and fall knobs to higher values it slows down
the change on the input signal. 

The shape knob can be used to adjust how quickly it responds to 
changes in voltages.

### Both Input
Passing the inverted gate from Channel 2 into this input makes it
so when the signal gate is open, it slows down the rate of change
in Channel 1. This change while the gate is open is what is used
to "sample" the signal. 

In reality the sample is continuously changing but the rate of 
change is slowed to the point where it doesn't sound like there is
change.

## Channel 2 Settings
Channel 2 takes the gate input and inverts it. The inverted signal
is then used as input into the Both input on Channel 1. When the
gate is high, Channel 2 inverts it to negative. That negative gate
is then used to slow the rate of change on Channel 1. 

# Notes
This effect can be achieved through various other setups as well.

# References
- https://www.makenoisemusic.com/content/manuals/MATHSmanual2013.pdf
- https://www.youtube.com/watch?v=pk22s4UPrzc
- https://www.youtube.com/watch?v=ZNxdEwSrnfI

# DRONE PATCH 1

## Modules

This patch uses the following modules:

* Marbles [Mutable Instruments]
* Cs-L [Instruo]
* Maths [Make Noise]
* VCF1 [Erika Synths]
* A Mix [Erika Synths]
* DSP [Erika Synths]
* Output [Erika Synths]

## Patch Paths

Patch paths are described in the following manner:

`[Output Module]:[Output Jack] -> [Input Module]:[Input Jack]`

* Marbles:X2 -> Cs-L:Top 1V/Oct
* Maths:OR -> Cs-L:Top Wavefolder CV
* Cs-L:Top Final -> VCF1:IN
* Cs-L:Bottom PWM -> VCF1:CV IN
* VCF1:OUT -> A MIX:IN 1
* A MIX:OUT -> DSP:IN
* DSP:OUT R -> Output:IN R
* DSP:OUT L -> Output:IN L

## Recommended Module Settings

Not all module settings will be documented.  Just the ones I feel are important
to replicate this patch.

### DSP

The DSP should be set to the `Mono Delay` effect.

### Maths

Set the attenuators for channels 1, 2, and 3 to send negative voltages that will
not interfere with the OR channel.

Set channel 4 to cycle when you want to have a stead strike of the CS-L's 
top wavefolder. Use channel 4's attenuator to influence how much it interacts 
with the top wavefolder.

The use of the OR channel instead of channel 4's direct output is to allow for
other envelopes to be patched into any of the other channels should further
exploration be desired.

### Marbles

The rate should be set to the slowest value possible.

The spead should be set to a low value to concentrate the values the Marbles
generates to a small range.

The bias should be set to a low value to have the values the Marbles generates
kept in the low voltages.

The X button should not be turned on. This allows the Marbles to freely generate
new voltage everytime.

### Cs-L
The top Cs-L oscillator set to a low frequency for droning.

## Exploring the Patch
Try a variety of adjustments to the Cs-L to generate interesting sounds.

For example, setting the top wave folder to a low value will stop generating a
continunous drone since it's connected to an exponential VCA. Now start cycling
channel 4 of the Maths. Adjusting the envelope sent by the Math's can generate
interestings sounds.

Playing around with the VCF1's cut off frequency and resonance can help the 
drone generate some high frequency sounds. Using the Cs-L's bottom oscillator's
PWM output as an LFO into the VCF1's cut off frequency can help generate quick
in a rhythmic fashion.

Using the Cs-L's bottom oscillator as a FM source for the Cs-L's top oscillator
helps introduce ever more sounds. Try patching in the square wave from the 
bottom oscillator and setting it to a sub frequency.

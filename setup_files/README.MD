You will need to install these:
1) A numpy and tflite runtime wheels compatible with Python 3.8, presented in the PYNQZ2 image
2) TFLite model of MCU-net

Reasons:
Arch of the PS on PYNQ Z2 is ARM7l and Pytorch is not very well supported on these.
Shifted to TFLite due to its emphasis on models for resource constrained devices
Tried MobileNetv1 w/o optimization, couldn't run, not enough memory
Found MCU-net online => tried that => Would work with an average fps of 2-3fps.




# Bad_USB
A PCB for a bad USB based on Malduino W, but with a built in hub to allow for use as a real USB stick.

A 'Bad USB' is a fake USB stick capable of injecting keystokes into any machine by pretending to be a keyboard, wile typically resembling a storage drive from the outside. This specific design attempts to remove the giveaway that the supposed USB stick does not have any storage, or even a drive. This is fixed by adding a USB hub internally that connects both the Cortex M0 (acting as keyboard) and the real USB stick to the computer, and because windows (and presumeably Mac and most Linux kernels) do not display if the USB stick is connected through a hub except in device manager. The other advantage this design offers is its webserver. The firmware is made by maltronics.com, and offers a rich interface for scripting keystrokes after the device is inserted, as opposed to most bad USBs which only have one payload that is executed as soon as it is plugged in.

NOT FOR MALICIOUS USE! This is merely a tool to prank freinds, changing their desktop backrounds, or 'rick-rolling' them. (see https://en.wikipedia.org/wiki/Rickrolling)

The main components are an ESP8266, an ARM Comtex M0, a USB hub controller, and a readily available USB stick. The USB stick is not in the scematic because it will be soldered on to pads with wires in order to save space by stacking.

![PCB](https://user-images.githubusercontent.com/36117326/165008082-c7a45a37-7bfb-40b8-bb8d-5e70b1ca5f0a.png)

![usb_stick_case_1](https://user-images.githubusercontent.com/36117326/165008087-29787c1e-c635-467c-8c41-ae01c85e7de1.png)

![usb_stick_case_2](https://user-images.githubusercontent.com/36117326/165008093-57d380f9-b050-4463-8ff8-c47f1dea6130.png)

![usb_stick_case_3](https://user-images.githubusercontent.com/36117326/165008105-2003a76a-133e-40d0-b2ee-49ea8f2d0de3.png)

[Bad USB schem.pdf](https://github.com/paulwrath1223/Bad_USB/files/8551061/Bad.USB.schem.pdf)

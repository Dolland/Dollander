# Handheld Gaming Console - Master Degree Thesis

As for the title, this project is my Electronics Engineering Master Thesis.
This is a handheld console based on Raspberry Pi Zero 2.

## HOW IT BEGAN

I started working on this idea some years ago and came up designing a console like in the photo:

*FOTO*

As you can see, this was a serious wires mess, but it worked! (actually it still works)
For the first prototipe I used ready-to-use boards for supply, audio, ADC and so on.
The screen was a Composite 5" retro camera 12V display (really bad quality).
The shell was entirely designed from scratch.

## HOW IT BECAME

After a year of use, i decided that this project deserved more attention and started thinking about a custom PCB that would integrate all the components needed for power supply, audio amplification, ADC, display driving etc.
I've designed the PMIC stage, as well as the display interfacing and all the other stuffs.
The PCB finally come out like this:

![photo_2024-11-05_22-15-06](https://github.com/user-attachments/assets/f4265d25-fa0f-4045-a11e-927acb31f033)


The console now has a 5" RGB Parallel Interface display driven by a HDMI-to-TTL converter that receives the HDMI signal from a HDMI switch, that in turn manages to switch the output between the internal display and the HDMI external port.

![photo_2024-11-05_22-15-19](https://github.com/user-attachments/assets/a23613f5-771b-4f65-9f9c-f9f7a5c7527c)


The console has an analog stick, 4 dorsal buttons, 14 front buttons, a speaker (but the PCB supports two speakers), a full-size HDMI output port, a USB-C charging port and a plenty of internal space for Li-Ion cells (i use a 3000mAh one but you can use bigger ones).

This project is by all means not perfect, some things are missing (backlight adjustment is supported by hardware but not implemented in the PCB) and surely the next PCB revision will be more compact (and so cheaper to order) but it works really well.

The design of the shell and the buttons was done in TinkerCAD (what an awful choice) because well, i only know this tool, but surely the next step should be porting all the CAD files into a more professional CAD (Fusion?)

Here is the top printing:

![photo_2024-11-05_22-15-35](https://github.com/user-attachments/assets/42243649-616d-4777-969c-2030cca95662)


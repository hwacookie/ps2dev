This library allows an Arduino to act like a PS/2 keyboard or mouse. It is based on the PS/2 protocol, which is a standard for connecting keyboards and mice to computers.
This is mainly a fork of the existing repo on https://github.com/Harvie/ps2dev/fork. My only addition is the possibilty to pass along a callback function that is called upon a reset of
the keyboard. This can be used to trigger key presses just once after a reset of the keyboard, instead of relying on power-up.

Example given: My use case is a fake PS/2 keyboard that sends ENTER keys upon boot-up to circumvent some pesky POST-errors of the BIOS. This needs to be done every time a computer is reset or powered on.
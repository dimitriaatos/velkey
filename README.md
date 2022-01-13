# VelKey

VelKey is a Max/MSP abstraction that adds velocity sensitivity to computer keyboards by using the amplitude of the keypress sound to determine velocity.

This is particularly easy with laptops using the built-in mic, but is also achievable with other keyboards by attaching a contact mic (piezoelectric disc).

## Prerequisites

- Java

## Disclaimer

- VelKey hasn't been tested, it is thus not guaranteed that it will work with every keyboard and mic.
- Using VelKey might intrigue you to strike the keys harder than usual. Please be aware that hard strikes might cause damage to the keyboard.

## Known issues

- The velocity sensitivity is often inconsistent, keys closer to the mic will be more sensitive than others.
- VelKey is designed for working in a quiet environment, sounds other than the keypress sounds will also affect the velocity values (this is tolerable to a certain degree).
- There can be only one velocity value at a time, when two keys are played simultaneously they'll both have the same velocity value.
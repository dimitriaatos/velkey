# VelKey

VelKey is a Max/MSP abstraction that adds velocity sensitivity to computer keyboards by using the amplitude of the keypress sound to determine velocity.

This is particularly easy with laptops using the built-in mic, but is also achievable with other keyboards by attaching a contact mic (piezoelectric disk).

## Abstractions

- `velkeyin`: this abstraction is a ready to use solution, it includes both the velocity tracking and a keyboard implementation similar to Max's KeyMidi, it can be used like a [notein] object.
- `velkey`: this abstraction implements only the velocity tracking. It can be useful for adding velocity sensitivity to other keyboard layouts.

## Prerequisites

- Java

## Installation

Place the velkey folder to a directory viewable by Max (listed in Max File Preferences).

## Disclaimer

- VelKey hasn't been tested, it is thus not guaranteed that it will work with every keyboard and mic.
- Using VelKey might intrigue you to strike the keys harder than usual. Please be aware that hard strikes might cause damage to the keyboard.

## Known issues

- The velocity sensitivity is often inconsistent, keys closer to the mic will be more sensitive than others.
- VelKey is designed for working in a quiet environment, sounds other than the keypress sounds will also affect the velocity values (this is tolerable to a certain degree).
- There can be only one velocity value at a time, when two keys are played simultaneously they'll both have the same velocity value.

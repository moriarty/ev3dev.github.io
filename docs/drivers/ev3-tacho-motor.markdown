---
autogen: This file was automatically generated by kernel-doc-text-to-markdown.py
title: EV3/NXT Tacho Motor Driver
---

This driver provides a [tacho-motor] interface for EV3 and NXT motors or any
other compatible motor with an [incremental rotary encoder] for position
and direction feedback that is connected to an output port. We call them
"tacho" motors because that is what the LMS2012 source code calls them. You
can find the sysfs device at `/sys/bus/legoev3/devices/<port>:ev3-tacho-motor`
where `<port>` is the the name of the output port the motor is connected to
(e.g. `outA`). There is not much of interest there though - all the useful
stuff is in the [tacho-motor] class.

This device is loaded automatically when a motor is plugged in and the
[ev3-output-port] is set to `auto` or when [ev3-output-port] is set to
`ev3-tacho-motor` mode.

[tacho-motor]: ../taco-motor-class
[incremental rotary encoder]: https://en.wikipedia.org/wiki/Rotary_encoder#Incremental_rotary_encoder
[ev3-output-port]: ../ev3-output-port

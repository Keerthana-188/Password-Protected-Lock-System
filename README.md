# Password-Protected-Lock-System
A simple digital lock system designed using basic logic gates to allow access only when the correct 3-bit password is entered.
# Overview

This project implements a 3-bit password-protected lock using XOR and NOR gates.
A DIP switch is used to set and enter the password, and a push button acts as an Enter key.
The system unlocks (green LED) only when all password bits match; otherwise, it indicates a locked state (blue LED).
The same logic is also verified through Verilog HDL simulation on EDA Playground.

# Components Used

8-pin DIP switch (password + user input)

XOR Gate IC 7486

NOR Gate IC 7402

Push button (Enter switch)

LEDs (Green – Unlock, Blue – Locked)

Resistors & switching diodes

5V / 9V power supply

# Working Principle

1. Each bit of the user input is compared with the preset password using XOR gates.

2. If all XOR outputs are LOW → NOR gate outputs HIGH → Correct password (Unlock).

3. If any bit differs → NOR output LOW → Wrong password (Locked).

4. The Enter push button triggers the verification to avoid false detections.
# Features

Logic-gate–based authentication

Hardware + Verilog HDL simulation

Clear LED indicators for lock/unlock

Low-cost and beginner-friendly digital design

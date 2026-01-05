# System Overview

## Problem Statement
The goal was to enable direct voice communication between two floors of the same building without:
- Mobile phones
- Internet connectivity
- RF-based systems (Wi-Fi, Bluetooth, walkie-talkies)

The solution needed to be **low-cost**, **locally buildable**, and functional over a short but obstructed distance.

## High-Level Concept
Audio signals are transmitted by **modulating the intensity of a laser beam**. The laser propagates through free space, is redirected using mirrors, and is received by a **solar panel**, which converts light intensity variations back into an electrical signal. This signal is then amplified and played through a speaker.

Two identical systems were used on each floor, enabling **full-duplex communication**.

## Signal Flow (One Direction)

Microphone / Audio Source  
→ Audio Amplifier  
→ Laser Diode Intensity Modulation  
→ Free-Space Optical Path  
→ Solar Panel (Optical-to-Electrical Conversion)  
→ Audio Amplifier  
→ Speaker  

## Design Philosophy
The system prioritizes:
- Simplicity over efficiency
- Physical intuition over formal protocols
- Experimentation over optimization



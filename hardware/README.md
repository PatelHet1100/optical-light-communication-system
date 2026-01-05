# Hardware Architecture

## Transmitter Section
- Audio source: Mobile phone via AUX output
- Modulation: Direct audio signal used to vary laser diode intensity
- Laser type: Low-power laser diode module
- Power: Battery powered

No dedicated laser driver IC was used. Audio was coupled directly, which simplified the design but introduced instability and distortion risks.

## Receiver Section
- Optical sensor: Mini solar panel
- Signal conditioning: Audio amplifier module
- Output: Speaker

The solar panel was chosen instead of an LDR due to better signal strength and bandwidth for audio frequencies.

## Power Considerations
- Both transmitter and receiver used battery supplies
- Laser diode heating was observed during extended operation
- No thermal regulation or current limiting was implemented

## Known Weakness
A major design flaw was **routing power and modulation through the audio jack**, which is electrically unsafe and unreliable. This is documented explicitly as a learning outcome.



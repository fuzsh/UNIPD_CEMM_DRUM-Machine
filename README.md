# Drum Machine Step Sequencer (Pure Data)
#### Description
A drum machine step sequencer is a device or software application used in music production to create and program rhythmic patterns for electronic drum sounds. It is a fundamental tool in electronic music production and is often found in hardware drum machines or as a feature in software-based music production environments.

- General Workflow:
  - Active DSP
  - we have bangs for each sound that receive a signal from the sequencer and then read the wav file;
  - send the read file to dac~ to convert the digital file to analog.
- Inside Main Sequencer:
  - There is a toggle that receives a signal for playing or stopping the process;
  - This toggle activates each individual sequence in a connected way.
- Inside Each Sequencer (for each sound):
  - There is an 8-step sequencer;
  - The counter sends a signal to 8 different 'bangs' that then go back to the primary sequencer process;
  - we use spigot to allow the signal through only if the related toggle is on.

---
#### Contributors
- Mirco Cazzaro
- Nicola Boscolo Cegion
- Farzad Shami

<p><em>Computer Engineering for Music and Multimedia course of <a href="http://www.unipd.it">University of Padova</a></em>

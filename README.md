# pekki
Quick expirement I did. This was made because I love the idea of isometric keyboards, but I did not want to shell out hundreds of dollars, so why not make one at home?

This uses Open Stage Control to manage and use the MIDI. It's in a whole tone scale, with an option to transpose the entire scale, with +-6 semitones for moving up and down.

Here is how I get it set up to work on my Macbook + Ableton:

1. Install Open Stage Control.
2. Go into Audio MIDI Setup -> Window "Show MIDI Studio" -> Double-click IAC Driver
3. Click "Device is Online" and add a new bus: OSC MIDI (see image)
<img width="585" height="595" alt="image" src="https://github.com/user-attachments/assets/c8fd21e7-7617-40a8-9b72-7675a7e900bf" />
4. Open Open Stage Control and set the MIDI to (probably) osc:1,1 and hit the play button in the top left.
5. Click the hamburger menu in the top left -> open -. pekki.json
6. If using an external device, go to your macbook's IP at port 8080 (http://192.168.x.x:8080)
7. In Ableton, open Settings -> Link, Tempo & MIDI and add ISC Driver (OSC MIDI) and set it to Track + MPE
   <img width="668" height="729" alt="image" src="https://github.com/user-attachments/assets/9b0e89f1-965a-4070-80b2-2d808d7a617c" />
8. **YOU MUST USE AN MPE COMPATIBLE SYNTH!** I used wavetable and it worked fine.
9. Play!


Disclosure: some of the work was made by ChatGPT 5.5 EDU, because I am too stupid to figure out how OSC works (especially when turning off a note value). Because of that, there's probably some inefficiencies in the JSON. I'm planning on rewriting it to look better at some point in the future.


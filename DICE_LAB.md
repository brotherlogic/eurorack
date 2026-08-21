# Dice Lab: Understanding the Generative Brain

The **ALA Dice** is a clone of Mutable Instruments Marbles. It is best understood not as a traditional sequencer, but as a "randomness tamer." It generates random rhythms and melodies, but gives you precise tools to constrain, quantize, and loop that randomness into musical patterns.

To learn Dice, we'll strip everything else back and sequence a simple drone.

## The Setup (The Canvas)
Let's patch the simplest possible voice so we can hear and see exactly what Dice is doing.
1. **Clock:** Patch **Pam's Out 1** $\rightarrow$ **Dice Clock In (t)** (the 't' section is on the left).
2. **Pitch:** Patch **Dice X1** (bottom middle row) $\rightarrow$ **Chipz OSC 1 Pitch CV**.
3. **Output:** Patch **Chipz OSC 1 Out** (use Triangle or Sine for a smooth tone) $\rightarrow$ **3x MIA** $\rightarrow$ **Output**.

*Note: Since we are not using an envelope or VCA, Chipz will drone continuously. This is perfect for hearing the pure pitch changes without being distracted by volume dynamics!*

---

## Exercise 1: Taming the Melodies (The X Section)

The right side of Dice (and the bottom jacks) handles pitch/voltage generation.

1. **Start Random:** Turn the large **Deja Vu** knob (center right) exactly to 12 o'clock. This means Dice is outputting 100% random new notes every step.
2. **Constrain the Range:**
   * Adjust the **Spread** knob (right side, middle). Turn it all the way down: you'll only hear one note. Slowly turn it up. This knob dictates the "range" or octave span of the random notes. Keep it around 9-10 o'clock for a 1-2 octave range.
   * Adjust the **Bias** knob (right side, top). This shifts the center of the pitch range up or down.
3. **Quantization (The Steps Knob):**
   * The **Steps** knob (right side, bottom) is the magic here.
   * **Counter-clockwise:** Unquantized, smooth, sliding voltages (like an LFO or theremin).
   * **12 o'clock:** Chromatic scale (all 12 piano keys).
   * **Clockwise past 1 o'clock:** It snaps to specific musical scales (major, minor, pentatonic). Turn it to about 2 o'clock—notice how the random notes suddenly sound highly musical and in key!

---

## Exercise 2: Taming the Rhythm (The 't' Section)

The left side of Dice handles rhythm and triggers. Pam's is sending a steady pulse into the `t` clock, but Dice decides what to do with it. Since our drone is continuous, we'll watch the built-in LEDs above the `t1` and `t3` jacks to see the rhythms it generates.

1. **Jitter:** Turn the **Jitter** knob (left side, top) up. Watch the LEDs. You'll see the timing of the triggers start to drift off the grid, feeling more human, sloppy, or drunken. Turn it back down for strict time.
2. **Coin Flip (Bias):** The **Bias** knob (left side, middle) determines how often triggers fire out of `t1` versus `t3`. Turn it left, and `t1` fires constantly. Turn it right, and `t1` stays silent while `t3` gets all the triggers. Watch the LEDs dance between the two jacks! Leave it around 11 o'clock.

---

## Exercise 3: The Deja Vu Magic (Looping)

This is the most important feature of Dice. Random notes are fun, but music requires repetition.

1. **Lock the Loop:** While the sequence is playing and you like the scale/range, slowly turn the large **Deja Vu** knob (center right) clockwise to about 3 o'clock.
2. **Listen:** The randomness will stop, and Dice will lock into a repeating sequence! The "random" buffer is now locked.
3. **Change the Loop Length:** Press the illuminated button below the Deja Vu knob. Each press changes the loop length (it cycles through 1, 2, 3, 4, 5, 6, 7, 8, 10, 12, 14, 16 steps). 
4. **Evolve the Loop:** Turn Deja Vu to 2 o'clock. Now, the loop plays, but there's a 10% chance a step will randomly change. Leave it here, and you have a sequence that plays itself but slowly evolves over time.

### Summary of Deja Vu:
* **12 o'clock:** Total randomness.
* **Far Right (5 o'clock):** 100% locked repeating loop.
* **In between (12 to 5):** A repeating loop that occasionally morphs and mutates.

Spend some time playing with just the **Deja Vu**, **Steps**, and **Spread** knobs. You can generate entire albums just turning these three!

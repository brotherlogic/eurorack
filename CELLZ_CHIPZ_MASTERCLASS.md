# Module Masterclass: Cellz & Chipz

This patch is designed to help you master **Cellz** by using it to control the dual-oscillator nature of **Chipz**.

## The Concept: "Playable Polyphony"
Cellz is not just a sequencer; it's a "programmable touch surface." It has two separate "brains" (Sequencer 1 and Sequencer 2) that can work independently. In this patch, we will use one half of Cellz to play a melody and the other half to play a bassline.

## The Patch

### 1. The Bass (Cellz Sequencer 1 -> Chipz OSC 1)
*   **Patch:** **Cellz CV 1** $\rightarrow$ **Chip 1 "Filter" jack**.
*   **Patch:** **Chipz OSC 1 Out** $\rightarrow$ **3x MIA Section 1, Jack A**.
*   **Action:** Tune Chipz OSC 1 to a low, growly frequency. Touch the pads on the **Left side** of Cellz. You are now manually "playing" the bassline.

### 2. The Melody (Cellz Sequencer 2 -> Chipz OSC 2)
*   **Patch:** **Cellz CV 2** $\rightarrow$ **Chip 2 "Width" jack**.
*   **Patch:** **Chipz OSC 2 Out** $\rightarrow$ **3x MIA Section 2, Jack A**.
*   **Action:** Tune Chipz OSC 2 to a higher pitch. Touch the pads on the **Right side** of Cellz. You now have a two-voice synthesizer!

### 3. The "Automation" (The Magic Trick)
Cellz can "walk" through the notes automatically.
*   **Patch:** **Dice t1** (Gate Output) $\rightarrow$ **Cellz Trig 1**.
*   **Patch:** **Dice t2** (Gate Output) $\rightarrow$ **Cellz Trig 2**.
*   **Action:** Turn up the **Rate** on Dice. Cellz will now start jumping between the pads on its own.
*   **The Discovery:** While it's sequencing automatically, you can still **touch** the pads to "override" the sequence or change the notes stored in them.

## Learning the "Cellz" Interface
*   **Setting Notes:** Hold a pad and turn the knobs on Cellz to change the voltage (pitch) stored in that pad.
*   **Direction:** The buttons at the top change how Cellz moves (Forward, Random, etc.).
*   **The Grid:** Notice how the LEDs move. Cellz is a 16-step grid, but you can define the "Loop" by selecting different start and end points.

## Final Mix (3x MIA)
*   **MIA Knob 1:** Bass Volume (Chipz OSC 1).
*   **MIA Knob 2:** Melody Volume (Chipz OSC 2).
*   **MIA Knob 3:** (Optional) Plug **Mojave** in here to add some "grit" or "space" to the chiptune sounds.

---

### What to listen for:
1.  **Chiptune Vibes:** Chipz is inherently "lo-fi." Use the **Width** knobs on Chipz to change the "pulse width"—this makes the sound go from a thin "reedy" beep to a fat, buzzy square wave.
2.  **Independent Movement:** Because Dice is triggering Trig 1 and Trig 2 at different times, your bass and melody will move at different rhythms, creating complex patterns from simple settings.

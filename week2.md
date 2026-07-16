# Week 2: 5 Minute Eurorack Habit

## Day 1: The Foundation

Based on the 5-minute Eurorack habit outline, "The Foundation" is about building muscle memory for the most fundamental signal path: **Clock -> Sequencer -> Voice -> Output**.

Here is a quick, basic patch using your specific case to build the foundation:

### 1. The Master Clock
* **Patch:** Connect **Pam's Pro Workout Output 1** $\rightarrow$ **ALA Dice Clock In (t)** (the main clock input).
* *Action:* Press play on Pam's. The Dice lights should start dancing to the tempo.

### 2. Pitch (V/Oct)
* **Patch:** Connect **ALA Dice X1** (bottom row, left-most CV output) $\rightarrow$ **ALA Resonate V/Oct**.
* *Action:* Turn the Dice *Rate* knob if you want to change how fast the pattern evolves. 

### 3. Trigger / Gate
* **Patch:** Connect **ALA Dice t1** (top row, left-most trigger output) $\rightarrow$ **ALA Resonate Strum**.
* *Action:* This tells the Resonate *when* to play a note.

### 4. Output
* **Patch:** Connect **ALA Resonate Out** $\rightarrow$ **NiftyCASE Audio Out** (or route it through your 3x MIA first if you want volume control: Resonate Out $\rightarrow$ 3x MIA Section 1 Jack A $\rightarrow$ 3x MIA Out $\rightarrow$ NiftyCASE Audio Out).

### 5. Tweak (The 5 Minute Habit)
Spend the rest of your 5 minutes tweaking:
* Adjust the **Structure** and **Brightness** on the Resonate.
* Play with the **Steps** and **Spread** knobs on the Dice to see how it changes the melody.
* Turn everything off when the 5 minutes are up. **(Correction: Leave it patched for Days 2 & 3!)**

## Day 2: Adding Movement

**Goal:** Modulate the foundation.

**Action:** Power on. Take the patch from Day 1 and add a single source of modulation. 
* **Patch:** Connect **Pam's Pro Workout Output 2** $\rightarrow$ **ALA Resonate Brightness CV In** (or Structure CV In). 
* **Setup (Pam's):** Long-press the knob on Output 2 to edit it. Set it to a slow LFO (e.g., Modifier: `/4`, Wave: `Triangle`).
* **Tweak:** Adjust the small attenuverter knob above the Brightness input on Resonate to dial in the modulation depth. Sit back and listen to how the tone breathes and evolves over a few minutes.
* **Crucial Step:** Leave it patched.

## Day 3: Rhythm & Sequencing

**Goal:** Give it some structure.

**Action:** Power on. Since Dice is already giving us random melodies, let's introduce **Cellz** as a 4-step sequencer to drive a rhythmic bassline using **Chipz**.
* **Patch:** 
  1. Connect **Pam's Pro Workout Output 3** (set to `/2` or `x1`) $\rightarrow$ **Cellz Clock In** (to advance the sequence).
  2. Connect **Cellz CV 1 Out** $\rightarrow$ **Chipz OSC 1 V/Oct In**.
  3. Connect **Chipz OSC 1 Out** $\rightarrow$ **3x MIA Section 2 Jack A**.
  4. Ensure your mix still reaches the **NiftyCASE Audio Out** (e.g., cascade Section 1's Resonate into Section 2's Chipz output).
* **Tweak:** Press the first 4 pads on Cellz and tune the small knobs for each pad to create a simple, repeating 4-step bassline sequence that drives under your Resonate melody.
* **Crucial Step:** Leave it patched.

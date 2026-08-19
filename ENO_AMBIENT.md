# Generative Eno-Style Ambient (2-Day Patch)

Since we're doing a 2-day patch within the 5-minute habit framework, we'll focus on setting up the generative "brain" and sound source today, and then expanding it into a lush, granular soundscape tomorrow. 

Brian Eno's ambient works rely heavily on slow, evolving, generative systems with beautiful, ringing timbres and tape-like textures.

## Day 1: The Generative Bell (Foundation)

**Goal:** Set up a slow, self-playing, bell-like sequence that rarely repeats.

### 1. The Slow Clock
* **Patch:** Connect **Pam's Pro Workout Output 1** $\rightarrow$ **ALA Dice Clock In (t)**.
* **Setup (Pam's):** Long-press Output 1 to edit. Set the modifier to something very slow, like `/2` or `/4` so the clock ticks lazily.

### 2. Generative Pitch & Trigger
* **Patch:** Connect **ALA Dice X1** (bottom row CV) $\rightarrow$ **ALA Resonate V/Oct**.
* **Patch:** Connect **ALA Dice t1** (top row Gate) $\rightarrow$ **ALA Resonate Strum**.
* **Tweak (Dice):**
  * Turn **Steps** to around 2 o'clock so it locks into a repeating loop but occasionally shifts.
  * Turn **Spread** to 10 o'clock to keep the melody within a couple of octaves.
  * *Tip:* Dice will automatically quantize to a scale (likely major or minor pentatonic, which is perfect for Eno).

### 3. The Tone
* **Patch:** Connect **ALA Resonate Out** $\rightarrow$ **3x MIA Section 1 Jack A** $\rightarrow$ **NiftyCASE Audio Out** (cascade it down as usual).
* **Tweak (Resonate):** Set **Structure** to around 11 o'clock (bell-like or sympathetic strings). Turn **Brightness** down to 10 o'clock for a muffled, soft tone. Turn **Damping** way up (2 or 3 o'clock) so the notes ring out for a long time.

**Crucial Step:** Spend a few minutes listening to the slow melody, adjusting Dice's *Chance* or *Steps* knobs until you find a pleasing pattern. **Leave it patched.**

---

## Day 2: The Tape Loop Cloud (Texture)

**Goal:** Process the clean bells into a lush, shifting, granular soundscape, emulating tape loops.

### 1. Route into the Granular Processor
* **Action:** Unpatch Resonate from the 3x MIA.
* **Patch:** Connect **ALA Resonate Out** $\rightarrow$ **Mojave L (Audio input)**.
* **Patch:** Connect **Mojave Out L** $\rightarrow$ **3x MIA Section 1 Jack A**.
* **Patch:** Connect **Mojave Out R** $\rightarrow$ **3x MIA Section 2 Jack A** (to get a wide stereo image).

### 2. Slow Modulation
To give it that organic, breathing Eno feel, we need a slow LFO to gently modulate the granular cloud.
* **Patch:** Connect **Pam's Output 2** $\rightarrow$ **Mojave Size CV In** (or Whirl CV In).
* **Setup (Pam's):** Set Output 2 to an extremely slow Triangle wave (e.g., `/16` or `/32` modifier).

### 3. Tweak the Cloud
* **Tweak (Mojave):** 
  * Turn **Drift** up to capture more of the audio buffer for a tape loop effect.
  * Turn **Gust** up to add a huge, cavernous reverb.
  * Turn **Size** up to create a sustained drone behind the bells.

Now sit back. The Resonate will chime slowly, while Mojave catches those chimes, smears them into a wide stereo cloud, and slowly breathes in and out thanks to Pam's modulation.

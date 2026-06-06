---
name: chords-progression
description: Decode and reverse-engineer complex guitar chord progressions when mid-range frequencies are ambiguous, using outer-voice isolation, harmonic interpolation, and ergonomic validation.
license: MIT
compatibility: opencode
metadata:
  domain: music-theory
  instrument: guitar
---

# Skill: Outer-Voice Chord Transcription

## Objective
To systematically decode and reverse-engineer complex chord progressions in guitar-driven music when mid-range frequencies are ambiguous. This skill relies on isolating outer voices (basslines and high treble notes), applying harmonic interpolation, and validating against instrument ergonomics.

## Prerequisites
- Basic understanding of diatonic chord theory and scale degrees.
- Familiarity with common harmonic functions (e.g., dominant tension and resolution).
- Understanding of standard guitar tuning and fretboard ergonomics (optional but highly recommended for the validation phase).

## Workflow

### Phase 1: Define the Boundaries (The "Bounding Box")
When the middle frequencies are muddy, frame the chord using the extreme frequencies.
- **Pinpoint the Anchor Highs:** Identify the highest ringing notes. Look for static "drones" or pedal points (e.g., sustained open B and E strings) that glue the progression together.
- **Track the Bass Root:** Isolate the lowest note. Do not attempt to determine the chord quality (major/minor) yet; simply find the exact pitch the bass is resting on.

### Phase 2: Analyze the Bassline Topography
Treat the bassline as the engine of the progression and plot its trajectory.
- **Identify the Core Movement:** Determine if the bass is moving in leaps (e.g., functional I-IV-V movements) or moving sequentially step-by-step.
- **Spot the Clichés:** Look for recognizable linear patterns:
  - *The Andalusian Descent:* A whole-step/half-step diatonic drop (e.g., `E -> D -> C -> B`).
  - *The Line Cliché:* A creeping, chromatic descent happening within a single chord family (e.g., `E -> D# -> D -> C#`).

### Phase 3: Harmonic Interpolation (Filling the Middle)
Use music theory to deduce the missing inner voices between the bass and the anchor highs.
- **The Diatonic Default:** Assume the chord fits naturally within the song's established key (e.g., if the key is Em, and the bass is C, assume a C Major chord).
- **Test for Extensions:** If the diatonic chord sounds too simple, check if the high melody notes are turning it into an extended chord (e.g., a bass of C with a high B and E naturally forces a `Cmaj7`).
- **Spot the Tension Generators:** If there is a sudden spike in tension, look for a dominant 7th chord (e.g., `B7` in the key of Em), especially right before a resolution.

### Phase 4: The Ergonomics Check (The Physicality Test)
Use physical playability as a lie-detector test for guitar arrangements.
- **The "Lazy Finger" Principle:** Great arrangers rely on voice leading. Look for progressions where two or three fingers remain perfectly still while only the bass finger moves (e.g., dropping the bass from `C` to `B` to create `C -> Cmaj7/B`).
- **Intra-Measure Slides:** If a bassline moves chromatically within a single measure (e.g., `B7/D# -> Bm7/D`), assume the guitarist is sliding one finger down a single fret rather than jumping to a disjointed chord shape. If a transcribed progression is physically awkward to play, it is likely incorrect.

### Phase 5: Functional Auditing (Debugging the Harmony)
Review the progression as a complete, logical system to iron out any structural bugs.
- **Check for Momentum Loss:** Does the bassline double back on itself awkwardly (e.g., `B -> C -> B`)? If so, test if a chromatic passing chord (like `D# -> D -> C`) creates a smoother, more logical descent.
- **Verify Resolutions:** If a heavy tension chord is introduced (like a secondary dominant or a diminished chord), ensure it actually resolves to its intended target. If the resolution fails, the tension chord was likely misidentified.

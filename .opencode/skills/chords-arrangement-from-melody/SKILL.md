---
name: chords-arrangement-from-melody
description: Derive chord arrangements from a given melody line by analyzing scale degrees, identifying harmonic rhythm, and applying voice-leading principles to build a supporting chord progression.
license: MIT
compatibility: opencode
metadata:
  domain: music-theory
  instrument: any
---

# Skill: Chords Arrangement from Melody

## Objective
To systematically construct a chord arrangement that supports a given melody line. Given only a monophonic melody, this skill produces a complete harmonic framework by analyzing structural tones, inferring harmonic rhythm, and applying standard voice-leading conventions.

## Prerequisites
- Understanding of major and minor scale construction and diatonic chords (I–vii°).
- Familiarity with basic chord functions (tonic, subdominant, dominant).
- Ability to read standard notation, tablature, or MIDI piano roll.

## Workflow

### Phase 1: Melody Analysis — Identify Structural Tones
Strip away ornamentation to find the skeleton of the melody.
- **Remove Passing Tones:** Eliminate stepwise motion between chord tones (passing tones, neighbor tones, appoggiaturas). Circle the notes that fall on strong beats (beats 1 and 3 in 4/4).
- **Find the Tonal Center:** Scan for the note that feels like "home" — often the first and/or last note of the phrase. If the melody uses a key signature or accidentals, deduce the key (e.g., one sharp = G major / E minor).
- **Flag Tension Notes:** Notes outside the diatonic scale (sharps/flats not in the key signature) are likely chromatic passing tones or secondary dominant chord tones.

### Phase 2: Harmonic Rhythm Estimation
Decide how often the chord changes based on the melody's pacing.
- **The One-Chord-Per-Bar Default:** Start by placing one chord per bar. If the melody contains mostly consonant skips (thirds, fifths, octaves), a single chord per bar is sufficient.
- **Subdivide for Busy Melodies:** If the melody changes direction multiple times per bar or contains rapid arpeggios, increase the harmonic rhythm to two chords per bar.
- **Sustain for Static Melodies:** If the melody hovers around 1–2 notes for several bars, stretch the same chord across those bars.

### Phase 3: Chord Assignment — The Harmonization Matrix
Assign a chord to each slot in your harmonic rhythm using the following priority rules.
- **Priority 1 — Bracket the Melody Note:** Choose a chord that contains the strong-beat melody note as its root, third, fifth, or seventh. Prefer root or third for strong beats.
- **Priority 2 — Favor Diatonic Chords:** Within the key, pick the chord whose root is a fifth below or a third above the previous chord's root (circle-of-fifths motion or mediant relationships).
- **Priority 3 — Catch Chromatic Notes with Secondary Dominants:** If a strong-beat melody note is outside the key (e.g., F# in the key of C), place the secondary dominant of its target chord before it (e.g., D7 → G to accommodate that F#).
- **Priority 4 — Check the Bass:** After selecting chords, look at the implied bass motion. Avoid writing a bassline that leaps by an awkward interval (like a tritone) unless the genre demands it.

### Phase 4: Voice Leading — Connect the Chords Smoothly
Make the progression playable and musical by minimizing leaps in the inner voices.
- **Common Tone Retention:** Keep any note shared between consecutive chords in the same voice (e.g., G in Cmaj7 and G7 stays put).
- **Stepwise Motion:** Move voices that cannot be held by the smallest possible interval (prefer a whole or half step).
- **Avoid Parallel Fifths/Octaves:** Do not let two voices move in parallel perfect fifths or octaves — this weakens the independence of the lines.
- **Soprano Anchoring:** Ensure the top voice (the melody) is always the highest note; if an inner voice crosses above the melody, lower it or redistribute the voicing.

### Phase 5: Validation — Playback and Refinement
Audit the arrangement for musicality and correctness.
- **The Melody Test:** Play (or mentally sing) the melody against the chords. If a chord clashes persistently on a strong beat, it is wrong — replace it.
- **The Bass Test:** Play the bass notes alone as a line. The bass should form a coherent counter-melody, not a random sequence of roots.
- **The Simplicity Check:** If the progression sounds overly complex, revert to simpler substitutions (e.g., replace a vii° with a V7, or a iii with a I). The best arrangements often use the most obvious chords.
- **Genre Calibration:** Adjust chord density and extensions to match the target genre:
  - *Pop/Ballad:* Mostly triads, occasional maj7 or sus4, slow harmonic rhythm.
  - *Jazz:* Frequent extensions (9ths, 13ths), ii-V-I patterns, faster harmonic rhythm.
  - *Rock/Punk:* Power chords (root + fifth), minimal voice leading, blocky changes.

# Score Follower

Play a MusicXML score part by part and follow along measure by measure. Built for practicing chamber music: mute your own part and play along with the others.

**Live site:** https://natalieschauser.github.io/score-follower/

## What it does

- Renders the score and highlights the measure being played
- Tempo slider that counts in the score's own beat unit (half notes in cut time, quarter notes in 4/4)
- Metronome with its own volume, plus a 1- or 2-bar count-in before playback
- Mute, solo and volume for each part
- Loop a single measure, jump to any bar, or tap a measure to start there
- Reads standard notation markings: "pizz." and "arco" switch between plucked and bowed sound, and x-noteheads play as percussive chops
- Opens any MusicXML file (`.musicxml`, `.xml`, `.mxl`) exported from MuseScore, Sibelius, Finale or Dorico

Uploaded files stay in your browser and are never sent anywhere.

## How it works

A single `index.html` with no build step. Notation is rendered with [OpenSheetMusicDisplay](https://opensheetmusicdisplay.org/), and sound is synthesized with the Web Audio API. The demo score is J. S. Bach's chorale BWV 66.6 (public domain), from the [music21](https://github.com/cuthbertLab/music21) corpus.

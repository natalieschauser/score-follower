# Score Follower

Play a MusicXML score part by part and follow along measure by measure. Built for practicing chamber music: mute your own part and play along with the others.

## Songs

The site comes with two cello quartet arrangements by Chenoa Orme-Stone, shared here with her permission:

- **Over the Rainbow / What a Wonderful World**: measures 1–78 come from her MusicXML file. Measures 79–131 were converted from the PDF score with [Audiveris](https://github.com/Audiveris/audiveris) and checked by hand, so a wrong note there is possible.
- **Mamma Mia**

You can also open any other MusicXML file with the upload button.

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

A single `index.html` with no build step. Notation is rendered with [OpenSheetMusicDisplay](https://opensheetmusicdisplay.org/), and sound is synthesized with the Web Audio API. The built-in songs are embedded in the page as MusicXML.

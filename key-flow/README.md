# KeyFlow

A responsive piano-learning studio built with Next.js App Router, TypeScript, and Tailwind CSS. The interface includes a VexFlow-rendered grand staff, a playable multi-octave keyboard, Tone.js sound, MIDI input support where available, and sample-data learning, practice, song, progress, settings, and admin pages.

## Run locally

```bash
pnpm install
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000). To type-check the project, run `pnpm exec tsc --noEmit`.

## Main routes

- `/` — KeyFlow landing page
- `/dashboard` — learning overview and practice activity
- `/studio` — interactive piano and notation studio
- `/learn` and `/learn/[courseId]/[lessonId]` — courses and lessons
- `/practice` — note-reading and rhythm exercises
- `/songs` — searchable song library
- `/progress` — learning statistics and achievements
- `/settings` — profile, piano, audio, and learning preferences
- `/admin` — sample course, lesson, exercise, song, MusicXML, and user management

## Studio controls

Use the on-screen keys or the displayed computer-key mapping. Piano notes are shown in the studio and appended to the VexFlow sheet. Tone.js provides synthesized notes and metronome playback. MIDI is opt-in and depends on browser and device support; no hardware is assumed to be connected. The app currently uses frontend sample data and does not claim to persist accounts, sessions, or admin changes to a backend.

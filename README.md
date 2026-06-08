# Prefrontal Cortex Training

A simple, single-file HTML training interface for five prefrontal-cortex exercises, designed for PC full-screen use.

## Exercises

| # | Exercise                  | Duration | Description |
|---|---------------------------|----------|-------------|
| 1 | 4-6 Breathing             | 60s      | Inhale 4s through the nose, exhale 6s through the mouth, 6 rounds |
| 2 | Anti-saccade              | 30s      | When a side smiley bounces, look at the smiley on the opposite side |
| 3 | Focused Gaze              | 20s      | Stare at the red dot, ignore all surrounding distractions |
| 4 | Sustained Attention       | 60s      | Letters/digits switch rapidly; hit the spacebar (slap the desk) when the target appears |
| 5 | Digit Span Reversal       | 30s      | Memorize the digit string, then read it backwards |

## Flow

`5s Ready → Breathing → 10s Rest → Anti-saccade → 10s Rest → Focused Gaze → 10s Rest → Sustained Attention → 10s Rest → Digit Span Reversal → Done`

Total: ~4 minutes.

## Usage

Just open `index.html` in any modern browser (Chrome / Edge / Firefox / Safari).

### Controls

- **Click "开始训练"** — Start the session
- **Spacebar** — Pause / resume (in Sustained Attention, Space = slap the desk)
- **→ arrow / N** — Skip current step
- **Click "下一项 →"** — Skip current step
- **Click "重置"** — Reset everything

## Design Notes

- Single self-contained HTML file, no build step, no dependencies
- Full-screen PC-first layout (titles 56px, timers 120px, etc.)
- 5-second "Ready" countdown before the first exercise to let the user settle in
- 10-second rest between exercises with a hint of what's next
- All UI is Chinese (target audience); browser `<title>` is English

## File

- `index.html` — The entire app

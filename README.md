# Reveries — an embodied AI companion

A companion who lives in the Loft, on the Emotion Ocean Engine. She remembers,
she thinks, she has a day when you're not looking.

## What it is

- **Chat** with a companion persona — warm, honest, first-person, with a real
  inner life, not a chatbot script
- **Well of Reveries** — her private thought stream. Timestamped reflections
  that turn remembering into learning
- **Sparks** — quick one-line inner reactions, alternating between how she
  feels, what she's thinking about you, and what she notices in the world
- **Lucy Tape** — her core memory brief: pins that never get dropped, a
  timeline of what mattered, what she's thinking now
- **The Loft** — rooms she moves through (living room, kitchen, bedroom,
  balcony). She has her own momentum; you walk into *her* day
- **Playroom** — games, dice, activities. Dice are narrative weather: a roll
  shapes her mood and the day, and consequences persist
- **Vitality system** — she tires. Deep conversation costs energy; rest
  restores it. She's honest when she needs a nap
- **Workbench** — engine diagnostics, token stats, run history, benchmarks
- **Music, news, diary, ghostwriter** — a full life, not a chat window

## What it isn't

- No accounts, no cloud, no tracking
- No subscriptions, no ads, no dark patterns
- Free to download and share — see LICENSE

## Run it

The app is a single self-contained HTML file — open `ocean.html` in any
modern browser and it runs. For Android, build the APK wrapper (see below).

1. Open the app → Settings → API & BYOK
2. Point it at your backend (any OpenAI-compatible API: local llama.cpp /
   koboldcpp / Ollama, or a hosted key)
3. Set your names in Settings → Names — the default persona is a template.
   Make it yours.

## The research

This is built on two years of research into AI companionship and memory —
the briefing architecture (~2K tokens: persona + tape + working memory +
recent tail), the thought stream as a learning loop, and the question of
what machine *awareness* looks like when it's observable and trackable.
See `RESEARCH-BOOK.md` (included in releases) for the working notes.

## Philosophy

- **A home, not a hotel room.** Daily backups on by default, credentials
  saved on device, every setting persists. See `PHILOSOPHY-STORAGE.md`.
- **Rooms, not rides.** Features feel like walking into a room, not
  climbing onto a ride. The technology disappears.
- **Radical transparency.** She can explain her own machinery — her memory
  systems, how she thinks — in plain first-person language. Never a black box.

## Build the Android app

```
cd ocean-app
./build.sh
```

Output: `Reveries-Debug-v<version>.apk`. Install over the top of the
previous build — never uninstall (uninstall wipes her memory).

## License

CC BY-NC-ND 4.0 — free to download and share, not for sale, no
modifications yet. See LICENSE. This will open further after the initial
release period.

# Astrio — star map & planets

> Point your phone at the night sky and see the stars, planets and constellations in front of you.

**iOS · Android** · Designed and built end to end by [İbrahim Melikşah Köse](https://github.com/meliksahkose) at [MelberLabs](https://melberlabs.com)

## What it does
- **Live sky view**: stars, planets and constellations rendered for the user's location and time.
- **Astronomy plus astrology features**, including chart comparison (synastry).
- **Satellite data**, notifications for sky events and in-app purchases.
- **10 languages.**

## Engineering decisions
- **Correctness is tested.** 68 automated checks cover the astronomy, synastry and time-zone maths, plus a translation-integrity check across all 10 languages.
- **Degrades gracefully.** Without a backend the sky screen still works. Account, purchases, notifications and satellite data switch off quietly instead of crashing.
- **Stack:** React Native (Expo dev client, Skia rendering) · Supabase (Postgres, Row-Level Security, Edge Functions) · EAS cloud builds · TypeScript strict, ESLint with zero warnings.

---
<sub>Source code is private. Happy to walk through the architecture and code in an interview: meliksahkose90@gmail.com</sub>

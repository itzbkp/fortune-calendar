<img width="800" height="520" alt="fortune-calendar" src="https://github.com/user-attachments/assets/d13dc914-c36f-4633-b293-9ea40f8b2850" />

# Fortune Calendar — Monthly Edition

The application displays favorable and unfavorable days in a month, based on your birth-star, using the traditional Vedic frameworks and core principles of Nakshatra Chakra and Panchang.

## What it does

- Computes the Moon's position for every minute of every day using an **ELP2000/60-term trigonometric series** for lunar longitude, combined with the **Lahiri ayanamsa** to convert to sidereal position.
- Determines which of the 27 **nakshatras** the Moon occupies at any moment, and tracks when it transitions from one to the next.
- Maps each day's nakshatra(s) to a **Tara** (one of 9 categories — Janma, Sampat, Vipat, Kshema, Pratyari, Sadhana, Naidhana, Mitra, Atimitra) relative to your selected birth nakshatra, and classifies each as favorable or unfavorable.
- Renders a monthly calendar grid where each day's card is colored according to its tara(s).

## Features

- **Birth Nakshatra & Month controls** — pick your birth nakshatra and browse any month; selections persist across sessions.
- **Simple / Detailed view toggle**:
  - *Simple*: each day shows a solid color based on the single dominant tara during the 9 AM–12 AM (next day) window.
  - *Detailed*: each day shows a gradient reflecting all tara transitions across the full day, with the short nakshatra codes for each segment.
- **Hover tooltips** on any day showing a 24-hour timeline with nakshatra transition points, tara-colored line segments, and a breakdown table of nakshatra/tara per segment.
- **Overview modal** explaining the color coding, with an expandable reference table of all 9 taras and their meanings.
- **Performance**: nakshatra transition times are found via binary search rather than a minute-by-minute scan, making month recalculation near-instant.

## Tech

Plain HTML/CSS/JavaScript — no build step, no dependencies. Open `index.html` directly in a browser.

## Disclaimer

This application is intended for informational and educational purposes only. Results are based on astrological principles and ephemeris data and should not be considered predictions or professional advice.

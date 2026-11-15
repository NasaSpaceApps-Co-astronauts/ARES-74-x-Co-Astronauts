# ARES-74 × Co-Astronauts – NASA Space Apps Challenge

## Project Summary
ARES-74 × Co-Astronauts is an integrated health and crew support platform designed to support astronaut health, wellbeing, and operational safety throughout a mission. Human spaceflight involves a constant interplay of physiological, psychological, and environmental factors, and treating them separately can delay the detection of emerging risks. The platform brings astronaut health monitoring, spacecraft environmental data, medical guidance, psychological support, and biomedical equipment data together in a single, accessible web interface, designed for situations where real-time medical support from Earth is delayed.

## Live Demo
- Demo: https://coastronautshealthtracker.netlify.app
- Demo video: (https://drive.google.com/drive/folders/1ATVacuyMAf9cSwrYo6vKOZrpPv77j9aX)

## Key Features
- **Crew telemetry dashboard:** heart rate, HRV, strain, sleep/recovery, SpO₂ and radiation dose for 4 crew profiles.
- **NASA HRP risk monitors:** 8 spaceflight risk panels (SANS, bone and renal, muscle, vestibular, immune, microbiome, decompression, teamwork and nutrition).
- **Health Guidance:** 15 conditions in a Green / Amber / Red system, with full explanation pages and action protocols.
- **Habitat and space weather feed:** cabin pressure, temperature, O₂ and CO₂, ISS orbit, NOAA proton flux and Kp index, NASA DONKI alerts.
- **AURA chat (PIN protected):** Psychologist, Flight Surgeon and Ops Copilot roles, with a local adaptive response engine and an optional backend (`/api/chat`) connection.
- **Wellbeing tools:** 4-7-8 breathing pacer, Earth soundscapes (Web Audio API), daily psychological check-in.
- **Loved Ones Voice Vault:** record or upload personal audio messages.
- **Vital renewal reminders:** timers for heart rate, radiation, SpO₂, blood pressure and temperature checks.
- **30 Medical Devices Guidebook:** breakdown signs, self-tests and backup actions, with a downloadable guide and a simulated NASA CHeCS anomaly report form.
- **NASA CSV importer:** load NASA datasets or the HRP telemetry template and play them back.

## Technologies
- HTML5, CSS3, vanilla JavaScript (single-page application, `index.html`)
- Web Audio API (offline soundscapes)
- MediaRecorder API (voice recording)
- Browser localStorage (voices, reminders, chat history, reports)
- Optional backend endpoint for AURA (`/api/chat`, Gemini-based), with automatic local fallback

-Netlify(hosting)

## Data Sources
- NASA ISSLIVE (Lightstreamer) – ISS cabin telemetry
- wheretheiss.at – ISS orbit and altitude
- NOAA SWPC – GOES proton flux and planetary K-index
- NASA DONKI – space weather notifications
- NASA Human Research Program risk areas: https://www.nasa.gov/hrp/risks/
- NASA Astronauts CSV (public dataset)
  
## Important Notes
- Crew biometric values are **simulated presets** for demonstration. They can be replaced through a CSV file or a REST/WebSocket feed.
- The "Submit to NASA" device report is a **simulated workflow** saved locally in the browser.
- The AURA demo PIN is `1969`. This is a prototype lock and not real security.
- This is a prototype and does not replace professional medical advice.

## How to Run
No installation needed. Open the live demo at https://coastronautshealthtracker.netlify.app, or download `index.html` from this repository and open it in a browser. An internet connection is needed for live NASA/NOAA feeds. If a feed is unreachable, the app continues with preset data.

## Team
| Member | Role |
|---|---|
| Pınar Aslan | Scrum Master | Araştırma ve Veri|
| Elif Örnek | Geliştirici ve Lider | Netlify canlı yayın, demo linki ve demo videosu, SpaceApps Teslimi|
| Zeynep Ece Kayaboynu |Ürün/İçerik|Araştırma ve Veri|Hata düzeltme ve testler |
| Günsu Bostancı |Araştırma ve Veri|Hata düzeltme ve testler |

## Sprint Reports
- [Sprint 1](docs/sprints/sprint-1-raporu.md)
- [Sprint 2](docs/sprints/sprint-2-raporu.md)
- [Sprint 3](docs/sprints/sprint-3-raporu.md)
- [Sprint 4](docs/sprints/sprint-4-raporu.md)

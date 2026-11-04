# SOOMi Sleep Check

**A free, 5-minute sleep health self-check on your phone.** No sign-up, no server, nothing saved.

**Try it:** [sleep-check.soomihealth.care](https://sleep-check.soomihealth.care) (in Korean, best on a phone)

Built at **[SOOMi Health](https://soomihealth.care)** by a non-developer founder working with AI coding agents. This repository is an overview; the source code is private.

![Welcome, a question, the goals screen, and the result summary](screens.webp)

> **Not a medical diagnosis.** The results help you reflect on your sleep. If a symptom worries you, talk to a sleep specialist.

---

## Why it exists

Snoring and daytime tiredness are easy to ignore, and many people never mention them to a doctor. This self-check is a free first step: in about five minutes, a person puts their sleep into words and gets a one-page report they can bring to a clinic.

SOOMi Health also builds [CareLoop](https://github.com/sylvie-kim/careloop), an operations console for sleep clinics and CPAP providers.

## What it checks

22 questions in four short parts, in Korean:

| Part | Questions | What comes back |
|---|---|---|
| Sleep pattern | 4 | Time to fall asleep, night awakenings, how mornings feel |
| Daytime sleepiness | 9 | A daytime sleepiness score from everyday situations (based on the Epworth Sleepiness Scale) |
| Breathing during sleep and health | 7 | A count of sleep apnea risk signals (based on STOP-Bang) |
| Habits and goals | 2 | Sleep habits you already keep, and what you hope changes |

The report opens with a summary grid, then one screen per result in plain words, a guide matched to the answers, and a short explainer on the overnight sleep test.

## Design choices

- **One question per screen**, answers at thumb height. Single-choice answers move on as soon as you tap.
- **Night questions, morning bookends.** Questions sit on a calm dark screen; the welcome, goals, and results use a bright morning look.
- **A clipboard that checks itself.** On the welcome screen, a pencil ticks off common warning signs one by one.
- **A sprout that grows** with each goal you pick, and again on the result summary.
- **Plain words on screen.** Questionnaire names never appear; each result is explained in everyday language.

## Privacy

- No login. The app never asks for a name, email, or phone number.
- Answers live only in the page's memory and disappear when the tab closes. No cookies, no storage, no analytics.
- Results can be sent to your own KakaoTalk or mail app from the phone. They never pass through SOOMi Health.

## Built with

React · TypeScript · Vite · Tailwind CSS · framer-motion. Static site, no backend.

---

Contact: [soomihealth.care](https://soomihealth.care)

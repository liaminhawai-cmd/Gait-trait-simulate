# Evidence-Based Gait Trait Simulator

An interactive, single-file web app that visualizes how psychological and
neurodevelopmental traits relate to **observable walking patterns** — and, for
each mapping, cites the gait-research literature it draws on along with an honest
rating of how strong that evidence is.

Open [`index.html`](index.html) in any modern browser. No build step, no
dependencies, no network required (web fonts are progressively enhanced).

## What it does

- **9 trait sliders** — Autism (ASD), ADHD, Anxiety, Depression, Mania,
  Dissociation, Arousal, Confidence, Aggression.
- **Real-time 3/4-view walker** driven by inverse-kinematics limbs and
  spring-damped arm/trunk dynamics, with step-locked variability noise.
- **Evidence panel** — for the trait you're adjusting, shows the reported gait
  features (with direction of effect), a plain-language summary, an
  evidence-strength badge, and key references.
- **Live gait metrics** — speed, cadence, stride length, base of support, arm
  swing, trunk flexion, and gait variability, expressed in approximate
  real-world units.
- **Presets** for common profiles, plus style toggle, skeleton overlay, motion
  trail, reset, and "copy settings".

## Evidence strength ratings

Each trait→gait mapping is tagged so the science isn't overstated:

| Rating | Meaning |
| --- | --- |
| **Strong** | Replicated, motion-capture-quantified (e.g. depression) |
| **Moderate** | Multiple supporting studies, some heterogeneity |
| **Emerging** | Indicative / indirect (e.g. actigraphy, DSM-level) |
| **Speculative** | Inferred from theory; little direct gait data |

### Key sources

- **Depression** *(strong)* — Michalak et al. (2009), *Psychosomatic Medicine*
  71:580–587; Lemke et al. (2000).
- **Autism (ASD)** *(moderate)* — Kindregan, Gallagher & Gormley (2015);
  Hallett et al. (1993); Nayate et al.
- **ADHD** *(moderate)* — Manicolo et al. (2017); Papadopoulos et al. (2014).
- **Anxiety** *(moderate)* — Staab (2012); Feldman et al. (2019); cautious-gait
  literature.
- **Aggression / Confidence** *(moderate)* — Satchell et al. (2017),
  *J. Nonverbal Behavior* 41:35–44.
- **Mania** *(emerging)* — DSM-5 psychomotor activation; actigraphy.
- **Dissociation** *(speculative)* — embodiment / depersonalization theory.

Full citations are shown inside the app's Evidence panel.

## Important caveat

These are **group-level statistical associations** — averages across studied
populations, not a way to diagnose or "read" any individual. Many effects are
small and overlap heavily with typical gait. This is an educational
visualization, **not a clinical instrument**.

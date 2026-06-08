# Cogni-Action Project -- Paper 1: Analysis Code

Companion code for the following publication:

  Martinez-Flores, R., Julio, C., Ibanez, R., Campos-Rojas, C., Jarpa, M.,
  Super, H., Tari, B., & Cristi-Montero, C. (2025).
  Impact of physical activity modalities on text processing and comprehension
  in adolescents. The Journal of Experimental Education, 1-16.
  https://doi.org/10.1080/00220973.2025.2513244

---

## Description

Mixed-effects models examining the effect of three physical activity
conditions (SC, MICT, C-HIIT) on text processing and reading comprehension
in adolescents. A crossover trial with 32 participants.

Outcomes analyzed:
- Average pupil dilation (cognitive load indicator): LMM
- Fixation duration: GLMM (inverse Gaussian, log link)
- Number of fixations: GLMM (Poisson, log link)
- Reading comprehension scores (CS, BT, MS): GLMM (Poisson, log link)

Two model sets:
- Without pupil diameter: total effect of condition on comprehension
- With pupil diameter as covariate: direct effect controlling for
  cognitive load (mediation logic)

Random effects: participant and item (text) in all models.

---

## Important notice

This script is shared as companion code to the published paper above.
It reflects the analysis exactly as submitted and accepted.
It should not be adapted or applied to a new dataset without
understanding the original design and research question.

For guidance: ricardo.antonio.martinezf@gmail.com

---

## Requirements

    install.packages(c("lme4", "fitdistrplus", "tidyverse",
                       "ggplot2", "sjPlot", "emmeans", "ggeffects"))

---

## Author

Ricardo Martinez-Flores
PhD(c), Institute of Neurosciences, University of Barcelona
Cogni-Action Project, Pontificia Universidad Catolica de Valparaiso, Chile
ricardo.antonio.martinezf@gmail.com
https://github.com/ricardo-martinez-flores

---

## License

CC BY 4.0 -- Ricardo Martinez-Flores
https://creativecommons.org/licenses/by/4.0/

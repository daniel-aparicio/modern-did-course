# Modern Difference-in-Differences and Synthetic Control

Slides for a short course on difference-in-differences with staggered, non-binary, non-absorbing and continuous treatments, and on synthetic control methods. Daniel Aparicio-Pérez, Universidad de Valencia.

The deck is the result of several editions of the course taught in 2025 and 2026. It is a single Beamer document of about 165 slides, in English, with Stata as the main software (R for the continuous-treatment module).

## Contents

| Block | Topic | Main references |
|---|---|---|
| 0 | TWFE and why it fails under heterogeneous effects | Goodman-Bacon (2021); de Chaisemartin & D'Haultfœuille (2020); Sun & Abraham (2021) |
| 1 | Staggered binary treatment | Callaway & Sant'Anna (2021); Sant'Anna & Zhao (2020) |
| 2 | Non-binary and non-absorbing treatments, five applied cases | de Chaisemartin & D'Haultfœuille (2020, 2024); `did_multiplegt_dyn` |
| 2, continued | Continuous treatment | Callaway, Goodman-Bacon & Sant'Anna (forthcoming, *AER*) |
| 3 | Synthetic control and synthetic DiD | Abadie (2021); Arkhangelsky et al. (2021); Clarke et al. (2024) |

Every figure in the deck is produced by Stata or R code shown on the slides, run on the replication data of the paper discussed. The code and the data are not part of this repository.

## Files

    Slides/main.tex             main document (Beamer, Metropolis theme, 16:9)
    Slides/Block0_TWFE.tex      Block 0
    Slides/Block1_CS.tex        Block 1
    Slides/Block2_dCH.tex       Block 2
    Slides/Block2b_contdid.tex  Block 2, continuous treatment
    Slides/Block3_SCM.tex       Block 3
    Slides/Recaps.tex           recap and closing frames (macros)
    Slides/figures/             figures, one folder per block
    Slides/main.pdf             compiled deck

Each `Block*.tex` is a `subfiles` document, so it compiles on its own or through `main.tex`.

## Compiling

    cd Slides
    pdflatex -interaction=nonstopmode main.tex
    pdflatex -interaction=nonstopmode main.tex

Two passes, for the page counter and the internal references. Use `pdflatex`; the deck does not need `xelatex` or `lualatex`.

## License

The slides are released under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0). You may share and adapt them, including for teaching, provided you credit the author.

## Contact

Daniel Aparicio-Pérez, Department of Economic Analysis, Universidad de Valencia. daniel.aparicio@uv.es

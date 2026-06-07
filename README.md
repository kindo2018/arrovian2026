
# Arrovian Possibility: Sheaf-Theoretic Navigation
This repository contains the Prolog implementation and computational experiment data for the paper:  
**"Holonomic Information Management: Sheaf-Theoretic Navigation of Arrovian Possibility"** (JSAI-IS AiBiz 2026).


## 1. Overview
This project provides a novel framework to formalize organizational decision-making as a **patching problem** of local preferences within a **sheaf**. While Arrow's Impossibility Theorem identifies topological obstructions to global consistency , this methodology identifies and excises these "singularities" to restore **Arrovian Possibility** within maximal consistent domains.

### Key Features
* **Sheaf-Theoretic Formalization**: Modeling preference aggregation as a section-patching problem over a simplicial complex.
* **Singularity Excision**: Systematically identifying and removing intransitive triples (topological obstructions) using Alexander duality.
* **Prolog Implementation**: A rigorous, recursive functional generator for exhaustive search and verification of maximal consistent regimes. So, the axiomatic theories of social choice can be intuitively described as a logical formula and is well-suited for exhaustive search..
* **Prevalence Analysis**: Quantitative mapping showing that consistent domains cover 85% to 97% of the total preference space.



## 2. Theoretical Background
The framework uses **Abstract Managerial Information Schemata (AMIS)** to bridge the gap between social choice axioms and algebraic topology:
* **IIA (Independence)**: Guaranteed by binary decomposition.
* **Transitivity**: Formalized as the sheaf consistency condition.
* **Holonomy**: Detecting systemic failures via parallel transport around cycles in the organizational structure.

## 3. Repository Structure
* `/prolog`: Contains the core recursive functional generator (main.pl) for generating binary aggregation rules and obstruction collecting, inequality indices (iex_n2.pl), a helper program (lib2025.pl), and profile-based aggregation rule generation (or only for verification is also beneficial)  with various experimentation results including using the decisiveness implication schema (arrow2025.pl).
* `/data`: Results for various cases $(n, m)$, including maximal possibility rules, minimal cuts (obstructions), as prolog programs.
* `/docs`: Specific examples with text based figures of maximal governance rules, such as the $n=2, m=4$ case presented in the paper.


## 4. How to Run the Experiments
The code is implemented in **Prolog**. To reproduce the results shown in the paper:

1. Install a Prolog interpreter (e.g., SWI-Prolog).
2. Load the main generator:
   ```prolog
   ?- [main].
   ```
3. See demos in the source codes.

## 5. Key Results
Our experiments reveal that topological "No-go" zones are concentrated in sparse singularities, restoring practical possibility for information management.
* **Prevalence Ratios**:
  * $(n, m) = (2, 3)$: 94.4% 
  * $(n, m) = (2, 4)$: 87.5% 
  * $(n, m) = (2, 5)$: 85.0% 
* **Symmetry**: Odd-numbered groups ($n=3$) can achieve perfect fairness (inequality index $1/3$), unlike even-numbered groups.

## 6. Citation
If you use this code or framework in your research, please cite:
Indo, K. (2026). Holonomic Information Management: Sheaf-Theoretic Navigation of Arrovian Possibility. In: Morinaga, S., Nakano, Y., Tono, K. (eds) New Frontiers in Artificial Intelligence. JSAI-isAI 2026. Lecture Notes in Computer Science(), vol 16608. Springer, Singapore. https://doi.org/10.1007/978-981-92-1527-0_12
```bibtex
@inproceedings{Indo2026holonomic,
author="Indo, Kenryo",
editor="Morinaga, Satoshi
and Nakano, Yukiko
and Tono, Katsuya",
title="Holonomic Information Management: Sheaf-Theoretic Navigation of Arrovian Possibility",
booktitle="New Frontiers in Artificial Intelligence",
year="2026",
publisher="Springer Nature Singapore",
address="Singapore",
pages="182--197",
doi ="10.1007/978-981-92-1527-0_12",
isbn="978-981-92-1527-0"
}```
## Notes & Ackowledgements
This work will be primarily presented at JSAI-IS AI Biz 2026 (June 2026, Takasaki, Japan). Preliminary findings related to certain experimental results were previously shared during the Decision Making session at the 2026 Spring Conference of the Operations Research Society of Japan (ORSJ), held at Reitaku University from March 4th to 6th, 2026. The core codebase for those experiments remains substantially consistent with this repository (see https://github.com/kindo2018/or2026).

---

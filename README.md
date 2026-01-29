# The Harness Thesis: Reliability is the next Frontier

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18416449.svg)](https://doi.org/10.5281/zenodo.18416449)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

In late 2025, a six-person startup named Poetiq surpassed Google on ARC-AGI-2, the most demanding benchmark for machine reasoning, achieving 54% accuracy against Gemini 3 Deep Think's 45% while spending half the compute budget. They trained no foundation models. They built a better harness. Their system generated candidate solutions, tested them against puzzle constraints, analyzed failures, and iterated, averaging fewer than two model requests per problem through aggressive stopping criteria. The same frozen foundation model performed dramatically better when embedded in infrastructure designed to verify and refine its outputs. That result exposes a structural misalignment in how the industry has pursued artificial intelligence.

Capability scales along two axes. The first is model scale: raw parameters, training compute, and the statistical patterns encoded through pre-training. The second is harness sophistication: the intelligence of verification layers, refinement loops, and preference systems that wrap the model. Industry has allocated hundreds of billions to the first axis while leaving the second largely unexplored. The returns have inverted. Harness sophistication now yields higher performance returns than additional training runs, yet enterprise adoption remains stalled because this infrastructure remains underdeveloped. While 88% of enterprises use AI, only 6-7% achieve value at scale. The barrier is reliability, not capability, and this reliability problem fractures along two distinct dimensions rooted in the stochastic nature of language models.

Formal reliability degrades through compounding error. A model achieving 95% accuracy on individual steps yields just 36% success probability across twenty sequential steps, and enterprise workflows routinely involve dozens of decisions where a single error cascades through everything downstream. Worse, models cannot verify their own work reliably because the verifier shares the generator's blind spots. Preference reliability suffers from the opposite pathology: excessive convergence. Models regress toward the mean of training data, generating competent but generic outputs that cannot capture the specific judgment differentiating one expert from another. Two equally competent lawyers draft different contracts reflecting different risk tolerances. Current AI cannot learn these tacit preferences.

This paper proposes the Harness Architecture as the resolution. An orchestrator governs iteration loops, allocating test-time compute optimally and stopping aggressively when evidence converges, converting inference budget into tunable reliability. A verification layer breaks the self-verification paradox through heterogeneous checking: formal provers like Lean for closed domains where truth is binary; parameterized simulation for complex domains where verification generates calibrated confidence distributions under explicit assumptions. A preference learning system captures expertise from implicit signals—choices, edits, rejections—without modifying model weights, learning what specific individuals consider good rather than what training data averaged. The frozen foundation principle keeps models interchangeable substrates while embedding adaptation in external infrastructure that can be inspected, versioned, and audited.

These capabilities lead to the Convergence Thesis: robust verification of complex, open-world claims eventually requires the same capabilities as generating those claims reliably. Statistical patterns cannot verify causal claims without world models capable of counterfactual simulation. The verification gap and the AGI gap are identical. Building this infrastructure constitutes building the path to general intelligence. The trajectory unfolds through four phases. Foundation loops mature now, delivering production reliability exceeding 95% for code and compliance. Domain loops follow from 2026-2028, deploying semi-automated verification for legal and medical analysis with human oversight. Differentiation loops emerge from 2026-2029 as preference learning externalizes expertise capture, making generic AI personal. World model integration culminates from 2027-2030, approaching the AGI threshold through causal simulation. Organizations that invest in domain formalization and capture preference signals today accumulate judgment data that becomes their moat tomorrow.

---

**Citation**

```bibtex
@misc{doose2026harness,
  author       = {Doose, Karl},
  title        = {The Harness Thesis: Reliability is the Next Frontier},
  month        = jan,
  year         = 2026,
  publisher    = {Zenodo},
  version      = {1.0},
  doi          = {10.5281/zenodo.18416449},
  url          = {https://doi.org/10.5281/zenodo.18416449}
}

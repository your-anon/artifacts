# Anonymous Artefact Release


## Contents

- `probe_v3.json` — the 57-item probe over the IDMC Global Report on
  Internal Displacement 2024. Each item contains a question, a gold claim,
  a near-miss distractor, a far-miss distractor, and five pre-written
  answer versions (correct, ATT-near, ATT-far, SUB-near, SUB-far) used in
  the 2x2 error-class x numeric-distance design described in Section 4.

- `questions_ambiguous.json` — a 12-item surface-ambiguous pilot probe,
  constructed for the rebuttal, using gold values already present in
  probe_v3.json but with temporal/type cue words removed from the question
  text (Section 6 / Limitations discussion of lexical leakage).

- `pilot_ambiguous.py` — the script used to run the surface-ambiguous
  pilot through the full generation pipeline.

- `pilot_ambiguous_results.json` — the real generator outputs for the
  surface-ambiguous pilot, run through the full pipeline (hybrid retrieval
  + reranking + parent passages + self-consistency).

- `JUDGE_PROMPTS.txt` — the exact prompts used for the faithfulness and
  answer-relevancy judges reported in Table 1 and Appendix C.

- `LICENSE.txt` — CC BY 4.0, matching the license of the accompanying
  paper submission.

## Release policy

Every item is released with its gold type and error-class labels. No
generated incorrect answer is released detached from its label, consistent
with the Ethics Statement in the submission.

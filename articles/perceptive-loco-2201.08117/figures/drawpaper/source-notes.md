# DrawPaper source and compilation notes

Paper: Learning robust perceptive locomotion for quadrupedal robots in the wild, author PDF compiled January 20, 2022 (22 pages).
Official source: https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf
SHA-256: `7e1c08c712ba96c2ada559285191a37fb37b9e3faf297670315a13d80ac75f55`.

The four final diagrams combine unmodified viewports from the retained built-in imagegen draft with independently typeset Chinese labels, exact mathematics and verified arrows. The draft is an illustration source; its proposed decoder arrangement is not the scientific final. All final diagrams share the adjacent `perceptive-loco-imagegen-draft.png` dependency. Compile each `.tex` from this directory with XeLaTeX, TeX Live 2026, Arial and macOS STHeiti Light/Medium fonts. The seven standalone equation sources use pdfLaTeX and Computer Modern mathematics.

## Scientific checks

- A: 208 height samples and 133 proprioceptive/command values. B: privileged teacher learns with PPO and clean simulation data.
- C: two GRU layers of 50 units; a 96-dimensional gate attenuates only the direct exteroceptive feature branch. Append 24 zeros before addition to the 120-dimensional recurrent representation. Noisy height features still enter the GRU. Proprioception plus belief enters the action MLP.
- D: 4 phase corrections and 12 joint residuals become 12 joint targets through nominal foot trajectories and inverse kinematics; they are not 16 torques.
- E: the student visits states and the fixed teacher labels those states. Behavior cloning and reconstruction independently contribute to the total loss. The decoder reads recurrent hidden information plus raw noisy heights through its own gate; targets are 208 heights plus 50 privileged values, not the 120-dimensional belief vector.
- F: mapping at 20 Hz and control at 50 Hz. Deployment updates hidden state, not trained parameters. Teacher and reconstruction supervision are absent from the deployed control path.

These checks refer to author-PDF pages 11–14 and supplement S3/S5/S6 on pages 17–18. The author PDF has a figure-number mismatch: its page 7 comparison is referenced as Fig. 4 without a printed caption; actual captions on pages 9, 10 and 13 read Fig. 4, Fig. 5 and Fig. 6. Page plus caption identity is retained in the manifest.

## Reuse and attribution

The cover and draft were created with built-in imagegen. They are conceptual illustrations. Original paper excerpts retain their original copyright; arXiv nonexclusive distribution was not interpreted as a Creative Commons license. Only selected excerpts used in scientific commentary are registered. The source PDF is not included.

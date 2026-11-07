# DeepMimic architecture specification

## Source and visual goal

Source: author-hosted ACM TOG / SIGGRAPH 2018 final paper, 18 pages including supplementary material, `DeepMimic_2018.pdf`. SHA-256: `c57cdd325b4bb921d95a5feb2742bdf016d48412ed969ea5f4ee2fe05e22db30`. This is not asserted to be byte-identical to an arXiv version.

The diagram answers how a reference motion becomes an executable simulated control policy and how three distinct skill-organizing options differ. Five stacked regions share a 340 bp mobile reading width. The humanoid illustrations represent simulation, including contact and gravity; they do not represent a physical robot experiment.

## Regions and scientific mapping

| Region | Input | Computation | Output / next use | Original location |
| --- | --- | --- | --- | --- |
| A | Reference motion clip | Random state initialization selects a clip time and copies pose, velocity and phase | Initial simulated character state in C; the reference also provides the comparison standard in D | §6 Reference State Initialization, pp5–6 |
| B | Current local-frame body state including phase; optional goal; optional heightmap | Humanoid ordinary path197→1024→512→36, ReLU hidden layers, linear mean; fixed diagonal Gaussian covariance. Terrain CNN produces64D feature before concatenation | Desired joint orientations for C; training samples the Gaussian | §5.1–5.2, Fig2, Table1 |
| C | Desired joint orientations plus current local feedback | Stable PD produces joint torques; Bullet simulation includes contacts and gravity | Next state returns to B. Policy30Hz, physics1.2kHz. Transitions feed D | §5.1 and §10 |
| D | Current/reference poses, velocities, end-effector positions, COM; task objective; transitions | Four imitation terms weighted .65/.10/.15/.10. Goal-task reward .7 imitation+.3 task. ET on designated unwanted contacts. GAE advantage for PPO; TD(lambda) value target | Updates B policy parameters and separate value parameters | §5.3, §6, §10 and AppA–D |
| E | Multiple reference clips or independently trained skill policies | Three alternatives: max reward in one policy; one-hot selector in one policy; value-weighted mixture over separate policies | Single-policy skill behavior or one sampled full-cycle skill; mixture selects at cycle boundaries | §7; §10.2 |

## Arrows and notation

- Teal arrows connect state→policy→joint target→stable PD→physics and return next simulated state to B. They denote runtime information, not parameter updates.
- Orange dashed route carries simulator transitions to the trajectory batch in D. D text names the update target B and distinguishes policy theta from value psi.
- A explicitly states RSI initializes C's character, not the PD controller or policy parameters. No reference-pose arrow enters B at each step.
- The three E options are parallel. They do not form a staged pipeline or split a long reference into independently learned fragments.
- Humanoid197 includes phase; optional goal/terrain inputs enlarge the input.36 is the Gaussian mean / action parameter dimension, not number of physical DoFs.
- The diagram uses no detailed stable-PD formula. It does not equate joint targets to torques.
- The value bar in E denotes the experimental normalization to[-1,1]. Temperature0.3 and no consecutive repeated skill are explained in the article, not crowded into this overview.
- Four reward component formulas and PPO clipping are separately typeset beside the corresponding article discussion. Generated imagery supplies only illustration.

## Layout and exclusions

All main labels, weights, policy distribution, skill expressions, and causal arrows are native TeX/TikZ. The imagegen draft is unchanged and retained as a dependency. Generated explanatory text outside selected crops is excluded, especially its incorrect suggestion that the method splits long skills into fragments. No performance number comes from generated imagery. No generation label appears inside the image. The one production credit belongs beside the figure in article text.

# Fair Reinforcement Learning for Just AI

**ICLR 2026**

Currently the most powerful AI systems are aligned with human values via reinforcement learning from human feedback. Yet, reinforcement learning from human feedback models human preferences as noisy samples from a single linear ordering of shared human values and is unable to incorporate democratic AI alignment. In
particular, the standard approach fails to represent and reflect diverse and conflicting perspectives of human values. Recent research introduced the theoretically principled notion of quantile fairness for training a reinforcement learning policy
in the presence of multiple, competing sets of values from different agents. Quite recent work provided an algorithm for achieving quantile fairness in the tabular setting with explicit access to the full set of states, actions and transition probabilities
in the MDP. These current methods require solving linear programs with the size of the constraint set given by the number of states and actions, making it unclear how to translate this into practical training algorithms that can only take actions and observe individual transitions from the current state. In this paper, we design
and prove the correctness of a new algorithm for quantile fairness that makes
efficient use of standard policy optimization as a black-box without any direct
dependence on the number of states or actions. We further empirically validate our
theoretical results and demonstrate that our algorithm achieves competitive fairness
guarantees to the prior work, while being orders of magnitude more efficient with
respect to computation and the required number of samples. Our algorithm opens a
new avenue for provable fairness guarantees in any setting where standard policy
optimization is possible.



[![Conference: ICLR 2026](https://img.shields.io/badge/ICLR-2026-blue.svg)](https://openreview.net/pdf?id=XNNDODynCl)


---

## 📌 Core Contributions

* ⚖️ **Democratic Alignment:** Seamlessly incorporates multiple, competing sets of values from different agents, moving past the "one-size-fits-all" limitation of traditional RLHF.
* 📦 **Black-Box Policy Optimization:** Operates as a wrapper around *standard policy optimization* algorithms, removing direct dependency on the total number of states or actions.
* 🚀 **Orders of Magnitude Faster:** Drastically reduces sample complexity and orders of magnitude more efficient with respect to computation compared to prior tabular methods.

---

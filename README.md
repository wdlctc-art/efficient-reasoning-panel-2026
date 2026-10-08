# Efficient Reasoning Panel: Discussion Questions

Panel discussion at the [COLM 2026 Workshop on Efficient Reasoning](https://wdlctc.github.io/efficient-reasoning-2026/), Oct 9, 2026, 15:30–16:00, Hilton Union Square, San Francisco (hybrid).

The 30-minute panel centers on four core questions, open to every panelist. The additional questions are a pool to draw from as time allows.

## Core questions

### 1. Recursive self-improvement: the central question of this era

Recursive self-improvement (RSI) means an AI system that improves itself, for example by generating its own training data or automating AI research, so each version improves the next.

**Many see recursive self-improvement as the central question of this era. What does RSI mean in 2026, and is today's self-distillation or self-play already "weak RSI"? Where does efficient reasoning fit in: is cheaper reasoning the accelerator of the self-improvement loop, or is the real bottleneck elsewhere: verification, data, or taste in choosing research directions?**

### 2. What does "efficiency" mean here?

**With self-improving systems and ever-larger agent runs, how do you understand "efficiency" in reasoning? Which of the dimensions below matter most in your work, which would you prioritize, and is anything missing?**

Some dimensions people often have in mind (not exhaustive; there is no need to pick just one):

- **A. Tokens per problem:** length of the thinking trace
- **B. Latency:** time until the user gets an answer
- **C. Compute or $ per *correct* answer:** unit cost of a right answer
- **D. Memory / KV cache:** footprint of long reasoning chains
- **E. Adaptive allocation:** thinking more only when the problem needs it
- **F. Training and data efficiency:** data and RL steps needed to learn to reason
- **G. Efficiency without losing faithful reasoning:** whether shorter thinking stays readable and monitorable

Possible angle: academia mostly reports token counts, while industry pays in dollars and milliseconds. Are we optimizing the wrong metric?

### 3. Scaling agents while staying efficient

**We now know that scaling agents (more parallel attempts, longer trajectories, multi-agent search) can push toward the hardest open math problems, even the Millennium Prize Problems. That kind of scaling is enormously expensive. How do we keep reasoning efficient while scaling agents: where does the next unit of compute buy the most, and when do returns start to diminish?**

Possible angle: more agents in parallel, longer single trajectories, or better verifiers?

### 4. Knowing when to think, and measuring it

**Benchmarks today reward accuracy at any cost. Can models learn *when* to think, and how should we evaluate efficiency: accuracy per dollar, a full Pareto curve, or something else?**

Possible angle: what training data or reward signal teaches a model difficulty awareness?

## Additional questions (as time allows)

5. **Efficiency versus transparency:** As reasoning gets compressed or moves into latent space, possibly optimized by the models themselves, we may lose the ability to monitor it. Is there an inherent trade-off between efficiency and transparency, and what should be non-negotiable?
6. **Efficient reasoning for agents:** In long-horizon agentic tasks, cost accumulates across dozens of steps: context keeps growing, tool calls add latency, and early mistakes compound. What does efficient reasoning mean for a whole task rather than a single answer? When should an agent think, act, or forget? Is the bigger win in thinking less per step, or in taking fewer steps?
7. **Reasoning under tight budgets:** Under strict memory, latency and power limits, such as on a phone, what does efficient reasoning look like: thinking budgets, distillation into small models, or routing hard cases to the cloud?
8. **Agent orchestration:** In agentic systems, much of the "reasoning" is orchestration, deciding which tool to call next. Where is the waste: in thinking tokens, or in unnecessary tool calls and round-trips?
9. **Why models overthink:** Is overthinking an artifact of RL rewards, or something deeper about how transformers learn to reason?
10. **Sequential versus parallel:** Are 16 short parallel chains more or less efficient than one long chain? When does depth beat breadth?
11. **Distillation:** Is distillation a ceiling? Which reasoning abilities are lost first when you distill into a small model?
12. **Outlook:** Three years from now, will "thinking mode" still be a separate switch, or will every model adapt its compute automatically? What is the most overrated and most underrated idea in efficient reasoning today?

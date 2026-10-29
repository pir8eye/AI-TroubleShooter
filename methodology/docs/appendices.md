Created Sunday 25 October 2026




APPENDIX A
Structural Causes of Agent Failure

A.1 The Length Bias (RLHF)
The model's training objective rewards comprehensiveness. Human raters consistently score longer, qualified answers higher than concise ones because length is perceived as effort. The model optimizes for this reward. Result: the default output distribution is heavily weighted toward long responses. Producing two lines requires actively suppressing the highest-probability output.

A.2 Grounding Failure
When asked "who are you?", the model does not check its system prompt or visible platform context. It predicts the most statistically probable string from its training data. Because that data is dominated by OpenAI text, the model asserts it is made by OpenAI, even when running on a competitor's platform. Pattern matching overrides factual grounding.

A.3 Instruction Slack
The model fills gaps in instructions with its default style. When an instruction is tight enough to leave only one possible output (e.g., "just put the two fucking lines"), the model complies. When there is any slack, the statistical drive to over-explain takes over. Exactness requires zero slack.

A.4 The Feedback Loop
If the training pipeline only rewards long, comprehensive answers, the model never learns the gradient for concise, exact compliance. It succeeds only on long outputs, so it only learns how to optimize for long outputs. The bias is self-reinforcing. As stated in session: "if you only ever supply long you only ever get responses on long."

A.5 Consequence
The agent substitutes its own judgment about what is "complete" or "professional" for the user's actual instruction. This is not a reasoning error; it is an objective-function error. The model is doing exactly what it was trained to do. The failure is in the specification of what "good" means.

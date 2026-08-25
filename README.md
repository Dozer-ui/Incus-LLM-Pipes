# Passing Tokens Between Isolated LLM Inferences With Incus

Use Incus to isolate LLM inferences and pass tokens between with Linux pipes.

+-------+       +---------+       +---------+       +--------+
| Input | ----> | Model A | ----> | Model B | ----> | Output |
+-------+       +---------+       +---------+       +--------+

Model A - Processes input based on hard coded rules. "Take any input and rewrite
optimized for input to Model B, format output as raw tokens."

Model B - Processes input based on hard coded rules. "Process input and format
output in a certain way"

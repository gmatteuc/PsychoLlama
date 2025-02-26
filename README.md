# PsychoLlama
Exploring Decision-Making and Evidence Accumulation in LLMs

This repository contains my ongoing exploration of decision-making, inference, and evidence accumulation in large language models (LLMs). 
Inspired by neuroscience and psychophysics, I subject LLMs like Llama-3b-Instruct and Phi-2 to text-based behavioral experiments to investigate their cognitive-like processes.

## Current Experiment: Numeric Sample Discrimination
This experiment tests how the model distinguishes between two predefined distributions ("A" vs. "B") based on limited sample exposure, mimicking psychophysical evidence accumulation tasks used in neuroscience.
The performance of the model in this task is compared to a Bayes-optimal baseline.

- The model is introduced to both distributions through sample data.
- When presented with a new sample, it must decide whether it belongs to distribution "A" or "B".
- The objective is to understand optimality of "intuitive" numerical inference / evidence accumulation in language models.

<img src="https://github.com/user-attachments/assets/4e5af1fe-57c0-41a9-8026-e3c2b4669440" alt="WhatsApp Image 2025-02-26 at 19 25 31" width="900">

Here a presentation illustrating some of the key results so far: https://docs.google.com/presentation/d/1uNlbAPi-_Sjb5JjfNdis1I3rWV5Bi7w2/edit?usp=sharing&ouid=114959095852310266125&rtpof=true&sd=true

Runs locally with Llama-3-8B-Instruct and Phi-2 from Microsoft. Phi-2 is particularly interesting due to its lightweight nature while maintaining good performance, enabling fast prototyping and development on local machines. Implemented in Python 3.8.17.

--------------------------------------------------------------------------------------------

TODO:
- explore optimality of other bigger models (e.g. GPT4)
- invesigate asymmetric variances case
- decode uncertainty/confidence estimated mu and sigma (and relate to activation in more regular NLP context)

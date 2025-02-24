# PsychoLlama
Exploring Decision-Making and Evidence Accumulation in LLMs

This repository contains my ongoing exploration of decision-making, rationality, and evidence accumulation in large language models (LLMs). Inspired by neuroscience and psychophysics, I subject Llama-3b-Instruct to text-based behavioral experiments to investigate its cognitive-like processes.

## Current Experiment: Numeric Sample Discrimination
This experiment tests how the model distinguishes between two predefined distributions ("A" vs. "B") based on limited sample exposure, mimicking psychophysical evidence accumulation tasks used in neuroscience.
The model is introduced to both distributions through sample data.
When presented with a new sample, it must decide whether it belongs to A or B or request more samples by responding "Next" (introducing a speed-accuracy trade-off).
The objective is to analyze decision bias, rationality, and sensitivity to uncertainty.

Runs locally with Llama-3-8B-Instruct on NVIDIA RTX 2000 (Ada Gen) with 4-bit quantization. Implemented in Python 3.8.17.

--------------------------------------------------------------------------------------------

TODO:
- continue exploring and run longer to sample better
- compare with reference bayesian model
- exploit properly the "next" option
- try to decode uncertainty/confidence pressure-to-perform from MLP and relate to same variables in natural language tasks

# FGSM Adversarial Attack & Defence

Implementation of the Fast Gradient Sign Method (FGSM) adversarial 
attack against a PyTorch neural network, with two defensive 
countermeasures evaluated and compared.

## What this project covers
- Building a neural network classifier in PyTorch
- Implementing FGSM from scratch (Goodfellow et al. 2014)
- Demonstrating accuracy collapse under increasing attack strength
- Implementing adversarial training as a primary defence
- Implementing input smoothing as a secondary defence
- Evaluating the accuracy-robustness tradeoff
- Analysing defence interaction effects

## Key findings
- At epsilon 0.5, undefended model drops from 100% to 46.67%
- Adversarial training recovers accuracy to 66.67% at epsilon 0.5
- Combining defences doesn't always improve results — overlapping 
  defences can interfere with each other
- Effective defence requires complementary layers, not duplicate ones

## MITRE ATLAS mapping
- AML.T0015 — Evade ML Model (attack implemented)
- AML.M0003 — Adversarial Training (defence implemented)
- AML.M0002 — Input Smoothing (defence implemented)

## Tools used
Python, PyTorch, scikit-learn, numpy

## Background
Third project in a structured learning path into AI/ML security.
Builds on manual adversarial attack techniques from previous projects
with a systematic, gradient-based attack method.

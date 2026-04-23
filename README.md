# HTGM v2 Hindi LLM – Session 17 | 150 Hours Training Progress

## Overview

Session 17 of HTGM v2 Hindi LLM training is now completed.

This session focused on stable checkpoint continuation, strong validation stability, and pushing the model beyond the important 38K+ optimizer steps milestone.

After 150+ total training hours, the model is showing better consistency, controlled validation loss, stable perplexity, and stronger long-session reliability.

This repository documents the real progress of building a Hindi LLM from scratch using a GPT-style Transformer architecture.

---

## Session Information

- Session Number: 17
- Total Training Time: 150+ Hours
- Total Sessions Completed: 17
- Major Milestone: 38K+ Optimizer Steps Crossed

---

## Technical Details

- Model Name: HTGM v2
- Type: Hindi Large Language Model (Hindi LLM)
- Architecture: GPT-style Transformer
- Model Size: 163.4M Parameters
- Sequence Length: 2048
- Vocabulary Size: 100,000
- Dataset Size: ~41GB
- Dataset Source: AI4Bharat Sangrah + Manual Cleaning
- Training Platform: Kaggle
- GPU: 2x T4
- Tokenizer: Hugging Face BPE-based Tokenizer

---

## Training Progress

- Total Planned Optimizer Steps: 923,382
- Resumed From Checkpoint Step: 1,202,522
- Current Training Step: 38,864+
- Mid Checkpoint Saved: ckpt_s38000.pt
- Final Checkpoint Saved: ckpt_final_s1243671.pt

---

## Dataset Used

### Loaded Chunks

- chunk_1.txt
- chunk_2.txt
- chunk_3.txt

---

## Training Metrics

### Core Metrics

- Training Loss: 3.7985
- Earlier Observed Loss: 4.1905
- Final Validation Loss: 4.9265
- Final Validation Perplexity (PPL): 137.90
- Training Perplexity: 44.63

### Optimization Metrics

- Learning Rate: 3.85e-05
- Gradient Global Norm: 0.3054
- Tokens Per Second: ~2914

---

## Checkpoint Strategy

Training resumed from a previous checkpoint instead of restarting from scratch.

### Benefits

- Safe long training workflow
- Stable continuation across sessions
- Hyperparameter testing without losing progress
- Reliable optimizer and scheduler recovery

This makes long Hindi LLM experiments practical and efficient.

---

## Observations

### What Improved

- Validation remains stable near 4.92
- Perplexity stays controlled near 137
- Training loss improved to 3.79
- Gradient norm remains stable
- GPU performance stayed strong
- No major crashes
- W&B monitoring active
- Smooth checkpoint saving

### Why It Matters

Crossing 38K+ steps is important, but maintaining validation quality matters even more.

This session proves that better optimization is more valuable than simply training longer.

---

## Current Status

- Training is stable
- Validation remains strong
- Model learning quality is improving
- Long-session reliability is strong

Still not production-ready, but the foundation is becoming much stronger.

---

## Next Steps

- Apply Supervised Fine-Tuning (SFT)
- Improve instruction-following capability
- Better dataset structuring
- Continue longer training sessions
- Improve response quality and coherence

---

## Author

Mahesh Editor  
India AI Official

---

## Build in Public

This project is shared publicly to document real AI development, not just final results.

Every checkpoint, problem, fix, and improvement is part of the journey.

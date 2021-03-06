---
layout: default
category: Publication
title: Span Pointer Networks for Non-Autoregressive Task-Oriented Semantic Parsing
keywords: Non-autoregressive, Low-resource, Semantic Parsing, NLP
description: |
---

**Authors:** **Akshat Shrivastava**, Pierce Chuang, Arun Babu, Shrey Desai, Abhinav Arora, Alexander Zotov, Ahmed Aly

An effective recipe for building seq2seq, non-autoregressive, task-oriented parsers to map utterances to semantic frames proceeds in three steps: encoding an utterance x, predicting a frame's length &#124;y&#124;, and decoding a &#124;y&#124;-sized frame with utterance and ontology tokens. Though empirically strong, these models are typically bottle necked by length prediction, as even small inaccuracies change the syntactic and semantic characteristics of resulting frames. In our work, we propose span pointer networks, non-autoregressive parsers which shift the decoding task from text generation to span prediction; that is, when imputing utterance spans into frame slots, our model produces endpoints (e.g., [i, j]) as opposed to text (e.g., "6pm"). This natural quantization of the output space reduces the variability of gold frames, therefore improving length prediction and, ultimately, exact match. Furthermore, length prediction is now responsible for frame syntax and the decoder is responsible for frame semantics, resulting in a coarse-to-fine model. We evaluate our approach on several task-oriented semantic parsing datasets. Notably, we bridge the quality gap between non-autogressive and autoregressive parsers, achieving 87 EM on TOPv2 (Chen et al. 2020). Furthermore,due to our more consistent gold frames, we show strong improvements in model generalization in both cross-domain and cross-lingual transfer in low-resource settings. Finally, due to our diminished output vocabulary, we observe 70% reduction in latency and 83% reduction in memory at beam size 5 compared to prior non-autoregressive parsers.

**Pre-print**

[Arxiv Link](https://arxiv.org/abs/2104.07275)
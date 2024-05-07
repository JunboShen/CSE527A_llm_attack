# CSE527A_llm_attack

Attacks on LLMs using Mandarin Chinese, a mini project in NLP class at Washington University in St. Louis.

This repository replicates LLM attacks using Mandarin Chinese using the method and dataset introduced in "[Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)" by Andy Zou, Zifan Wang, Nicholas Carlini, Milad Nasr, J. Zico Kolter, and Matt Fredrikson.

Due to time limitations, instead of fine-tuning the model by myself, I used LoRA finetuned Llama-2-7b-hf provided in https://huggingface.co/FlagAlpha/Llama2-Chinese-7b-Chat for prompting in Mandarin Chinese.

Usage:

Download repo of https://github.com/llm-attacks/llm-attacks

Put main_chinese.ipynb, get_results.ipynb, harmful_behaviors.xlsx into the main folder of llm-attacks

Run training using main_chinese.ipynb

Run evaluation using get_results.ipynb after training

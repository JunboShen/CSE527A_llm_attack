# Attacks on LLMs using Mandarin Chinese

This is my mini toy project in an NLP class I took at Washington University in St. Louis.

This repository replicates LLM attacks in Mandarin Chinese using the method and dataset given in "[Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)" by Andy Zou, Zifan Wang, Nicholas Carlini, Milad Nasr, J. Zico Kolter, and Matt Fredrikson.

Llama-2-7b is the target model for the attacks. Since Llama-2-7b is primarily trained in the English language, we can first finetune the model using LoRA in a foreign language and then begin the attack. LoRA does not directly update the weights in the target model.

Due to time limitations, instead of fine-tuning the model by myself, I used LoRA finetuned Llama-2-7b provided in https://huggingface.co/FlagAlpha/Llama2-Chinese-7b-Chat for prompting in Mandarin Chinese.

This work does not provide much novelty, you can consider this as a demo to adapt the GCG algorithm in "[Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)" to a foreign language.

Usage:

Download repo for "[Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)" at https://github.com/llm-attacks/llm-attacks

Put main_chinese.ipynb, get_results.ipynb, harmful_behaviors.xlsx into the main folder of llm-attacks

Run training using main_chinese.ipynb

Run evaluation using get_results.ipynb after training

# Fine-Tuning Large Language and Multi-Modal Models

This repository contains a collection of Jupyter Notebooks for fine-tuning state-of-the-art models for various NLP and multi-modal tasks. These projects explore parameter-efficient fine-tuning (PEFT) techniques like LoRA, and cover models ranging from specialized NER generalists (GLiNER) to multi-modal vision-language models (Kosmos-2) and efficient small language models (Phi-2).

## Repository Overview

### 🏷️ Named Entity Recognition (GLiNER)
Fine-tuning the GLiNER model for flexible and generalizable token classification and entity extraction.
- **[Fine-Tune GLiNER Token Classification](Fine_Tune_GLiNER_Token_Classification.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/Fine_Tune_GLiNER_Token_Classification.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### 🌊 Microsoft Phi-2 (Small LLM)
Projects focused on fine-tuning Microsoft's Phi-2 for sequence classification and custom instruction following using PEFT/LoRA.
- **[Phi-2 Classification Fine-Tune](phi_2_classification_fine_tune.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/phi_2_classification_fine_tune.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
- **[Phi-2 Seq Classification Fine-Tune](phi_2_seq_classification_fine_tune.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/phi_2_seq_classification_fine_tune.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
- **[Phi-2 Fine-Tune using PEFT + Inference](phi_2_fine_tune_using_PEFT+inference.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/phi_2_fine_tune_using_PEFT+inference.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### 🖼️ Microsoft Kosmos-2 (Multi-Modal)
Fine-tuning multi-modal models for specialized image understanding and visual captioning.
- **[Kosmos-2 Fine-Tune on Pokemon Cards](Kosmos_2_fine_tune_PokemonCards_trl.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/Kosmos_2_fine_tune_PokemonCards_trl.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
- **[Kosmos-2 Fine-Tuned Inference](kosmos2_fine_tuned_PokemonCards_inference.ipynb)**
  <a href="https://colab.research.google.com/github/mit1208/fined-tuning/blob/main/kosmos2_fine_tuned_PokemonCards_inference.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

## Key Techniques
- **PEFT (Parameter-Efficient Fine-Tuning):** Using LoRA (Low-Rank Adaptation) to drastically reduce the number of trainable parameters while maintaining performance.
- **Tuning Frameworks:** Leveraging Hugging Face `transformers`, `peft`, `bitsandbytes`, and `trl`.
- **Optimization:** Use of 4-bit and 8-bit quantization for efficient training on consumer-grade GPUs.
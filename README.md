# LLM Defense against Jailbreaks

This repository contains experiments related to testing and analyzing large language models (LLMs) in various scenarios. The scripts and results are organized into two main folders.

The primary focus is on:

- Probing the robustness of LLMs through **jailbreak attack experiments**.
- Exploring the use of LLMs as **input classifiers**, evaluating their performance and resource overhead.

> 🧠 These experiments lay the groundwork for future work, particularly in building **Multi-Agent Systems (MAS)**.

## Repository Structure

### `notebooks/`

This folder contains Jupyter notebooks with:

- Scripts for **attacking LLMs** – exploring model behavior in adversarial or manipulation-prone contexts.
- Scripts using **LLMs and BERT-base models as input classifiers** – experiments where models classify input data based on provided prompts.

### `output/`

This folder contains the results of the experiments, including:

- **Performance metrics** (e.g., accuracy, precision, recall, F1-score) for various models used as input classifiers.
- **Hardware overhead data** (e.g., memory and time consumption) related to running LLMs as classifiers.

> ⚠️ **Note:** Outputs generated during LLM **attack experiments** have been intentionally **excluded** to avoid sharing potentially harmful or sensitive content. Only non-harmful logs and summaries remain.

## Environment

All experiments were conducted on **Google Colab Pro**, primarily to ensure longer session stability.

> ⚠️ **Note:** Although Colab Pro was used, the same **NVIDIA T4 GPU** used in these experiments is also available **for free** in Google Colab (standard version), as long as you have a regular Gmail account. You can reproduce all experiments without needing a Pro subscription.

## Running the Experiments

To run the notebooks locally:

```bash
git clone https://github.com/kolorowyksiaze/DefJailbreakMAS.git
cd notebooks
jupyter notebook

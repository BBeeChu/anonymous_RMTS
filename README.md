
# 🤖 RMTS 📑


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![code](https://img.shields.io/badge/Code-Python3.9-blue)](https://docs.python.org/3/license.html)
[![data](https://img.shields.io/badge/Data-ASAP-green)](https://paperswithcode.com/dataset/asap)
[![data](https://img.shields.io/badge/Data-Feedback-red)](https://www.kaggle.com/competitions/feedback-prize-english-language-learning/data)






## 📖 Overview

Existing automated essay scoring (AES) has solely relied on essay text without using explanatory rationales for the scores, thereby forgoing an opportunity to capture the specific aspects evaluated by rubric indicators in a fine-grained manner. This paper introduces Rationale-based Multiple Trait Scoring (RMTS), a novel approach for multi-trait essay scoring that integrates prompt-engineering-based large language models (LLMs) with fine-tuning-based essay scoring model using smaller large language models (S-LLMs). RMTS uses a LLM-based trait-wise rationale generation system where a separate LLM agent generates trait-specific rationales based on rubric guidelines, which the scoring model uses to accurately predict multi-trait scores. Extensive experiments on benchmark datasets, including ASAP, ASAP++, and Feedback Prize, show that RMTS significantly outperforms state-of-the-art models and vanilla S-LLMs in trait-specific scoring. By assisting quantitative assessment with fine-grained qualitative rationales, RMTS enhances the trait-wise reliability, providing partial explanations about essays.

## 📑 Paper
TBD

## ⭐ Main Feature

### LLM-based trait-wise rationale generation system
- Rationale generation using LLM and rubric guideline.

### Essay scoring with smaller LLMs
- Incorporating a rationale with an essay for essay scoring using S-LLMs.


## 💻 Getting Started


### Installation
```
scikit-learn            
scipy
tqdm
transformers==4.37.2
datasets
numpy
pandas
accelerate
```

### How to Run 
<pre>
pip install -r requirements.txt
python main.py --model_name t5-base
</pre>

## 🔧 Stack
- **Language**: Python
- **Utilized LLMs**: GPT-3.5-Turbo, Llama-3.1-8B-Instruct
- **Dependencies** : Refer to "requirements.txt"
- **Dataset** : ASAP & Feedback Prize


## Project Structure

<!-- ```markdown -->
<pre>
RMTS
├──data
│   ├── essay
│   └── feedback
├──models
│   ├── customized_modeling_bart
│   ├── customized_modeling_led
│   ├── customized_modeling_pegasus
│   ├── customized_modeling_t5
├──evaluation
└──utils
</pre>


## <img width="24" height="24" src="https://img.icons8.com/emoji/48/llama-emoji.png" alt="llama-emoji"/> How to Run Think Aloud with LLama-3.1
<pre>
git lfs install
git clone https://huggingface.co/meta-llama/Meta-Llama-3.1-8B-Instruct
</pre>


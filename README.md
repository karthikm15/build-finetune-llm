# build-finetune-llm
This repository aims to showcase our work in pretraining and finetuning an attention-based transformer architecture on question answering (QA) and summarization. The file directory is organized as follows:
```
build-finetune-llm
└─── checkpoints
│   │   baseline_model_weights.pth
|   |   finetune_qa_model_weights.pth
|   |   finetune_summarization_model_weights.pth
└─── notebooks
    |   finetuning_qa.ipynb
    │   finetuning_summarization.ipynb
    │   pretraining.ipynb
|____ images
    |   Deep Learning Architecture.png
```

---

## File Directory Contents

`baseline_model_weights.pth`: Checkpointed model weights from pretraining. This model received a 3.4 validation loss after twenty epochs of training. The model architecture is as follows: ![model architecture](https://github.com/karthikm15/build-finetune-llm/blob/main/images/Deep%20Learning%20Architecture.png)

`finetune_qa_model_weights.pth`: Checkpointed model weights for question answering.

`finetune_summarization_model_weights.pth`: Checkpointed model weights for summarization.

`finetuning_qa.ipynb`: Notebook for finetuning model on question answering on Stanford QA data.

`finetuning_summarization.ipynb`: Notebook for finetuning model on summarization on CNN Daily Mail data.

`pretraining.ipynb`: Notebook for training attention-based transformer model on OpenWebText data.

## How to Run Code

For running either or pretrained or finetuned model checkpoints, load the checkpoints from the `checkpoints` folder. The Jupyter notebooks contain the relevant code for recreating the transformer architecture from scratch. Here are the datasets that were used:
* **OpenWebText Dataset:** https://openwebtext2.readthedocs.io/en/latest/
* **SquadQA Dataset:** https://huggingface.co/datasets/squad
* **CNN DailyMail Dataset:** https://huggingface.co/datasets/cnn_dailymail

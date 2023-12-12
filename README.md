# build-finetune-llm
This repository aims to showcase our work in pretraining and finetuning an attention-based transformer architecture on question answering (QA) and summarization. The file directory is organized as follows:
```
build-finetune-llm
└─── checkpoints
│   │   baseline_model_weights.pth 
└─── notebooks
    |   finetuning_qa.ipynb
    │   finetuning_summarization.ipynb
    │   pretraining.ipynb
|____ images
    |   Deep Learning Architecture.png
```

---

## File Directory Contents

`baseline_model_weights.pth`: Checkpointed model weights from pretraining. This model received a 3.4 validation loss after twenty epochs of training. The model architecture is as follows: ![model architecture](images.png)

`finetuning_qa.ipynb`: Notebook for finetuning pretrained model on question answering for the Stanford QA dataset.

`finetuning_summarization.ipynb`: Notebook for finetuning pretrained model on summarization on the CNN Daily Mail dataset.

`pretraining.ipynb`: Notebook for training attention-based transformer model on the OpenWebText dataset.

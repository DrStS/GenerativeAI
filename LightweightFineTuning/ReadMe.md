Project: Apply Lightweight Fine-Tuning to a Foundation Model
Prepare the Foundation Model
Criteria	Submission Requirements
Load a pretrained HF model

Includes the relevant imports and loads a pretrained Hugging Face model that can be used for sequence classification

Load and preprocess a dataset

Includes the relevant imports and loads a Hugging Face dataset that can be used for sequence classification. Then includes relevant imports and loads a Hugging Face tokenizer that can be used to prepare the dataset.

A subset of the full dataset may be used to reduce computational resources needed.

Evaluate the pretrained model

At least one classification metric is calculated using the dataset and pretrained model

Perform Lightweight Fine-Tuning
Criteria	Submission Requirements
Create a PEFT model

Includes the relevant imports, initializes a Hugging Face PEFT config, and creates a PEFT model using that config

Train the PEFT model

The model is trained for at least one epoch using the PEFT model and dataset

Save the PEFT model

Fine-tuned parameters are saved to a separate directory. The saved weights directory should be in the same home directory as the notebook file.

Perform Inference Using the Fine-Tuned Model
Criteria	Submission Requirements
Load the saved PEFT model

Includes the relevant imports then loads the saved PEFT model

Evaluate the fine-tuned model

Repeats the earlier evaluation process (same metric(s) and dataset) to compare the fine-tuned version to the original version of the model

Suggestions to Make Your Project Stand Out
Try using the bitsandbytes package (installed in the workspace) to combine quantization and LoRA. This is also known as QLoRA
Try training the model using different PEFT configurations and compare the results
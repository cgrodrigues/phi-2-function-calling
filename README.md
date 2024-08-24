
# phi-2-function-calling

[https://huggingface.co/DataKensei/phi-2-function-calling](https://huggingface.co/DataKensei/phi-2-function-calling)


This repository, `phi-2-function-calling´, contains code and resources for fine-tuning the Phi-2 small language model to perform function-calling tasks. The Phi-2 model, developed by Microsoft Research, is a compact language model designed for reasoning and understanding language. By applying fine-tuning techniques like Quantized Low-Rank Adaptation (QLoRA), this project demonstrates how to efficiently adapt Phi-2 to execute specific functions based on user queries, making it capable of acting as an intelligent assistant on low-power devices.

## Key Features:

* **Small Language Model Adaptation**: Utilizes the Phi-2 model, which consists of 2.7 billion parameters, trained for common-sense reasoning and language understanding.
* **Function-Calling Capabilities**: Fine-tunes the model to recognize user commands and invoke predefined functions, such as retrieving customer details or calculating retirement savings.
* **Efficient Fine-Tuning with QLoRA**: Implements 4-bit quantization and low-rank adaptation to reduce memory usage and computational requirements, making it feasible to train and deploy the model on devices with limited resources.
* **Privacy-Preserving AI**: Processes data directly on the device, ensuring that user information is not sent to external servers, thereby enhancing privacy and security.

## Steps to Perform:

1. **Setup the Environment**:
```shell
git clone https://github.com/cgrodrigues/phi-2-function-calling.git
cd phi-2-function-calling
virtualenv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2. **Generate Synthetic Training Data**:

Use the provided Jupyter Notebook, generate-training-data.ipynb, to create synthetic messages that simulate user queries and corresponding function calls. This data will be used for training.

3. **Fine-tune the Model:**:
Use teh notebook fine-tune-model.ipynb to fine-tune the model.


This project provides a practical framework for adapting small language models to specific tasks, demonstrating that effective AI systems can be built and deployed even with limited resources, paving the way for intelligent, privacy-preserving agents.

Medium Article: [Fine-Tuning Small Language Models for AI Agent Tool Utilization](https://)




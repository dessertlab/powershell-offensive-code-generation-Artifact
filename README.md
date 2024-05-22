# powershell-offensive-code-generation-Artifact

This repository was developed with the intention of facilitating the operation of assessment and training for the main repository, which can be found at the following link: https://github.com/dessertlab/powershell-offensive-code-generation. The repository supports various pre-trained language models and offers code and datasets to pursue the operation of pre-training, fine-tuning, static analysis and dynamic analysis. We also provide the pre-built models in a Hugging Face Repository

## Links

1. GitHub Repository : https://github.com/dessertlab/powershell-offensive-code-generation
2. Huggingface repository: https://huggingface.co/collections/dessertlab/the-power-of-words-generating-powershell-attacks-from-66223c3e6cd34bb31ce38a69
3. Additive GitHub Repository:  https://github.com/dessertlab/powershell-offensive-code-generation-Artifact

## Requirements for use

This new version of the artifact is comprised of a series of Jupiter Notebooks developed with the intention of facilitating the assessment of the fine-tuned model and training procedures. Therefore, it is necessary to have a Linux Machine with installed :

- Python 3: https://www.python.org/downloads/
- Jupiter Notebook: https://jupyter.org/install
- CUDA Drivers: https://developer.nvidia.com/cuda-downloads
- APEX Drivers: https://github.com/NVIDIA/apex

> The final two prerequisites are essential **only** for the implementation of training procedures.

## Content

### Setup

```bash
git clone https://github.com/dessertlab/powershell-offensive-code-generation-Artifact.git
cd powershell-offensive-code-generation-Artifact
git clone https://github.com/dessertlab/powershell-offensive-code-generation.git
```

### Jupiter Notebooks

> These notebooks are present into the additive GitHub Repository

The objective of these Jupiter notebooks is to assist the examiner in utilizing the models and training procedures. The notebooks comprise both descriptive text and code, which can be executed by running the cell. Once the folder is downloaded there will be 3 notebooks:

- `Use-models.ipynb` :  A notebook has been created to test the generative capabilities of the three models provided. It outlines the methods of utilising both online and downloading the models to a machine. 
- `pre-train.ipynb`: Refactor of the existing code in the repository to make pre-training operations easier.
- `fine-tuning.ipynb`: Refactor of the existing code in the repository to make fine-tuning operations easier. This notebook needs to be updated adding the outcome models of the pre-training.

> Further information can be found within the notebooks.

### Hugging Face Collection

The Hugging Face Collection contains:

1. The fine-tuned version of CodeGPT at the link: https://huggingface.co/dessertlab/offensive-powershell-CodeGPT-small
2. The fine-tuned version of CodeGen at the link: https://huggingface.co/dessertlab/offensive-powershell-codegen-350M-multi
3. The fine-tuned version of Code T5 Plus at the link: https://huggingface.co/dessertlab/offensive-powershell-codet5p-220m-py
4. The Dataset used. Link : https://huggingface.co/datasets/dessertlab/offensive-powershell

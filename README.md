# Text Extraction from Documents

This repo demonstrates sample environment creation for Docling framework. 
* Python 3.10
* docling v2.2.0 (https://huggingface.co/ds4sd/docling-models/tree/v2.2.0)
* uv (Python packages and virtual environment management)

<br>

## 1. Base Setting
### 1.1. Install `uv`
    pip install pip

### 1.2. Create a virtual environment with specific Python version
    uv venv --python 3.10 .venv

### 1.3. Update `pip`
    uv pip install --upgrade pip

### 1.4. Install all packages from `requirments.txt`
    uv pip install -r requiremnts.txt

<br>

## 2. Clone `Docling` repository
### 2.1. Clone HF repository (except large files)
    cd configs
    git clone https://huggingface.co/ds4sd/docling-models --branch v2.2.0

### 2.2. Download and replace the large files from HF (**BRANCH MUST BE v2.2.0**)
* model.safetensors

    https://huggingface.co/ds4sd/docling-models/tree/v2.2.0/model_artifacts/layout

* tableformer_accurate.safetensors

    https://huggingface.co/ds4sd/docling-models/tree/v2.2.0/model_artifacts/tableformer/accurate
  
* tableformer_fast.safetensors

    https://huggingface.co/ds4sd/docling-models/tree/v2.2.0/model_artifacts/tableformer/fast

### 2.3. Replace the files (**Keep the folder structure**).

### 2.4. Create `EacyOcr` folder under `docling-models` folder

### 2.5. Download required files for EasyOCR

* craft_mlt_25k.pth

    https://huggingface.co/xiaoyao9184/easyocr/blob/master/craft_mlt_25k.pth

* latin_g2.pth

    https://huggingface.co/xiaoyao9184/easyocr/blob/master/latin_g2.pth

* english_g2.pth

    https://huggingface.co/xiaoyao9184/easyocr/blob/master/english_g2.pth

### 2.6. Save the files in the newly created `EasyOcr` folder.


##
Test file is in `test.ipynb` under `notebooks` folder!!





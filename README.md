# immunoduct
Pipeline for tumor immunology. Input should be GCT files made by `riboduct`.

## Installation
### 1. Install conda
`immunoduct` requires `conda` package manager. To install `conda` for Linux,
```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
echo ". ${HOME}/miniconda3/etc/profile.d/conda.sh" >> ~/.bashrc
source ~/.bashrc
```

### 2. Install pipeline
Download and install `immunoduct`.
```
git clone https://github.com/msfuji/immunoduct.git
cd immunoduct
conda activate
bash immunoduct.sh install
conda deactivate
```

## Usage
Make a local copy of pipeline for each project.
```
git clone https://github.com/msfuji/immunoduct.git
cd immunoduct
```
Modify `config.yaml`. Start running the pipeline.
```
conda activate immunoduct
bash immunoduct.sh run config.yaml
conda deactivate
```

# rag-system-FFD4


This is a minimal implementation of the RAG model for question answering 

## Requirements 
- Python 3.8 or later

#### Install Python using MiniConda 
1) Download and install MiniConda from [here] (https://docs.anaconda.com/miniconda/#quick-command-line-install)

2) Create a new environment using the following command:
``` bash 
$ conda create -n rag-system-FFD4 python
```
3) Activate the environment:
``` bash 
$ conda activate /home/hager/miniconda3/envs/rag-system-FFD4
```
### (Optional) Setup command line for better readability
``` bash 
export PS1="\[\033[01;32m\]\u@\h:\w\n\[\033[00m\]\$ "
```

## Installation

### Install the required packages 

``` bash 
pip install --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org -r requirements.txt
```
### Setup the environment variables
``` bash 
$ cp .env.example .env 
```

Set your environment variables in the `.env` file. Like `OPENAI_API_KEY` value.

## Run the FastAPI server
``` bash 
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000
```


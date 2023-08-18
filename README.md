# CAMS
## An Annotated Corpus for Causal Analysis of Mental Health Issues in Social Media Posts

This repository is created to support the paper ['CAMS: An Annotated Corpus for Causal Analysis of Mental health on Social media'](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.686.pdf) (accepted (published) in Language Resources and Evaluation Conference LREC'2022) 

We introduce a new dataset for Causal Analysis of Mental health illness in Social media posts (CAMS). We first introduce the annotation schema for this task of causal analysis. The causal analysis comprises two types of annotations, viz, causal interpretation and causal categorization. We show the efficacy of our scheme in two ways: (i) crawling and annotating 3155 Reddit data and (ii) re-annotate the publicly available SDCNL dataset of 1896 instances for interpretable causal analysis. We further combine them as CAMS dataset.

## Dataset Overview

The labeled data could be downloaded from [here](https://github.com/CMOONCS/CAMS/tree/main/data).

## Terms of use
- This corpus can be used freely for research purposes.
- The [paper ](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.686.pdf) provides details of the creation and use of the corpus. 
- If you use the corpus, then please cite the paper.
- Please feel free to send us an email:
  - with feedback regarding the corpus.
  - with information on how you have used the corpus.
  - if interested in a collaborative research project.

### Steps to run on WSL (Ubuntu 20.04)
- Add “deadsnakes” PPA to Your Machine
  ```bash
  sudo add-apt-repository ppa:deadsnakes/ppa
  ```

- Install Python 3.8 via “apt”
  ```bash
  sudo apt install python3.8 -y
  ```

- Install pip for Python 3
  ```bash
  sudo apt update
  sudo apt install python3-pip
  ```

- Install ipython for Python 3
  ```bash
  sudo apt install ipython3
  ```

- Install Jupyter
  ```bash
  pip3 install jupyter
  ```

- Create alias to launch jupyter without browser from the WSL:
  - Open your bash configuration: ```vim ~/.bashrc ```
  - Add to the end of the file and save/exit:
  ``` alias jupyter-notebook="~/.local/bin/jupyter-notebook --no-browser" ```

Now you can run a jupyter server ``` jupyter-notebook ``` and access the service with your browser from Windows ``` localhost:8888 ```.

### Steps to run on Github Codespaces
- You must install Python v3.8 and pip (as described in devcontainer.json)
- Instal python dependences
  ```bash
  pip install -r requirements.txt
  ```
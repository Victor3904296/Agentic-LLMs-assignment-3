# Agentic-LLMs-assignment-3

To reproduce our results, follow the steps listed in this README file.

## Installation
Start with creating a virtual environment and install the given requirements.

````bash
python -m venv .venv
.venv\bin\activate
pip install -r requirements.txt
````

## Executor models
The executor classifier models have already been trained and are in the submission. They can be found in the model folder. However, if you would like to train them again before running the simulation (optional), then they can be trained using the following command:

```bash
python 0_train_models.py
```


## API key
To successfully run this experiment, make sure you have an OpenRouter API key,
in order to gain access to the Claude Haiku 5.5 model.

## Run experiment

To run this experiment, run `2_llm_mcp.py` it will ask for your personal API 
key, after which the script will be run. 

```bash
python 2_llm_mcp.py
```

The results will be stored in the `.\results\` folder, including:
* Confusion matrix plots for each disease executor (`confusion_*_llm.png`)
* Overall performance graph (`output.png`)
* Classification metrics of triage process (`triage_report_*.csv`)
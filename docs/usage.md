
# 📖 How to Use Deep Civics

## Step 1: Install

```bash
pip install deepcivics

```

Or clone the repo:


```bash
git clone https://github.com/YOUR_USERNAME/deepcivics.git
cd deepcivics
pip install -e .

```

## Step 2: Generate a config
```bash
from deepcivics import generate_config_from_url

generate_config_from_url(
    csv_url="https://data.cdc.gov/api/views/bi63-dtpu/rows.csv",
    country="USA"
)
```

## Step 3: Ask Questions

```bash
from deepcivics import CivicLLM
from deepcivics.config import load_config

cfg = load_config()
llm = CivicLLM(cfg['model'])
answer = llm.ask("Which states have the highest death count?", context)
```


## Step 4: Visualize 

```bash
from deepcivics import visualization, civic_action

visualization.plot_bar_count(df, cfg["columns_of_interest"][0])
print(civic_action.generate_email(question, answer, "CDC"))
```

## Required Fields:

source: public CSV/JSON URL

columns_of_interest: must match actual column names

model: can be alias or full Hugging Face name




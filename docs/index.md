---
layout: default
title: Deep Civics
---

# 🌍 Deep Civics

**Deep Civics** is a multilingual, civic intelligence toolkit for exploring public data from government (.gov), open-data, and institutional sources. It allows anyone — citizens , policymakers, educators, journalists, and investors — to **fetch, analyze, question, and visualize real public datasets** in just a few steps.

---

## 🚀 What Can You Do With Deep Civics?

- ✅ Import any `.csv` from a government or open-data site (URL or local)
- ✅ Generate a config file automatically from the data
- ✅ Ask questions in any language using LLMs (e.g., “What trends are visible in rural health?”)
- ✅ Get answers + summaries from Hugging Face transformers
- ✅ Visualize key columns with 1-line charting
- ✅ Export insights for social media or policy communication
- ✅ Run entirely in the browser using Jupyter + Binder

---

## ⚙️ Core Methods & Modules

| Module | Description |
|--------|-------------|
| `generate_config_from_url(url, country)` | Generate a `deepcivics.yaml` from any `.csv` URL |
| `load_config(path='deepcivics.yaml')` | Load YAML configuration into a dictionary |
| `fetch_csv(path_or_url)` | Load CSV data from local file or web |
| `CivicLLM(model_name)` | Wrapper around Hugging Face's `pipeline()` for Q&A |
| `ask(question, context)` | Ask a model a question on tabular data as text |
| `plot_bar_count(df, column)` | Plot frequency/count bar charts from CSV columns |


---

## 🧱 Architecture Overview

📊 CSV Dataset (.gov / World Bank / OpenData)
↓
🛠️ generate_config_from_url() → 📝 YAML Config (deepcivics.yaml)
↓
🔍 fetch_csv() + load_config() → pandas DataFrame
↓
🧠 CivicLLM.ask(question, csv_as_text[:N])
↓
📊 plot_bar_count() → Quick data viz

#See ROADMAP.md for:

    ✅ Completed modules

    🛠️ Planned: mobile support, real RAG, form builder

    🌐 Policy comms export templates

    🔌 Multilingual interface options
	
	
#🤝 Contributing

Pull requests are welcome! 

#License

MIT 
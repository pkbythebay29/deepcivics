
# 🛣️ Deep Civics Roadmap

Deep Civics is an open, multilingual platform for accessing and interrogating public `.gov` datasets using LLMs. The goal is to empower individuals, journalists, researchers, policy thinkers and investment professionals to better understand and respond to civic data — anywhere in the world.

---

## ✅ Phase 1: Core Infrastructure

- [x] Python package: `deepcivics/`
- [x] Config via `deepcivics.yaml` + autogen
- [x] Notebook quickstarts 
- [x] Hugging Face LLM pipeline (replaceable via YAML)
- [x] Plotting + civic question answering
- [x] GitHub Pages landing and usage documentation
- [x] Binder integration for full in-browser use
- [x] Model alias system via `models.yaml`

---

## 🔜 Phase 2: Browser + Mobile Accessibility

- [ ] WASM-compatible notebook support (e.g., JupyterLite)
- [ ] Streamlit/PyScript front end for local/offline use
- [ ] Mobile-first interface (text + CSV upload)
- [ ] Voice-driven data query (basic STT → LLM)
- [ ] Offline config builder (URL → YAML → notebook)

---

## 🔭 Phase 3: Internationalization & Extensibility

- [ ] Prebuilt starter packs: 1 dataset per continent/domain
- [ ] Community-curated `datasets/` registry
- [ ] Add streaming model support (`OpenRouter`, `GPT4All`, etc.)
- [ ] Local LLM detection + fallback (via Transformers.js)


---

## 💡 Ideas (Not Yet Prioritized)

- Visual LLM comparison (accuracy vs. language vs. size)
- In-notebook explainer for LLM decisions ("why this answer?")
- Policy proposal synthesis assistant
- RDF export / semantic data tagging
- Civic question crowdsourcing (AskPublic-style model)

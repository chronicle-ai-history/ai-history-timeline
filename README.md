# AI History Timeline

78 milestones in the history of artificial intelligence from 1943 to 2026, each dated, categorized, scored for significance under a published rubric and linked to its primary source.

Curated by [Chronicle](https://epoch.founden.co/?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026), an interactive, sourced timeline of AI history. Every row links to a full dossier with the evidence behind it.

- **Current version and downloads:** [epoch.founden.co/data](https://epoch.founden.co/data?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) (CSV and JSON, always the live archive)
- **This snapshot:** 2026-10-02, 78 events, 1943 to 2026
- **License:** CC BY 4.0 for the table (scope below)

## Fields

| Field | Type | Description |
|---|---|---|
| `id` | string | Stable identifier of the event, also its dossier slug. |
| `date` | string | When it happened: YYYY-MM-DD, or YYYY when only the year is established. |
| `year` | integer | Calendar year. |
| `date_precision` | string | day, month or year: how precisely the date is known. |
| `name` | string | The subject as people name and search for it, for example Turing test. |
| `title` | string | Editorial headline. |
| `organization` | string | The person, lab or institution behind it. |
| `category` | string | Models, Research, Launches, Open source, Benchmarks, Policy, Culture or Robotics. |
| `summary` | string | What happened, in one sentence. |
| `impact` | string | Why it mattered, in one sentence. |
| `significance_score` | integer | Editorial significance from 0 to 100: the weighted sum of the 5 ratings under rubric 1.0. |
| `tier` | string | Defining (80 to 100), Major (60 to 79) or Notable (0 to 59). |
| `confidence` | string | Established, Supported or Provisional: how settled the evidence and historical perspective are. It does not change the score. |
| `rating_novelty` | integer | Conceptual shift, 0 to 5, worth 30% of the score: How much did this change the available approach? |
| `rating_influence` | integer | Downstream influence, 0 to 5, worth 25% of the score: How much subsequent research or practice does it underpin? |
| `rating_reach` | integer | Breadth of impact, 0 to 5, worth 20% of the score: How widely did the change matter beyond its original setting? |
| `rating_access` | integer | Access & diffusion, 0 to 5, worth 15% of the score: How much did it enable others to use or build on the work? |
| `rating_institutions` | integer | Institutional change, 0 to 5, worth 10% of the score: Did it change lasting infrastructure, governance, or incentives? |
| `primary_source_url` | string | The original paper, announcement or archive record. |
| `source_count` | integer | Sources cited in the event's dossier. |
| `dossier_url` | string | The event's full, cited dossier. |

## Quick start

```python
import pandas as pd

df = pd.read_csv("https://epoch.founden.co/data/ai-history-events.csv")  # always the current archive
df.sort_values("significance_score", ascending=False).head(10)[["year", "name", "organization", "significance_score"]]
```

## All events

| Date | Event | Organization | Category | Score |
|---|---|---|---|---|
| 1943 | [McCulloch-Pitts neuron](https://epoch.founden.co/events/mcculloch-pitts?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | McCulloch & Pitts | Research | 86 |
| 1950 | [Turing test](https://epoch.founden.co/events/the-question-that-started-it-all?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Alan Turing | Research | 95 |
| 1956 | [Dartmouth workshop](https://epoch.founden.co/events/artificial-intelligence-gets-a-name?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Dartmouth | Research | 94 |
| 1958 | [Perceptron](https://epoch.founden.co/events/the-perceptron?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Frank Rosenblatt | Research | 78 |
| 1959 | [Arthur Samuel's checkers program](https://epoch.founden.co/events/samuel-checkers?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Arthur Samuel · IBM | Research | 80 |
| 1965 | [DENDRAL expert system](https://epoch.founden.co/events/dendral?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Stanford · DENDRAL | Research | 71 |
| 1966 | [ELIZA chatbot](https://epoch.founden.co/events/a-conversation-with-eliza?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | MIT | Culture | 67 |
| 1966 | [Shakey the robot](https://epoch.founden.co/events/shakey-enters-the-world?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | SRI | Robotics | 67 |
| 1973 | [First AI winter](https://epoch.founden.co/events/the-first-ai-winter?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Research funding | Culture | 53 |
| 1982 | [Hopfield network](https://epoch.founden.co/events/hopfield-networks?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | John Hopfield | Research | 81 |
| 1986 | [Backpropagation](https://epoch.founden.co/events/learning-by-backpropagation?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Rumelhart, Hinton & Williams | Research | 93 |
| 1997-05-11 | [Deep Blue vs Kasparov](https://epoch.founden.co/events/deep-blue-beats-kasparov?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | IBM | Benchmarks | 62 |
| 1997 | [LSTM](https://epoch.founden.co/events/lstm?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Hochreiter & Schmidhuber | Research | 89 |
| 2003 | [Neural probabilistic language model](https://epoch.founden.co/events/neural-language-model?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Bengio, Ducharme, Vincent & Jauvin | Research | 80 |
| 2006 | [Deep belief networks](https://epoch.founden.co/events/the-deep-learning-revival?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Geoffrey Hinton & collaborators | Research | 75 |
| 2007 | [NVIDIA CUDA](https://epoch.founden.co/events/cuda?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | NVIDIA · CUDA | Launches | 91 |
| 2009 | [ImageNet](https://epoch.founden.co/events/imagenet-changes-the-dataset?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Princeton & Stanford | Research | 92 |
| 2011-02-16 | [IBM Watson](https://epoch.founden.co/events/watson-wins-jeopardy?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | IBM | Benchmarks | 58 |
| 2012 | [AlexNet](https://epoch.founden.co/events/the-alexnet-moment?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | University of Toronto | Research | 95 |
| 2013-01-16 | [word2vec](https://epoch.founden.co/events/word2vec?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Mikolov and collaborators · Google | Research | 83 |
| 2013-12-19 | [Deep Q-network](https://epoch.founden.co/events/deep-q-learning?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Mnih and collaborators · DeepMind | Research | 80 |
| 2013-12-20 | [Variational autoencoder](https://epoch.founden.co/events/variational-autoencoders?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Kingma & Welling | Research | 81 |
| 2014-06-10 | [Generative adversarial networks](https://epoch.founden.co/events/machines-learn-to-imagine?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Ian Goodfellow & collaborators | Research | 83 |
| 2014-09-10 | [Sequence-to-sequence learning](https://epoch.founden.co/events/sequence-to-sequence?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Sutskever, Vinyals & Le | Research | 80 |
| 2014-12-22 | [Adam optimizer](https://epoch.founden.co/events/adam?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Kingma & Ba | Research | 84 |
| 2015-12-10 | [ResNet](https://epoch.founden.co/events/resnet?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | He and collaborators · Microsoft | Research | 93 |
| 2015-12-11 | [OpenAI](https://epoch.founden.co/events/openai-is-founded?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Culture | 62 |
| 2016-03-15 | [AlphaGo vs Lee Sedol](https://epoch.founden.co/events/move-37-a-new-kind-of-intuition?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google DeepMind | Benchmarks | 83 |
| 2017-06-12 | [Transformer](https://epoch.founden.co/events/attention-is-all-you-need?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google researchers | Research | 98 |
| 2017-12-05 | [AlphaZero](https://epoch.founden.co/events/alphazero?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Silver and collaborators · DeepMind | Research | 75 |
| 2018-06-11 | [GPT-1](https://epoch.founden.co/events/the-first-gpt?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 78 |
| 2018-10-11 | [BERT](https://epoch.founden.co/events/bert-reads-both-ways?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google | Research | 86 |
| 2019-02-14 | [GPT-2](https://epoch.founden.co/events/gpt-2-and-the-release-debate?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 72 |
| 2019-10-23 | [T5](https://epoch.founden.co/events/t5?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Raffel and collaborators · Google | Research | 75 |
| 2020-05-28 | [GPT-3](https://epoch.founden.co/events/gpt-3-scales-up?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 86 |
| 2020-06-19 | [DDPM](https://epoch.founden.co/events/ddpm?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Ho, Jain & Abbeel | Research | 83 |
| 2020-10-22 | [Vision Transformer](https://epoch.founden.co/events/vision-transformer?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Dosovitskiy and collaborators · Google | Research | 83 |
| 2020-11-30 | [AlphaFold 2](https://epoch.founden.co/events/a-50-year-biology-problem?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google DeepMind | Research | 95 |
| 2021-01-05 | [DALL·E](https://epoch.founden.co/events/dall-e-language-becomes-image?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 72 |
| 2021-06-29 | [GitHub Copilot](https://epoch.founden.co/events/your-ai-pair-programmer?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | GitHub | Launches | 75 |
| 2021-12-20 | [Latent diffusion models](https://epoch.founden.co/events/latent-diffusion?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Rombach and collaborators | Research | 86 |
| 2022-03-04 | [InstructGPT](https://epoch.founden.co/events/instructgpt?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Ouyang and collaborators · OpenAI | Research | 86 |
| 2022-03-29 | [Chinchilla scaling laws](https://epoch.founden.co/events/chinchilla?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Hoffmann and collaborators · DeepMind | Research | 80 |
| 2022-04-06 | [DALL·E 2](https://epoch.founden.co/events/dall-e-2?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 69 |
| 2022-08-22 | [Stable Diffusion](https://epoch.founden.co/events/stable-diffusion-opens-up?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Stability AI & collaborators | Open source | 92 |
| 2022-11-30 | [ChatGPT release](https://epoch.founden.co/events/hello-chatgpt?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Launches | 85 |
| 2023-02-24 | [LLaMA](https://epoch.founden.co/events/llama-enters-the-picture?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Meta | Open source | 69 |
| 2023-03-14 | [GPT-4](https://epoch.founden.co/events/gpt-4-raises-the-bar?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 80 |
| 2023-03-14 | [Claude release](https://epoch.founden.co/events/meet-claude?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Launches | 54 |
| 2023-04-05 | [Segment Anything](https://epoch.founden.co/events/segment-anything?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Kirillov and collaborators · Meta | Research | 81 |
| 2023-07-18 | [Llama 2](https://epoch.founden.co/events/llama-2-opens-commercial-access?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Meta | Open source | 74 |
| 2023-09-27 | [Mistral 7B](https://epoch.founden.co/events/mistral-7b?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Mistral AI | Open source | 70 |
| 2023-11-01 | [Bletchley Declaration](https://epoch.founden.co/events/the-bletchley-declaration?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | AI Safety Summit | Policy | 60 |
| 2023-12-06 | [Google Gemini](https://epoch.founden.co/events/the-gemini-era-begins?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google DeepMind | Models | 75 |
| 2024-02-15 | [OpenAI Sora](https://epoch.founden.co/events/sora-imagines-in-motion?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 64 |
| 2024-03-04 | [Claude 3](https://epoch.founden.co/events/claude-3-arrives?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Models | 54 |
| 2024-05-08 | [AlphaFold 3](https://epoch.founden.co/events/alphafold-3-expands-the-picture?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google DeepMind & Isomorphic Labs | Research | 72 |
| 2024-05-13 | [GPT-4o](https://epoch.founden.co/events/gpt-4o-a-more-natural-interface?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 75 |
| 2024-06-20 | [Claude 3.5 Sonnet](https://epoch.founden.co/events/claude-35-sonnet?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Models | 63 |
| 2024-07-23 | [Llama 3.1](https://epoch.founden.co/events/llama-3-1?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Meta · Llama 3.1 | Open source | 74 |
| 2024-08-01 | [EU AI Act](https://epoch.founden.co/events/the-eu-ai-act-enters-into-force?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | European Union | Policy | 83 |
| 2024-09-12 | [OpenAI o1](https://epoch.founden.co/events/thinking-before-answering?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 72 |
| 2024-10-08 | [Hopfield and Hinton Nobel Prize](https://epoch.founden.co/events/nobel-physics-neural-networks?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Nobel Prize in Physics | Benchmarks | 60 |
| 2024-10-09 | [AlphaFold Nobel Prize](https://epoch.founden.co/events/nobel-protein-structure?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Nobel Prize in Chemistry | Benchmarks | 60 |
| 2024-10-22 | [Claude computer use](https://epoch.founden.co/events/claude-uses-a-computer?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Launches | 61 |
| 2024-11-25 | [Model Context Protocol](https://epoch.founden.co/events/a-common-language-for-tools?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Open source | 77 |
| 2025-01-20 | [DeepSeek-R1](https://epoch.founden.co/events/the-deepseek-moment?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | DeepSeek | Open source | 85 |
| 2025-02-24 | [Claude Code](https://epoch.founden.co/events/claude-code-enters-the-terminal?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Launches | 64 |
| 2025-03-25 | [Gemini 2.5](https://epoch.founden.co/events/gemini-2-5?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google DeepMind | Models | 64 |
| 2025-04-29 | [Qwen3](https://epoch.founden.co/events/qwen3?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Qwen team · Alibaba | Open source | 70 |
| 2025-05-22 | [Claude 4](https://epoch.founden.co/events/claude-4-gets-to-work?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Models | 58 |
| 2025-08-05 | [gpt-oss](https://epoch.founden.co/events/gpt-oss?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI · gpt-oss | Open source | 70 |
| 2025-08-07 | [GPT-5](https://epoch.founden.co/events/gpt-5-arrives?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 70 |
| 2025-11-18 | [Gemini 3](https://epoch.founden.co/events/gemini-3?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Google | Models | 70 |
| 2026-02-05 | [Claude Opus 4.6](https://epoch.founden.co/events/claude-opus-4-6?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Models | 47 |
| 2026-06-30 | [Claude Sonnet 5](https://epoch.founden.co/events/claude-sonnet-5?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | Anthropic | Models | 47 |
| 2026-08-02 | [AI Act enforcement](https://epoch.founden.co/events/ai-act-enforcement-expands?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | European Union | Policy | 61 |
| 2026-09-03 | [GPT-6 Astra](https://epoch.founden.co/events/gpt-6-astra?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026) | OpenAI | Models | 45 |

## How events are chosen and scored

Inclusion favors documented conceptual advances, enabling datasets and infrastructure, influential systems, material changes in access, and institutional turning points. A model release alone does not establish a breakthrough, and the coverage is curated rather than exhaustive.

Each event is rated 0 to 5 on 5 criteria with explicit anchors: conceptual shift (30%), downstream influence (25%), breadth of impact (20%), access & diffusion (15%), institutional change (10%). The weighted sum is the 0 to 100 `significance_score` (rubric 1.0). Confidence is reported separately and never multiplies the score. Full rubric, anchors and limitations: [methodology](https://epoch.founden.co/methodology?utm_source=github&utm_medium=dataset&utm_campaign=open_data_oct2026).

## Curation and limitations

Events were selected, dated and rated through Chronicle's editorial process, with AI-assisted research and writing. Every event links an original source (a paper, an official announcement or an archive record), and the dossiers cite more. Scores are comparative editorial judgments, not measurements: they carry hindsight, English-language, availability and recency bias, and a score of 81 is not meaningfully more precise than 80. Recent events are marked Provisional. Corrections are welcome through the contact options on the site.

## License

The table (the columns listed above) is licensed [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Credit it as: *Chronicle AI history dataset (https://epoch.founden.co/data), CC BY 4.0*. The long-form dossiers and research reports on the site are not covered by this license and remain all rights reserved. Linked sources keep their own licenses.

## Citation

Chronicle. (2026). AI history dataset: 78 scored and sourced events [Data set]. https://epoch.founden.co/data

```bibtex
@misc{chronicle_ai_history_2026,
  author = {{Chronicle}},
  title = {AI history dataset: 78 scored and sourced events},
  year = {2026},
  howpublished = {\url{https://epoch.founden.co/data}},
  note = {CC BY 4.0}
}
```

# Belarusian NLP and Speech Processing resources

A curated list of Belarusian Natural Language and Speech Processing resources, datasets, and models.

Inspired by [egorsmkv/speech-recognition-uk](https://github.com/egorsmkv/speech-recognition-uk).

<!-- omit from toc -->
### Table of Contents

- [🤝 Contributing](#-contributing)
- [🏡 Communities and platforms](#-communities-and-platforms)
- [📚 Datasets](#-datasets)
- [🎤 Speech-to-Text Models](#-speech-to-text-models)
- [🤖 Text-to-Speech Models](#-text-to-speech-models)
- [📝 NLP Models and Tools](#-nlp-models-and-tools)

### 🤝 Contributing

Contributions are very welcome! Please open a pull request to add missing resources, update entries, or fix any of the `TODO`s below. Help keep this list current.

### 🏡 Communities and platforms

- say.by — [Telegram](https://t.me/say_by)
- [corpus.by](https://www.corpus.by)
- [ssrlab.by](https://ssrlab.by)
- [bnkorpus.info](https://bnkorpus.info)
- [Belarus](https://github.com/Belarus) — GitHub organization
- [nlproc.by](https://github.com/nlprocby) — GitHub community

### 📚 Datasets

| Name | Type | Notes |
|------|------|-------|
| [Common Voice](https://commonvoice.mozilla.org/en/datasets) | STT | Mozilla multilingual speech corpus |
| [google/fleurs](https://huggingface.co/datasets/google/fleurs/viewer/be_by/train) | STT | |
| [knihi.com — Корпус беларускага маўлення](https://knihi.com/none/Korpus_bielaruskaha_maulennia_dla_trenirouki_niejronnych_sietak_zip.html) | STT | Corpus for neural network training. TODO: confirm dataset type |
| ssrlab | STT | TODO |
| [maaxap/BelarusianGLUE](https://huggingface.co/datasets/maaxap/BelarusianGLUE) | NLP | [Paper](https://aclanthology.org/2025.acl-long.25/) |
| [oscar](https://huggingface.co/datasets/oscar) | NLP | |
| [mc4](https://huggingface.co/datasets/mc4) | NLP | |
| [poritski/YABC](https://github.com/poritski/YABC) | NLP | Эксперыментальны корпус беларускай мовы (ЭКБМ) |
| [Belarus/GrammarDB](https://github.com/Belarus/GrammarDB) | NLP | Grammar Database of Belarusian language |
| [tsimafeip/Translator](https://github.com/tsimafeip/Translator) | NLP | Russian-Belarusian translation pairs |
| [UniversalDependencies/UD_Belarusian-HSE](https://github.com/UniversalDependencies/UD_Belarusian-HSE) | NLP | Universal Dependencies treebank. [Project page](https://universaldependencies.org/treebanks/be_hse/index.html) |
| [Tatoeba — Belarusian](https://tatoeba.org/en/sentences/show_all_in/bel/none) | NLP | Belarusian sentences in Tatoeba |

### 🎤 Speech-to-Text Models

| Name | Metrics | Notes |
|------|---------|-------|
| [ales/wav2vec2-cv-be](https://huggingface.co/ales/wav2vec2-cv-be) | - | wav2vec2 + kenlm language model, trained on Common Voice 8. [Demo](https://huggingface.co/spaces/ales/wav2vec2-cv-be-lm) · [Code](https://github.com/navalnica/wav2vec2-belarusian) |
| [openai/whisper](https://github.com/openai/whisper) | - | Original Whisper models from OpenAI |
| [ales/whisper-small-belarusian](https://huggingface.co/ales/whisper-small-belarusian) | WER `6.79` on CV11 | Whisper Small fine-tuned on Common Voice 11. [Demo](https://huggingface.co/spaces/ales/whisper-small-belarusian-demo) · [Code](https://github.com/navalnica/whisper-finetuning-be) |
| [ales/whisper-base-belarusian](https://huggingface.co/ales/whisper-base-belarusian) | - | Whisper Base fine-tuned on Common Voice 11. [Code](https://github.com/navalnica/whisper-finetuning-be) |
| [nvidia/stt_be_conformer_ctc_large](https://huggingface.co/nvidia/stt_be_conformer_ctc_large) | WER `4.8` on CV10 | NVIDIA NeMo Conformer-CTC |
| [nvidia/stt_be_conformer_transducer_large](https://huggingface.co/nvidia/stt_be_conformer_transducer_large) | WER `3.8` on CV10 | NVIDIA NeMo Conformer-Transducer |
| [nvidia/stt_be_fastconformer_hybrid_large_pc](https://huggingface.co/nvidia/stt_be_fastconformer_hybrid_large_pc) | WER `2.72` on CV12, P&C WER `3.87` on CV12 | NVIDIA NeMo FastConformer Hybrid |
| [espnet/belarusian_commonvoice_blstm](https://huggingface.co/espnet/belarusian_commonvoice_blstm) | - | ESPnet BLSTM trained on Common Voice |

### 🤖 Text-to-Speech Models

| Name | Metrics | Notes |
|------|---------|-------|
| [coqui-ai/TTS](https://github.com/coqui-ai/TTS/blob/dev/recipes/bel-alex73/README.md) | - | Official CoquiAI Belarusian recipe |
| [jhlfrfufyfn/bel-tts](https://github.com/jhlfrfufyfn/bel-tts) | - | GlowTTS + HifiGAN. [Model](https://huggingface.co/jhlfrfufyfn/bel-tts) · [HF demo](https://huggingface.co/spaces/jhlfrfufyfn/bel-tts) · [Web demo](https://nikuchin.fun/tts) ([source](https://github.com/jhlfrfufyfn/bel-tts-server)) |
| [alex73/belarusian-tts](https://github.com/alex73/belarusian-tts) | - | CoquiAI implementation by Yurii Paniv ([@robinhad](https://github.com/robinhad)). Original repo and models deleted — only fork remains |

### 📝 NLP Models and Tools

| Name | Topic | Notes |
|------|-------|-------|
| [KoichiYasuoka/roberta-small-belarusian-upos](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian-upos) | POS-tagging | UPOS tagset |
| [stanfordnlp/stanza-be](https://huggingface.co/stanfordnlp/stanza-be) | POS-tagging | Stanza framework |
| [poritski/YABC_Tagger](https://github.com/poritski/YABC_Tagger) | POS-tagging, Lemmatization | Rule-based. Perl. Uses [poritski/YABC](https://github.com/poritski/YABC) as grammar base |
| [volchek/beltagger](https://github.com/volchek/beltagger) | POS-tagging, Lemmatization | Improved C++ port of [poritski/YABC_Tagger](https://github.com/poritski/YABC_Tagger). Cross-platform. Known issues: requires Windows-1251 input (no UTF-8), tagset not fully compatible with BNKorpus, incomplete grammar base ([Belarus/GrammarDB](https://github.com/Belarus/GrammarDB) not yet incorporated), suffix table calculation not ported from Perl, depends on Boost |
| [alesdrobysh/belmorph](https://github.com/alesdrobysh/belmorph) | Morphology | Morphological analyzer, inflection, and lexeme generation for TypeScript. [Demo](https://alesdrobysh.github.io/belmorph) |
| [pkasila/bel-sklony](https://github.com/pkasila/bel-sklony) | Declension | Belarusian nouns declension web page. [Demo](https://sklony.pkasila.net/) |
| [KoichiYasuoka/roberta-small-belarusian](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian) | Masked Language Modeling | |

# Belarusian NLP and Speech Processing resources

This repository contains links to Belarusian Natural Language and Speech Processing resources and datasets.<br>

It is inspired by similar project with Ukrainian Speech Processing resources: [egorsmkv/speech-recognition-uk](https://github.com/egorsmkv/speech-recognition-uk)

### TODOs:
* add detailed descriptions to each of list items
* evaluate models on benchmarks and log their performance

# 🎙 Speech-to-Text

## 🎙💡 Implementations

* wav2vec2:
  * [yks72p/stt_be](https://github.com/yks72p/stt_be). Used Common Voice 8 dataset to train acoustic & language models.

* whisper:
  * original [openai/whisper](https://github.com/openai/whisper) models
  * Whisper models fine-tuned on Belarusian Common Voice 11 dataset:
    * [Whisper Small](https://huggingface.co/ales/whisper-small-belarusian)
    
* Nvidia NeMo models:
  * [nvidia/stt_be_conformer_ctc_large](https://huggingface.co/nvidia/stt_be_conformer_ctc_large)
  * [nvidia/stt_be_conformer_transducer_large](https://huggingface.co/nvidia/stt_be_conformer_transducer_large)
 
* ESPnet:
  * [espnet/belarusian_commonvoice_blstm](https://huggingface.co/espnet/belarusian_commonvoice_blstm)

## 🎙📊 Benchmarks

Model comparisons grouped by dataset. TODO

## 🎙📚 Datasets

* [Common Voice](https://commonvoice.mozilla.org/en/datasets). Speech recognition dataset
* Dataset from [knihi.com](https://knihi.com/none/Korpus_bielaruskaha_maulennia_dla_trenirouki_niejronnych_sietak_zip.html). TODO: what is the type of dataset?
* [google/fleurs](https://huggingface.co/datasets/google/fleurs/viewer/be_by/train)
* ssrlab: TODO. Speech recognition dataset

------

# 📢 Text-to-Speech

## 📢💡 Implementations

* CoquiAI implementations
  * [jhlfrfufyfn/bel-tts](https://github.com/jhlfrfufyfn/bel-tts). GlowTTS + HifiGan
    * [Code](https://github.com/jhlfrfufyfn/bel-tts)
    * [Model](https://huggingface.co/jhlfrfufyfn/bel-tts)
    * [Demo on HuggingFace](https://huggingface.co/spaces/jhlfrfufyfn/bel-tts)
    * [Demo on a custom web-page](https://nikuchin.fun/tts). The source code for the demo page: [here](https://github.com/jhlfrfufyfn/bel-tts-server)
  * [alex73/belarusian-tts](https://github.com/alex73/belarusian-tts). CoquiAI implementation by Yurii Paniv (@robinhad).<br>
    Original repo & models were deleted - only fork is available now

---

# 📝 NLP

## POS-tagging
* [KoichiYasuoka/roberta-small-belarusian-upos](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian-upos)
* [stanfordnlp/stanza-be](https://huggingface.co/stanfordnlp/stanza-be)
* [YABC_Tagger](https://github.com/poritski/YABC_Tagger). Trained on [Эксперыментальны корпус беларускай мовы](https://github.com/poritski/YABC)

## Masked Language Modeling
* [KoichiYasuoka/roberta-small-belarusian](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian)

## 📝📚 Datasets

* [Эксперыментальны корпус беларускай мовы, ЭКБМ](https://github.com/poritski/YABC)
* Universal dependencies dataset:
  * [Page](https://universaldependencies.org/treebanks/be_hse/index.html)
  * [GitHub Repository](https://github.com/UniversalDependencies/UD_Belarusian-HSE)
* [Tatoeba Belarusian sentences](https://tatoeba.org/en/sentences/show_all_in/bel/none)

---

# 🧍‍♀️🧍 Communities and platforms:
* [corpus.by](https://www.corpus.by)
* [ssrlab.by](https://ssrlab.by)
* [bnkorpus.info](https://bnkorpus.info)
* [Belarus](https://github.com/Belarus) organization on github
* [nlproc.by](https://github.com/nlprocby) community on github

---
# 🦔 Unsorted
* nothing for now

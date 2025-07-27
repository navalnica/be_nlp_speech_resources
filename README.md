# Belarusian NLP and Speech Processing resources

This repository contains links to Belarusian Natural Language and Speech Processing resources and datasets.<br>

It is inspired by similar project with Ukrainian Speech Processing resources: [egorsmkv/speech-recognition-uk](https://github.com/egorsmkv/speech-recognition-uk)

# 🧍‍♀️🧍 Communities and platforms:
* say.by - [web page](say.by), [telegram](https://t.me/say_by)
* [corpus.by](https://www.corpus.by)
* [ssrlab.by](https://ssrlab.by)
* [bnkorpus.info](https://bnkorpus.info)
* [Belarus](https://github.com/Belarus) organization on github
* [nlproc.by](https://github.com/nlprocby) community on github

# 💬➡️📘 Speech-to-Text

## 💬➡️📘 - 📚 Datasets

* [Common Voice](https://commonvoice.mozilla.org/en/datasets). Speech recognition dataset
* Dataset from [knihi.com](https://knihi.com/none/Korpus_bielaruskaha_maulennia_dla_trenirouki_niejronnych_sietak_zip.html). TODO: what is the type of dataset?
* [google/fleurs](https://huggingface.co/datasets/google/fleurs/viewer/be_by/train)
* ssrlab: TODO. Speech recognition dataset

## 💬➡️📘 - 🚀 Models

* wav2vec2 trained on Common Voice 8 + kenlm language model trained on Common Voice 8:
  * Model: [ales/wav2vec2-cv-be](https://huggingface.co/ales/wav2vec2-cv-be)
  * Demo: [ales/wav2vec2-cv-be-lm](https://huggingface.co/spaces/ales/wav2vec2-cv-be-lm)
  * Code: [navalnica/wav2vec2-belarusian](https://github.com/navalnica/wav2vec2-belarusian)

* whisper:
  * original [openai/whisper](https://github.com/openai/whisper) models
  * Whisper models fine-tuned on Belarusian Common Voice 11 dataset:
    * Whisper Small:
      * Model: [ales/whisper-small-belarusian](https://huggingface.co/ales/whisper-small-belarusian)
      * test WER on CommonVoice11: `6.79`
      * Demo: [ales/whisper-small-belarusian-demo](https://huggingface.co/spaces/ales/whisper-small-belarusian-demo)
      * Code: [navalnica/whisper-finetuning-be](https://github.com/navalnica/whisper-finetuning-be)
    * Whisper Base:
      * Model: [ales/whisper-base-belarusian](https://huggingface.co/ales/whisper-base-belarusian)
      * Code: [navalnica/whisper-finetuning-be](https://github.com/navalnica/whisper-finetuning-be)
    
* Nvidia NeMo models:
  * [nvidia/stt_be_conformer_ctc_large](https://huggingface.co/nvidia/stt_be_conformer_ctc_large)
    * [huggingface self-reported metric] test WER on CommonVoice10: `4.8`
  * [nvidia/stt_be_conformer_transducer_large](https://huggingface.co/nvidia/stt_be_conformer_transducer_large)
    * [huggingface self-reported metric] test WER on CommonVoice10: `3.8`
  * [nvidia/stt_be_fastconformer_hybrid_large_pc](https://huggingface.co/nvidia/stt_be_fastconformer_hybrid_large_pc)
    * [huggingface self-reported metric] test WER on CommonVoice12: `2.72`
    * [huggingface self-reported metric] test WER P&C CommonVoice12: `3.87`
 
* ESPnet:
  * [espnet/belarusian_commonvoice_blstm](https://huggingface.co/espnet/belarusian_commonvoice_blstm)

## 💬➡️📘 - 🥇 Benchmarks

Model comparisons grouped by dataset. TODO

------

# 📘➡️💬 Text-to-Speech

## 📘➡️💬 - 🚀 Models

### CoquiAI implementations

* official CoquiAI contains [recipe for Belarusian](https://github.com/coqui-ai/TTS/blob/dev/recipes/bel-alex73/README.md)
* [jhlfrfufyfn/bel-tts](https://github.com/jhlfrfufyfn/bel-tts). GlowTTS + HifiGan
  * [Code](https://github.com/jhlfrfufyfn/bel-tts)
  * [Model](https://huggingface.co/jhlfrfufyfn/bel-tts)
  * [Demo on HuggingFace](https://huggingface.co/spaces/jhlfrfufyfn/bel-tts)
  * [Demo on a custom web-page](https://nikuchin.fun/tts). The source code for the demo page: [here](https://github.com/jhlfrfufyfn/bel-tts-server)
* [alex73/belarusian-tts](https://github.com/alex73/belarusian-tts). CoquiAI implementation by Yurii Paniv (@robinhad).<br>
  Original repo & models were deleted - only fork is available now

---

# 📝 NLP

## 📝 - 📚 Datasets

* [BelarusianGLUE](https://huggingface.co/datasets/maaxap/BelarusianGLUE)
* [oscar](https://huggingface.co/datasets/oscar)
* [mc4](https://huggingface.co/datasets/mc4)
* [poritski/YABC](https://github.com/poritski/YABC) - Эксперыментальны корпус беларускай мовы, ЭКБМ
* [Belarus/GrammarDB](https://github.com/Belarus/GrammarDB) - Grammar Database of Belarusian language
* [tsimafeip/Translator](https://github.com/tsimafeip/Translator) - Dataset with russian-belarusian translation pairs
* Universal dependencies dataset:
  * [Page](https://universaldependencies.org/treebanks/be_hse/index.html)
  * [GitHub Repository](https://github.com/UniversalDependencies/UD_Belarusian-HSE)
* [Tatoeba Belarusian sentences](https://tatoeba.org/en/sentences/show_all_in/bel/none)

## 📝 - 🚀 Models

### POS-tagging
* [KoichiYasuoka/roberta-small-belarusian-upos](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian-upos)
* [stanfordnlp/stanza-be](https://huggingface.co/stanfordnlp/stanza-be)
* [poritski/YABC_Tagger](https://github.com/poritski/YABC_Tagger). Rule-based POS-tagger and lemmatizer.<br>
  Written in Perl. 
  Uses [poritski/YABC](https://github.com/poritski/YABC) as a Grammar base (?)
* [volchek/beltagger](https://github.com/volchek/beltagger).
  An improved version of [poritski/YABC_Tagger](https://github.com/poritski/YABC_Tagger) rule-based POS-tagger and lemmatizer.<br>
  Cross-platform, written in C++.<br>
  Known issues:
  * requires input data to be incoded in Windows-1251, does not support UTF-8;
  * tagset is not fully-compatible with BNKorpus's tagset and grammar base
  * grammar base used is not full enough. [Belarus/GrammarDB](https://github.com/Belarus/GrammarDB) is a better paradigms source but is not incorporated yet
  * suffix table calculation script is not ported from Perl to C++
  * code uses Boost libarary  
  
### Other
* [pkasila/bel-sklony](https://github.com/pkasila/bel-sklony) - web page with Belarusian nouns declension. Demo: [sklony.pkasila.net](https://sklony.pkasila.net/)

### Masked Language Modeling
* [KoichiYasuoka/roberta-small-belarusian](https://huggingface.co/KoichiYasuoka/roberta-small-belarusian)



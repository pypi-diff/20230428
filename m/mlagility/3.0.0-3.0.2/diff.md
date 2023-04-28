# Comparing `tmp/mlagility-3.0.0.tar.gz` & `tmp/mlagility-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlagility-3.0.0.tar", last modified: Thu Apr 27 22:04:48 2023, max compression
+gzip compressed data, was "mlagility-3.0.2.tar", last modified: Fri Apr 28 17:01:28 2023, max compression
```

## Comparing `mlagility-3.0.0.tar` & `mlagility-3.0.2.tar`

### file list

```diff
@@ -1,1930 +1,1932 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.515469 mlagility-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 22:04:23.000000 mlagility-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-27 22:04:48.515469 mlagility-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-27 22:04:23.000000 mlagility-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.243471 mlagility-3.0.0/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.247471 mlagility-3.0.0/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/diffusers/clip_text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/diffusers/safety_clipvision.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/diffusers/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/diffusers/vae_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.247471 mlagility-3.0.0/models/graph_convolutions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/chebconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/dnaconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/egconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/feastconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/gatedgraphconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/generalconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/leconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/pnaconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/resgatedgraphconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/sageconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/graph_convolutions/tagconv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.343471 mlagility-3.0.0/models/popular_on_huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/0x7194633_keyt5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/AI-Growth-Lab_PatentSBERTa.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/AmazonScience_qanlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/BM-K_KoSimCSE-roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Babelscape_wikineural-multilingual-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Bhuvana_t5-base-spellchecker.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-ca-pos-egy.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-ca.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-da-pos-msa.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-da.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-mix-pos-msa.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-msa.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CompVis_ldm-text2im-large-256.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/CompVis_stable-diffusion-v1-4.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/DMetaSoul_sbert-chinese-general-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-masakhaner.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-ner-hrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Davlan_distilbert-base-multilingual-cased-ner-hrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Davlan_xlm-roberta-base-ner-hrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Davlan_xlm-roberta-large-ner-hrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/DmitryPogrebnoy_MedRuRobertaLarge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ElKulako_cryptobert.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-base-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-large-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-tiny-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/FinanceInc_finbert_fls.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/HooshvareLab_bert-fa-zwnj-base-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/HooshvareLab_distilbert-fa-zwnj-base-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Huffon_sentence-klue-roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-DeBERTa-v2-710M-Chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-NLI.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-Sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IIC_dpr-spanish-passage_encoder-allqa-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IIC_dpr-spanish-question_encoder-allqa-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IlyaGusev_rubert_telegram_headlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/IlyaGusev_rut5_base_sum_gazeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Intel_dpt-large-ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Intel_dpt-large.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_camembert-ner-with-dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_camembert-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_roberta-large-ner-english.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/K024_mt5-zh-ja-en-trimmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KBLab_sentence-bert-swedish-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KES_T5-TTParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KES_TEC-English.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Kamuuung_autonlp-lessons_tagging-606217261.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_bert-base-japanese-upos.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_bert-large-japanese-wikipedia-ud-head.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_deberta-base-japanese-aozora-ud-head.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_deberta-base-thai-ud-head.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_roberta-base-thai-spm-upos.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base-finetuned-kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base-ssv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MaRiOrOsSi_t5-base-finetuned-question-answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MarcBrun_ixambert-finetuned-squad-eu-en.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Michau_t5-base-en-generate-headline.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MilaNLProc_feel-it-italian-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MilaNLProc_feel-it-italian-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-anli.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-docnli-ling-2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-large-mnli-fever-anli-ling-wanli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-xsmall-mnli-fever-anli-ling-binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-mnli-xnli.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-xnli-multilingual-nli-2mil7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_policy-distilbert-7d.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Musixmatch_umberto-commoncrawl-cased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Narrativa_bsc_roberta2roberta_shared-spanish-finetuned-mlsum-summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/NbAiLab_nb-bert-base-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/NeuML_bert-small-cord19qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_gpt2-vietnamese.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_t5-en-vi-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_vibert4news-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Preetiha_clause_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Recognai_bert-base-spanish-wwm-cased-xnli.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Recognai_zeroshot_selectra_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_bert_bfd.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_t5_xl_bfd.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_t5_xl_uniref50.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Sahajtomar_German_Zeroshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-2B-mono.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-2B-multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-mono.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-6B-mono.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-6B-multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-large-ntp-py.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Salesforce_mixqg-base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Sehong_t5-large-QuestionGeneration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/SenseTime_deformable-detr.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Sentdex_GPyT.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Seznam_small-e-czech.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_roberta_toxicity_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_russian_toxicity_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_xlmr_formality_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/StevenLimcorn_indonesian-roberta-base-emotion-classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/TristanBehrens_js-fakes-4bars.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/TurkuNLP_sbert-cased-finnish-paraphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/UBC-NLP_AraT5-base-title-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Unbabel_gec-t5_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/VMware_vbert-2021-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Visual-Attention-Network_van-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Visual-Attention-Network_van-tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Wikidepia_IndoT5-base-paraphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/Xuhui_ToxDect-roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/abhishek_autonlp-bbc-news-classification-37229289.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ahmedrachid_FinancialBERT-Sentiment-Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ai4bharat_IndicBART.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ai4bharat_IndicBARTSS.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/aiknowyou_aiky-sentence-bertino.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-large-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-large-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-xlarge-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-xlarge-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-xxlarge-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/albert-xxlarge-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-klej-cased-tokenizer-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-klej-cased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-large-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allenai_t5-small-next-word-generator-qoogle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/allenai_t5-small-squad2-question-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/aneuraz_awesome-align-with-co.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ans_vaccinating-covid-tweets.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/apple_deeplabv3-mobilevit-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/apple_deeplabv3-mobilevit-xx-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/apple_mobilevit-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/apple_mobilevit-xx-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/asi_gpt-fr-cased-base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/assemblyai_bert-large-uncased-sst2.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/aubmindlab_araelectra-base-discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/aujer_ni_model_8_19.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/avichr_heBERT.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/avichr_heBERT_sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/aware-ai_bart-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/azwierzc_herbert-large-poquad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/azwierzc_plt5-base-poquad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/azwierzc_plt5-large-poquad.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/batterydata_batterybert-cased-squad-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-base-multilingual-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-base-multilingual-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-base-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-large-cased-whole-word-masking.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-large-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-large-uncased-whole-word-masking.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bert-large-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-bert-base-aihub-mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-bert-base-mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-sentence-roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-sroberta-base-continue-learning-by-mnr.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_bert-base-uncased-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_distilbert-base-uncased-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_electra-base-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_roberta-base-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bigscience_T0.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/bigscience_T0p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/blinoff_roberta-base-russian-v0.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cahya_bert-base-indonesian-522M.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cahya_distilbert-base-indonesian.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cahya_roberta-base-indonesian-522M.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-single.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-hate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-irony.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-offensive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-xlm-roberta-base-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/chkla_parlbert-topic-german.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/clips_mfaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-nli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/codeparrot_codeparrot-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/codeparrot_codeparrot.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_LaBSE-en-ru.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-base-cased-nli-threeway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny-sentiment-balanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny-toxicity.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny2.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rut5-small-chitchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rut5-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-MiniLM2-L6-H768.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-xsmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-distilroberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2m_crossSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2o_arabic_crossSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2o_chinese_simplified_crossSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_multilingual_XLSum.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/d4data_biomedical-ner-all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-nlvr2.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-vqa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-mlm.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dangvantuan_sentence-camembert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dangvantuan_sentence-camembert-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/daveni_twitter-xlm-roberta-emotion-es.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_all-mpnet-base-v2-table.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_deberta-v3-base-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_deberta-v3-large-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_electra-base-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_roberta-base-squad2-covid.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_roberta-base-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_tinyroberta-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_xlm-roberta-base-squad2-distilled.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deepset_xlm-roberta-large-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dennlinger_bert-wiki-paragraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dennlinger_roberta-cls-consec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deutsche-telekom_bert-multi-english-german-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/deutsche-telekom_electra-base-de-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/distilbert-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/distilbert-base-multilingual-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/distilbert-base-uncased-finetuned-sst-2-english.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/distilbert-base-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/distilroberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dkleczek_bert-base-polish-cased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dkleczek_bert-base-polish-uncased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/doc2query_all-t5-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/doc2query_all-with_prefix-t5-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/doc2query_msmarco-t5-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dslim_bert-base-NER.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dslim_bert-large-NER.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/dumitrescustefan_bert-base-romanian-cased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/edumunozsala_beto_sentiment_analysis_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/edumunozsala_vit_base-224-in21k-ft-cifar100.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/efederici_cross-encoder-umberto-stsb.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/efederici_sentence-bert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ehdwns1516_klue-roberta-base-kornli.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/embedding-data_distilroberta-base-sentence-transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/esiebomajeremiah_autonlp-email-classification-657119381.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_camembert-base-squadFR-fquad-piaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_dpr-ctx_encoder-fr_qa-camembert.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_dpr-question_encoder-fr_qa-camembert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/fabiochiu_t5-base-tag-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_bart-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_bart-large.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_contriever-msmarco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_contriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-base-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-base-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-large-224-22k-1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-small-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-tiny-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-xlarge-224-22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-xlarge-384-22k-1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_data2vec-vision-base-ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-small-distilled-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-small-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-tiny-distilled-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-tiny-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_detr-resnet-50-panoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_detr-resnet-50.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vitb16.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vitb8.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vits16.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vits8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_flava-full.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_levit-128S.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-base-ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-base-coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-large-ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-small-coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-tiny-ade.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_mbart-large-50.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_opt-125m.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_opt-350m.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_regnet-y-040.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_vit-mae-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_vit-mae-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/facebook_xlm-roberta-xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/fhswf_bert_de_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-community_clip-rsicd-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-community_roberta-hindi.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-community_t5-large-wikisplit.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_mpnet-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v4_MiniLM-L6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_st-codesearch-distilroberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_stackoverflow_mpnet-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flexudy_t5-base-multi-sentence-doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/flexudy_t5-small-wav2vec2-grammar-fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/fran-martinez_scibert_scivocab_cased_ner_jnlpba.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/funnel-transformer_large-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/funnel-transformer_xlarge-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/gerulata_slovakbert.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/gilf_french-camembert-postag-model.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/gilf_french-postag-model.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_bert2bert_L-24_wmt_de_en.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_byt5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_byt5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_byt5-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_canine-c.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_canine-s.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_ddpm-celebahq-256.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_ddpm-cifar10-32.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_electra-base-discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_electra-base-generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_electra-large-discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_electra-small-discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_fnet-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_long-t5-local-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_long-t5-tglobal-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_long-t5-tglobal-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_long-t5-tglobal-xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_mobilebert-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-base-patch16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-base-patch32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-large-patch14.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_bbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_cnn_daily_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_discofuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_t5-small-ssm-nq.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-224-in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch32-224-in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch32-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-huge-patch14-224-in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-224-in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch32-224-in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch32-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hakurei_lit-6B.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-dutch-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-polish-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hetpandya_t5-base-tapaco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hetpandya_t5-small-tapaco.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hiiamsid_sentence_similarity_hindi.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hiiamsid_sentence_similarity_spanish_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/imranraad_idiom-xlm-roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/inkoziev_rugpt_chitchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/intfloat_simlm-msmarco-reranker.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/j-hartmann_emotion-english-distilroberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/j-hartmann_purchase-intention-english-roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/j-hartmann_sentiment-roberta-large-english-3-classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/jaehyeong_koelectra-base-v3-generalized-sentiment-analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/jhgan_ko-sbert-multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/jhgan_ko-sroberta-multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/jhgan_ko-sroberta-sts.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/joeddav_bart-large-mnli-yahoo-answers.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/johngiorgi_declutr-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/johngiorgi_declutr-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/jsylee_scibert_scivocab_uncased-finetuned-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_ft_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc-lt.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/keepitreal_vietnamese-sbert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ken11_albert-base-japanese-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/kiheh85202_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/kiri-ai_distiluse-base-multilingual-cased-et.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/laituan245_molt5-large-smiles2caption.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/law-ai_InLegalBERT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/lcw99_t5-base-korean-chit-chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/liandarizkia_SA01-IndoBert.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/madhurjindal_autonlp-Gibberish-Detector-492513457.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/malteos_scincl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/marefa-nlp_marefa-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/matthewburke_korean_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/maxpe_twitter-roberta-base-jun2022_sem_eval_2018_task_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mdhugol_indonesia-bert-sentiment-classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/melll-uff_bertweetbr.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/michiyasunaga_BioLinkBERT-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/michiyasunaga_BioLinkBERT-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/michiyasunaga_LinkBERT-base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_BiomedVLP-CXR-BERT-specialized.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k-ft22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k-ft22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_codebert-base-mlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_conditional-detr-resnet-50.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_cvt-13.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_prophetnet-large-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-101.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-152.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-18.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-34.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-50.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384-in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224-in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window12-384-in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224-in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-small-patch4-window7-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-tiny-patch4-window7-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_swinv2-tiny-patch4-window8-256.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_tapex-large-finetuned-tabfact.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-base-handwritten.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-base-printed.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-handwritten.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-printed.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-str.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-small-handwritten.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-small-stage1.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/microsoft_xprophetnet-large-wiki100-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ml4pubmed_BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext_pub_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ml6team_bert-base-uncased-city-country-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ml6team_distilbert-base-german-cased-toxic-comments.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/model-attribution-challenge_codegen-350M-multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/model-attribution-challenge_opt-350m.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/model-attribution-challenge_xlnet-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/monilouise_ner_news_portuguese.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_TinyBERT-spanish-uncased-finetuned-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-base-german-finetuned-ler.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-italian-finedtuned-squadv1-it-alfa.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-medium-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-multi-cased-finetuned-xquadv1.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-small-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-small2bert-small-finetuned-cnn_daily_mail-summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-spanish-cased-finetuned-ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-tiny-5-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-tiny-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-german-finetuned-summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-spanish-finetuned-summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-turkish-summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_codebert-base-finetuned-detect-insecure-code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_distill-bert-base-spanish-wwm-cased-finetuned-spa-squad2-es.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_electra-small-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_electricidad-base-discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_roberta-base-1B-1-finetuned-squadv1.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_spanbert-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_spanbert-large-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-common_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-e2m-intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-imdb-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-quartz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-question-generation-ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-span-sentiment-extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-squadv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-wikiSQL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-small-finetuned-quora-for-paraphrasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nateraw_vit-age-classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nateraw_vit-base-patch16-224-cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/navteca_bart-large-mnli.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/navteca_nli-deberta-v3-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/navteca_roberta-base-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/navteca_roberta-large-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nbroad_mt5-base-qgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/neuralspace-reverie_indic-transformers-bn-distilbert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/neuraly_bert-base-italian-cased-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/neuropark_sahajBERT.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nickmuchi_yolos-small-rego-plates-detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nickprock_xlm-roberta-base-banking77-classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nkoh01_MSRoberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_groupvit-gcc-yfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-ade-512-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-1024-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-512-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-768-768.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b1-finetuned-ade-512-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b2-finetuned-cityscapes-1024-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-ade-512-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-cityscapes-1024-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-ade-512-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-cityscapes-1024-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b5-finetuned-cityscapes-1024-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/nytimesrd_paraphrase-MiniLM-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/obrizum_all-MiniLM-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/obrizum_all-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-base-patch16.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-base-patch32.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-large-patch14.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/optimum_all-MiniLM-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/patrickvonplaten_longformer2roberta-cnn_dailymail-fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/paust_pko-t5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/paust_pko-t5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/persiannlp_mt5-large-parsinlu-arc-comqa-obqa-multiple-choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/philschmid_BERT-Banking77.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-conll2003.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-3-class.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-4-class.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/phiyodr_bart-large-finetuned-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/phiyodr_bert-base-finetuned-squad2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/phpaiola_ptt5-base-summ-cstnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pierreguillou_ner-bert-large-cased-pt-lenerbr.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pin_senda.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pritamdeka_S-BioBert-snli-multinli-stsb.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pritamdeka_S-Biomed-Roberta-snli-multinli-stsb.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pritamdeka_S-Bluebert-snli-multinli-stsb.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pritamdeka_S-PubMedBert-MS-MARCO.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/projecte-aina_roberta-base-ca-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pszemraj_grammar-synthesis-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pszemraj_grammar-synthesis-large.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/pvl_labse_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/racai_distilbert-base-romanian-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ramsrigouthamg_t5-large-paraphraser-diverse-high-quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ramsrigouthamg_t5_paraphraser.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/raynardj_ner-gene-dna-rna-jnlpba-pubmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/razent_spbert-mlm-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/razent_spbert-mlm-wso-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoBERT-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoBERT-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoGPT2-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoGPT2-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/readerbench_jurBERT-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/recobo_agriculture-bert-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/saattrupdan_nbailab-base-ner-scandi.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-lid-lince.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-ner-lince.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-pos-lince.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-spaeng-sentiment-analysis-lince.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sail_poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/salesken_natural_rephrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/salesken_paraphrase_diversity_ranker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/salesken_paraphrase_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/salesken_text_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sampathkethineedi_industry-classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/savasy_bert-base-turkish-ner-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/savasy_bert-base-turkish-sentiment-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sberbank-ai_sbert_large_mt_nlu_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sberbank-ai_sbert_large_nlu_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_LaBSE.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L12-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L12-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L6-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-distilroberta-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-mpnet-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_all-roberta-large-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_allenai-specter.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-base-nli-cls-token.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-base-nli-max-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-base-nli-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-base-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-base-wikipedia-sections-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-large-nli-max-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-large-nli-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_bert-large-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_clip-ViT-B-32-multilingual-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-stsb-quora-ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distilroberta-base-msmarco-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distilroberta-base-paraphrase-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distiluse-base-multilingual-cased-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_distiluse-base-multilingual-cased-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_facebook-dpr-ctx_encoder-multiset-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_facebook-dpr-ctx_encoder-single-nq-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_facebook-dpr-question_encoder-multiset-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_facebook-dpr-question_encoder-single-nq-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_gtr-t5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_gtr-t5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_gtr-t5-xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L-12-v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L-6-v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L6-cos-v5.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-bert-base-dot-v5.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-dot-prod-v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-tas-b.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-cos-v5.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-dot-v5.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-multilingual-en-de-v2-tmp-lng-aligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-multilingual-en-de-v2-tmp-trained-scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilroberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-ance-firstp.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-cos-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-dot-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-distilbert-cos-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-cos-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-dot-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-bert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-distilroberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-roberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nli-roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_nq-distilbert-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L12-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L3-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-TinyBERT-L6-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-albert-small-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-distilroberta-base-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-distilroberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-multilingual-MiniLM-L12-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-multilingual-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_paraphrase-xlm-r-multilingual-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_quora-distilbert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_quora-distilbert-multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_roberta-base-nli-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_roberta-base-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_roberta-large-nli-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_roberta-large-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_sentence-t5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_sentence-t5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_sentence-t5-xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_sentence-t5-xxl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-bert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-bert-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-distilbert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-distilroberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-mpnet-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-roberta-base-v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_stsb-xlm-r-multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_use-cmlm-multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_xlm-r-100langs-bert-base-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_xlm-r-bert-base-nli-stsb-mean-tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_xlm-r-distilroberta-base-paraphrase-v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/setu4993_LaBSE.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/setu4993_smaller-LaBSE.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/siebert_sentiment-roberta-large-english.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sijunhe_nezha-cn-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/sijunhe_nezha-large-wwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/snunlp_KR-SBERT-V40K-klueNLI-augSTS.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/soheeyang_rdr-ctx_encoder-single-nq-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/soheeyang_rdr-question_encoder-single-nq-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/soleimanian_financial-roberta-large-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/squirro_albert-base-v2-squad_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/strombergnlp_dant5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/svalabs_gbert-large-zeroshot-nli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/t5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/t5-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/t5-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/taeminlee_kogpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/tartuNLP_EstBERT_NER.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/tdobrxl_ClinicBERT.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/tennessejoyce_titlewave-t5-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/teven_all_bs160_allneg.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/teven_all_bs192_hardneg.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/teven_all_bs320_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/thanathorn_mt5-cpe-kmutt-thai-sentence-sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/thunlp_Lawformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/transfo-xl-wt103.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/tugstugi_bert-large-mongolian-uncased.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/tuhailong_SimCSE-bert-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_albert-base-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-12_H-128.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-12_H-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-2_H-128.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-4_H-256.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-4_H-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-6_H-128.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-6_H-768.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-8_H-256.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_chinese_roberta_L-8_H-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-chinese-extractive-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-chinanews-chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-cluener2020-chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-dianping-chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-binary-chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-full-chinese.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-word-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_t5-base-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_t5-small-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_t5-v1_1-base-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uer_t5-v1_1-small-chinese-cluecorpussmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/unicamp-dl_translation-pt-en-t5.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/unitary_multilingual-toxic-xlm-roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/unitary_toxic-bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/unitary_unbiased-toxic-roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ushikado_yuyuyui-chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/uw-madison_nystromformer-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/valhalla_bart-large-finetuned-squadv1.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/valhalla_t5-base-squad.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/vblagoje_dpr-ctx_encoder-single-lfqa-wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/vinvino02_glpn-kitti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/vinvino02_glpn-nyu.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_dpr-ctx_encoder-bert-base-multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/voidful_dpr-question_encoder-bert-base-multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/wanyu_IteraTeR-ROBERTA-Intention-Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/whaleloops_phrase-bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/wonrax_phobert-base-vietnamese-sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-clm-ende-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-clm-enfr-1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-mlm-en-2048.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-roberta-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-roberta-large-finetuned-conll03-german.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlm-roberta-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlnet-base-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/xlnet-large-cased.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ybelkada_japanese-roberta-question-answering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ydshieh_roberta-large-ner-english.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/ydshieh_vit-gpt2-coco-en.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-esg.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-fls.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-tone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.343471 mlagility-3.0.0/models/selftest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/selftest/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/selftest/twolayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.487470 mlagility-3.0.0/models/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/adv_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/bat_resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_base_patch16_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_large_patch16_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/beit_large_patch16_512.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/botnet26t_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/botnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_m36_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_m48_448.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_s24_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_s24_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_s36_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_xs24_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_xxs24_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_xxs24_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_xxs36_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cait_xxs36_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/coat_lite_mini.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/coat_lite_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/coat_lite_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/coat_mini.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/coat_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convit_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convit_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convmixer_1024_20_ks9_p14.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convmixer_1536_20.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convmixer_768_32.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_base_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_base_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_base_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_large_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_large_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_large_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_nano.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_nano_hnf.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_nano_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_small_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_small_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_small_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_tiny_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_tiny_hnf.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_tiny_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_tiny_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_xlarge_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_xlarge_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/convnext_xlarge_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_15_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_15_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_15_dagger_408.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_18_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_18_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_18_dagger_408.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_9_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_9_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_base_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_small_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/crossvit_tiny_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_focus_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_focus_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_focus_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_focus_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3darknet_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3edgenet_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3se_edgenet_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3sedarknet_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3sedarknet_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cs3sedarknet_xdw.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cspdarknet53.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cspresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cspresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cspresnet50w.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/cspresnext50.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/darknet17.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/darknet21.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/darknet53.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/darknetaa53.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_base_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_base_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_huge_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_huge_patch14_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_large_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_large_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_small_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_small_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit3_small_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_base_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_base_distilled_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_small_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_tiny_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/deit_tiny_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet121.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet121d.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet161.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet169.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet201.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenet264.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/densenetblur121d.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla102.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla102x.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla102x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla169.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla34.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla46_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla46x_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla60.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla60_res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla60_res2next.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla60x.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dla60x_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f0.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f1.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f2.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f3.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f4.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f5.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dm_nfnet_f6.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn107.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn131.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn68.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn68b.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn92.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/dpn98.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_botnext26ts_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_halonext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_nfnet_l0.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_nfnet_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_nfnet_l2.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_nfnet_l3.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_resnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/eca_vovnet39b.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet101d.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet200d.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet269d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet26t.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnetlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnext26t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ecaresnext50t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/edgenext_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/edgenext_small_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/edgenext_x_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/edgenext_xx_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b0_g16_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b0_g8_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b0_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b2a.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b3_g8_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b3_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b3a.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_b8.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_cc_b0_4e.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_cc_b0_8e.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_cc_b1_8e.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_el.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_el_pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_es_pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_l2.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_lite0.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_lite1.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_lite2.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_lite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnet_lite4.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_rw_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_rw_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_rw_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/efficientnetv2_xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ens_adv_inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet19b_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet19b_slim.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet19b_slim_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet39b.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet39b_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet57b.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ese_vovnet99b.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/fbnetc_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/fbnetv3_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/fbnetv3_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/fbnetv3_g.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gc_efficientnetv2_rw_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gcresnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gcresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gcresnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gcresnext50ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gernet_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gernet_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gernet_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ghostnet_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ghostnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ghostnet_130.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet101_v1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet101_v1c.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet101_v1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet101_v1s.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet152_v1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet152_v1c.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet152_v1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet152_v1s.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet18_v1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet34_v1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet50_v1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet50_v1c.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet50_v1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnet50_v1s.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_senet154.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_seresnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gluon_xception65.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gmixer_12_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gmixer_24_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gmlp_b16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gmlp_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/gmlp_ti16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/halo2botnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/halonet26t.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/halonet50ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/halonet_h1.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/haloregnetz_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_e.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hardcorenas_f.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w18.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w18_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w18_small_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w30.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w32.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w40.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w44.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w48.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/hrnet_w64.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ig_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ig_resnext101_32x32d.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ig_resnext101_32x48d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ig_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/inception_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/jx_nest_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/jx_nest_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/jx_nest_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lambda_resnet26rpt_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lambda_resnet26t.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lambda_resnet50ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lamhalobotnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lcnet_035.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lcnet_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lcnet_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lcnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/lcnet_150.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_senet154.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnext26_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/legacy_seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_128.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_128s.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_192.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_256d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/levit_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_b16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_b16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_b16_224_miil.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_b16_224_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_b32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_l16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_l16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_l32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixer_s32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixnet_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixnet_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixnet_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixnet_xl.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mixnet_xxl.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_a1.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mnasnet_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_035.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_110d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_120d.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv2_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_large_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_large_100_miil.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_large_100_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_small_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevit_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevit_xs.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevit_xxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_125.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_150.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_150_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_150_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_175.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_175_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_175_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_200_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/mobilevitv2_200_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nasnetalarge.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nest_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nest_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nest_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_ecaresnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_ecaresnet26.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_ecaresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_regnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_resnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_resnet26.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_seresnet26.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nf_seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f0.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f1.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f2.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f3.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f4.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f5.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f6.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_f7.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/nfnet_l0.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_b_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_b_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_s_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_s_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_ti_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_ti_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_xs_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pit_xs_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/pnasnet5large.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/poolformer_m36.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/poolformer_m48.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/poolformer_s24.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/poolformer_s36.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetv_040.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetv_064.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_002.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_004.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_006.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_008.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_016.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_032.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_040.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_064.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_080.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_120.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_160.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetx_320.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_002.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_004.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_006.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_008.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_016.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_032.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_040.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_040s_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_064.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_080.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_120.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_160.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnety_320.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_005.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_040.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_040h.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_b16.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_b16_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_c16.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_c16_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_d32.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_d8_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/regnetz_e8.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_a2.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b1g4.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b2g4.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/repvgg_b3g4.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net101_26w_4s.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net50_14w_8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net50_26w_4s.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net50_26w_6s.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net50_26w_8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2net50_48w_2s.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/res2next50.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_12_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_12_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_12_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_24_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_24_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_36_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_36_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_big_24_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_big_24_224_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resmlp_big_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest101e.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest14d.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest269e.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest26d.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest50d_1s4x24d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnest50d_4s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet101d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet10t.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet14t.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet152d.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet18d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet200.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet200d.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet26.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet26d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet26t.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet32ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet34d.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet50_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet50t.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet51q.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnet61q.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetaa101d.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetaa50.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetaa50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetblur101d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetblur18.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetblur50.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetblur50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs101.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs152.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs200.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs270.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs350.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs420.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetrs50.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101x1_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101x1_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101x3_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_101x3_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152d.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x2_bit_teacher.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x2_bit_teacher_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x2_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x2_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x4_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_152x4_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50d_evob.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50d_evos.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50d_frn.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50d_gn.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50t.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50x1_bit_distilled.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50x1_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50x1_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50x3_bitm.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnetv2_50x3_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/resnext50d_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnet_130.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnet_150.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnet_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnetr_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnetr_130.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnetr_150.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/rexnetr_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sebotnet33ts_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sedarknet21.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sehalonet33ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/selecsls42.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/selecsls42b.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/selecsls60.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/selecsls60b.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/selecsls84.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/semnasnet_050.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/semnasnet_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/semnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/semnasnet_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/semobilevit_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/senet154.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sequencer2d_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sequencer2d_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/sequencer2d_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet152d.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet200d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet269d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnetaa50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext101d_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext26d_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext26t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext26tn_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/seresnextaa101d_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/skresnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/skresnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/skresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/skresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/skresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/spnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/ssl_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_base_patch4_window12_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_base_patch4_window12_384_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_base_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_base_patch4_window7_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_large_patch4_window12_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_large_patch4_window12_384_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_large_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_large_patch4_window7_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_s3_base_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_s3_small_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_s3_tiny_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_small_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swin_tiny_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_base_window12_192_22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_base_window12to16_192to256_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_base_window12to24_192to384_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_base_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_base_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_base_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_base_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_base_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_giant_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_giant_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_huge_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_huge_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_large_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_large_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_small_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_small_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_small_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_tiny_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_tiny_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_cr_tiny_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_large_window12_192_22k.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_large_window12to16_192to256_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_large_window12to24_192to384_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_small_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_small_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_tiny_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swinv2_tiny_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/swsl_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b0_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b0_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b1_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b1_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b2_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b2_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b3_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b3_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b4_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b4_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b5_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b5_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b6_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b6_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b7_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b7_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b8.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_b8_ap.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_cc_b0_4e.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_cc_b0_8e.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_cc_b1_8e.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_el.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_l2_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_l2_ns_475.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_lite0.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_lite1.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_lite2.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_lite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnet_lite4.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_l_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_l_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_m_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_m_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_s_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_s_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_xl_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_efficientnetv2_xl_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mixnet_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mixnet_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mixnet_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_large_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_large_minimal_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tf_mobilenetv3_small_minimal_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tinynet_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tinynet_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tinynet_c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tinynet_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tinynet_e.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tnt_b_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tnt_s_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_densenet121.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_resnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_resnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_resnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/tv_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_pcpvt_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_pcpvt_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_pcpvt_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_svt_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_svt_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/twins_svt_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg11.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg11_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg13.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg13_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg16_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vgg19_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/visformer_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/visformer_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_18x2_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224_miil.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_224_sam.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_plus_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch32_224_sam.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch32_plus_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch8_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_patch8_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_r26_s32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_r50_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_r50_s16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_r50_s16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_resnet26d_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_resnet50_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_resnet50_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_base_resnet50d_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_giant_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_gigantic_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_huge_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_huge_patch14_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_r50_s32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_r50_s32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_large_r50_s32_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch16_cls_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch16_clsgap_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch16_plus_240.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_base_patch32_plus_rpn_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_cls_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_relpos_small_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_18x2_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_36x1_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_patch8_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_r26_s32_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_r26_s32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_r26_s32_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_resnet26d_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_small_resnet50d_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_srelpos_medium_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_srelpos_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d1_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d1_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d2_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d2_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d3_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d3_448.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d4_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d4_448.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d5_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d5_448.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/volo_d5_512.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vovnet39a.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/vovnet57a.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/wide_resnet101_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/wide_resnet50_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception41.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception41p.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception65.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception65p.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xception71.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_large_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_medium_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_nano_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_small_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/timm/xcit_tiny_24_p8_384_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.499470 mlagility-3.0.0/models/torch_hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/alexnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/convnext_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/convnext_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/convnext_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/convnext_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/dcgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/densenet121.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/densenet161.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/densenet169.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/densenet201.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_v2_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_v2_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/efficientnet_v2_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/ghostnet_1x.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/googlenet.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/hardnet39ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/hardnet68.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/hardnet68ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/hardnet85.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv1_resnest50.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_mobilenet_v3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_resnest50.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_resnest50_380x380.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mealv2_resnest50_cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/midas_v2.1_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/midas_v3_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/midas_v3_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mnasnet0_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mnasnet0_75.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mnasnet1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mnasnet1_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mobilenet_v3_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/mobilenet_v3_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/proxyless_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/proxyless_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/proxyless_mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/proxyless_mobile_14.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_16gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_1_6gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_32gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_3_2gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_400mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_800mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_x_8gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_128gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_16gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_1_6gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_32gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_3_2gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_400mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_800mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/regnet_y_8gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest101.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest200.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest269.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_1s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_1s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_1s4x24d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_2s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_2s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_4s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnest50_fast_4s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet101_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet18_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet18_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet34_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet34_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet50_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnet50_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnext101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/se_resnet101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/shufflenet_v2_x0_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/shufflenet_v2_x1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/shufflenet_v2_x1_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/shufflenet_v2_x2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/squeezenet1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/squeezenet1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/swin_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/swin_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/swin_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg11.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg11_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg13.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg13_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg16_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vgg19_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vit_b_16.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vit_b_32.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vit_h_14.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vit_l_16.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/vit_l_32.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/wide_resnet101_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torch_hub/wide_resnet50_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.499470 mlagility-3.0.0/models/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/fasterrcnn_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/fasterrcnn_resnet50_fpn_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/fcos_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/keypointrcnn_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/maskrcnn_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/maskrcnn_resnet50_fpn_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/retinanet_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/retinanet_resnet50_fpn_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/ssd300_vgg16.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/torchvision/ssdlite320_mobilenet_v3_large.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.507470 mlagility-3.0.0/models/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bert_for_question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bert_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bert_tiny_for_sequence_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/bigbird_pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/biggan.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/blenderbot_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/camembert.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/convbert.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/data2vecaudio.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/data2vectext.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/deberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/deit.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/deit_base_for_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/deit_tiny_for_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/detr.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/detr_for_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/distil_wav2vec2_for_audio_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/distilbert.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/distilbert_for_question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/distilhubert_for_audio_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/electra.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/electra_for_sequence_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/flaubert.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/funnel.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/funnel_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/gpt1.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/gpt2_doublehead.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/ibert.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/imagegpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/layoutlm.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/luke.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/m2m_100.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/marian.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/marianmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/megatron_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/minilmv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilebert.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilebert_for_sequence_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilevit_small_for_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilevit_x_small_for_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mobilevit_xx_small_for_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mpnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mt5_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mt5_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/mt5_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/openai_doublehead.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/perceiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/poolformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/rag.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/realm.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/rembert.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/retribert.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/roformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/segformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/sew.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/sew_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/speech_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/speech_encoder_decoder_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/speech_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/splinter.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/squeezebert.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/t5_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/t5_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/t5_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/t5_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/unispeech.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/unispeech_sat.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/vision_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/wav2vec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/xglm.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/xlm.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/xlm_roberta.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/xlnet-512.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/xlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 22:04:23.000000 mlagility-3.0.0/models/transformers/yolos_tiny_for_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 22:04:23.000000 mlagility-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:04:48.515469 mlagility-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-27 22:04:23.000000 mlagility-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.243471 mlagility-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    18504 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/analysis/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/analysis/tf_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/analysis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility/api/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/execute_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/ortmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/run_ort_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/script_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/setup_ort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/api/trtmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15942 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/cli/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility/common/
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/common/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/mlagility/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/mlagility.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    89365 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 22:04:48.000000 mlagility-3.0.0/src/mlagility.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.511469 mlagility-3.0.0/src/onnxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.515469 mlagility-3.0.0/src/onnxflow/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/onnx_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/quantization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/tensor_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/common/tf_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.515469 mlagility-3.0.0/src/onnxflow/justbuildit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4973 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/buildit.py
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/hummingbird.py
--rw-r--r--   0 runner    (1001) docker     (123)    21873 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/ignition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/justbuildit/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:04:48.515469 mlagility-3.0.0/src/onnxflow/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 22:04:23.000000 mlagility-3.0.0/src/onnxflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.443534 mlagility-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 17:00:56.000000 mlagility-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-28 17:01:28.443534 mlagility-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-28 17:00:56.000000 mlagility-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.027530 mlagility-3.0.2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.027530 mlagility-3.0.2/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/diffusers/clip_text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/diffusers/safety_clipvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/diffusers/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/diffusers/vae_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.027530 mlagility-3.0.2/models/graph_convolutions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/chebconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/dnaconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/egconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/feastconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/gatedgraphconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/generalconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/leconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/pnaconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/resgatedgraphconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/sageconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/graph_convolutions/tagconv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.155531 mlagility-3.0.2/models/popular_on_huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/0x7194633_keyt5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/AI-Growth-Lab_PatentSBERTa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/AmazonScience_qanlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/BM-K_KoSimCSE-roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Babelscape_wikineural-multilingual-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Bhuvana_t5-base-spellchecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-ca-pos-egy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-da-pos-msa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-da.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-mix-pos-msa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CAMeL-Lab_bert-base-arabic-camelbert-msa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CompVis_ldm-text2im-large-256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/CompVis_stable-diffusion-v1-4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/DMetaSoul_sbert-chinese-general-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-masakhaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-ner-hrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Davlan_distilbert-base-multilingual-cased-ner-hrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Davlan_xlm-roberta-base-ner-hrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Davlan_xlm-roberta-large-ner-hrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/DmitryPogrebnoy_MedRuRobertaLarge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ElKulako_cryptobert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-base-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-large-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-tiny-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/FinanceInc_finbert_fls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/HooshvareLab_bert-fa-zwnj-base-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/HooshvareLab_distilbert-fa-zwnj-base-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Huffon_sentence-klue-roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-DeBERTa-v2-710M-Chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-NLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-Sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IIC_dpr-spanish-passage_encoder-allqa-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IIC_dpr-spanish-question_encoder-allqa-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IlyaGusev_rubert_telegram_headlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/IlyaGusev_rut5_base_sum_gazeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Intel_dpt-large-ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Intel_dpt-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_camembert-ner-with-dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_camembert-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_roberta-large-ner-english.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/K024_mt5-zh-ja-en-trimmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KBLab_sentence-bert-swedish-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KES_T5-TTParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KES_TEC-English.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Kamuuung_autonlp-lessons_tagging-606217261.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_bert-base-japanese-upos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_bert-large-japanese-wikipedia-ud-head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_deberta-base-japanese-aozora-ud-head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_deberta-base-thai-ud-head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_roberta-base-thai-spm-upos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base-finetuned-kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base-ssv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MaRiOrOsSi_t5-base-finetuned-question-answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MarcBrun_ixambert-finetuned-squad-eu-en.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Michau_t5-base-en-generate-headline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MilaNLProc_feel-it-italian-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MilaNLProc_feel-it-italian-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-anli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-docnli-ling-2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-large-mnli-fever-anli-ling-wanli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-xsmall-mnli-fever-anli-ling-binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-mnli-xnli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-xnli-multilingual-nli-2mil7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_policy-distilbert-7d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Musixmatch_umberto-commoncrawl-cased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Narrativa_bsc_roberta2roberta_shared-spanish-finetuned-mlsum-summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/NbAiLab_nb-bert-base-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/NeuML_bert-small-cord19qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_gpt2-vietnamese.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_t5-en-vi-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_vibert4news-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Preetiha_clause_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Recognai_bert-base-spanish-wwm-cased-xnli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Recognai_zeroshot_selectra_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_bert_bfd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_t5_xl_bfd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_t5_xl_uniref50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Sahajtomar_German_Zeroshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-2B-mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-2B-multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-6B-mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-6B-multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-large-ntp-py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Salesforce_mixqg-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Sehong_t5-large-QuestionGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/SenseTime_deformable-detr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Sentdex_GPyT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Seznam_small-e-czech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_roberta_toxicity_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_russian_toxicity_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_xlmr_formality_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/StevenLimcorn_indonesian-roberta-base-emotion-classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/TristanBehrens_js-fakes-4bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/TurkuNLP_sbert-cased-finnish-paraphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/UBC-NLP_AraT5-base-title-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Unbabel_gec-t5_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/VMware_vbert-2021-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Visual-Attention-Network_van-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Visual-Attention-Network_van-tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Wikidepia_IndoT5-base-paraphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/Xuhui_ToxDect-roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/abhishek_autonlp-bbc-news-classification-37229289.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ahmedrachid_FinancialBERT-Sentiment-Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ai4bharat_IndicBART.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ai4bharat_IndicBARTSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/aiknowyou_aiky-sentence-bertino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-large-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-large-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-xlarge-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-xlarge-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-xxlarge-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/albert-xxlarge-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-klej-cased-tokenizer-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-klej-cased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-large-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allenai_t5-small-next-word-generator-qoogle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/allenai_t5-small-squad2-question-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/aneuraz_awesome-align-with-co.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ans_vaccinating-covid-tweets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/apple_deeplabv3-mobilevit-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/apple_deeplabv3-mobilevit-xx-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/apple_mobilevit-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/apple_mobilevit-xx-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/asi_gpt-fr-cased-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/assemblyai_bert-large-uncased-sst2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/aubmindlab_araelectra-base-discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/aujer_ni_model_8_19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/avichr_heBERT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/avichr_heBERT_sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/aware-ai_bart-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/azwierzc_herbert-large-poquad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/azwierzc_plt5-base-poquad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/azwierzc_plt5-large-poquad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/batterydata_batterybert-cased-squad-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-base-multilingual-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-base-multilingual-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-base-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-large-cased-whole-word-masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-large-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-large-uncased-whole-word-masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bert-large-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-bert-base-aihub-mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-bert-base-mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-sentence-roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-sroberta-base-continue-learning-by-mnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_bert-base-uncased-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_distilbert-base-uncased-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_electra-base-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_roberta-base-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bigscience_T0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/bigscience_T0p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/blinoff_roberta-base-russian-v0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cahya_bert-base-indonesian-522M.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cahya_distilbert-base-indonesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cahya_roberta-base-indonesian-522M.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-hate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-irony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-offensive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-xlm-roberta-base-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/chkla_parlbert-topic-german.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/clips_mfaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-nli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/codeparrot_codeparrot-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/codeparrot_codeparrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_LaBSE-en-ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-base-cased-nli-threeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny-sentiment-balanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny-toxicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rut5-small-chitchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rut5-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-MiniLM2-L6-H768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-xsmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-distilroberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2m_crossSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2o_arabic_crossSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2o_chinese_simplified_crossSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_multilingual_XLSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/d4data_biomedical-ner-all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-nlvr2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-mlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dangvantuan_sentence-camembert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dangvantuan_sentence-camembert-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/daveni_twitter-xlm-roberta-emotion-es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_all-mpnet-base-v2-table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_deberta-v3-base-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_deberta-v3-large-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_electra-base-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_roberta-base-squad2-covid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_roberta-base-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_tinyroberta-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_xlm-roberta-base-squad2-distilled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deepset_xlm-roberta-large-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dennlinger_bert-wiki-paragraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dennlinger_roberta-cls-consec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deutsche-telekom_bert-multi-english-german-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/deutsche-telekom_electra-base-de-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/distilbert-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/distilbert-base-multilingual-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/distilbert-base-uncased-finetuned-sst-2-english.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/distilbert-base-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/distilroberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dkleczek_bert-base-polish-cased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dkleczek_bert-base-polish-uncased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/doc2query_all-t5-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/doc2query_all-with_prefix-t5-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/doc2query_msmarco-t5-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dslim_bert-base-NER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dslim_bert-large-NER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/dumitrescustefan_bert-base-romanian-cased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/edumunozsala_beto_sentiment_analysis_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/edumunozsala_vit_base-224-in21k-ft-cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/efederici_cross-encoder-umberto-stsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/efederici_sentence-bert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ehdwns1516_klue-roberta-base-kornli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/embedding-data_distilroberta-base-sentence-transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/esiebomajeremiah_autonlp-email-classification-657119381.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_camembert-base-squadFR-fquad-piaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_dpr-ctx_encoder-fr_qa-camembert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_dpr-question_encoder-fr_qa-camembert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/fabiochiu_t5-base-tag-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_bart-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_bart-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_contriever-msmarco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_contriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-base-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-base-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-large-224-22k-1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-small-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-tiny-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-xlarge-224-22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-xlarge-384-22k-1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_data2vec-vision-base-ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-small-distilled-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-small-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-tiny-distilled-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-tiny-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_detr-resnet-50-panoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_detr-resnet-50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vitb16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vitb8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vits16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vits8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_flava-full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_levit-128S.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-base-ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-base-coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-large-ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-small-coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-tiny-ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_mbart-large-50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_opt-125m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_opt-350m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_regnet-y-040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_vit-mae-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_vit-mae-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/facebook_xlm-roberta-xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/fhswf_bert_de_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-community_clip-rsicd-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-community_roberta-hindi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-community_t5-large-wikisplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_mpnet-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v4_MiniLM-L6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_st-codesearch-distilroberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_stackoverflow_mpnet-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flexudy_t5-base-multi-sentence-doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/flexudy_t5-small-wav2vec2-grammar-fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/fran-martinez_scibert_scivocab_cased_ner_jnlpba.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/funnel-transformer_large-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/funnel-transformer_xlarge-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/gerulata_slovakbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/gilf_french-camembert-postag-model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/gilf_french-postag-model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_bert2bert_L-24_wmt_de_en.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_byt5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_byt5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_byt5-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_canine-c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_canine-s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_ddpm-celebahq-256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_ddpm-cifar10-32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_electra-base-discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_electra-base-generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_electra-large-discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_electra-small-discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_fnet-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_long-t5-local-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_long-t5-tglobal-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_long-t5-tglobal-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_long-t5-tglobal-xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_mobilebert-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-base-patch16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-base-patch32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-large-patch14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_bbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_cnn_daily_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_discofuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_t5-small-ssm-nq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-224-in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch32-224-in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch32-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-huge-patch14-224-in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-224-in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch32-224-in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch32-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hakurei_lit-6B.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-dutch-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-polish-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hetpandya_t5-base-tapaco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hetpandya_t5-small-tapaco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hiiamsid_sentence_similarity_hindi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hiiamsid_sentence_similarity_spanish_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/imranraad_idiom-xlm-roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/inkoziev_rugpt_chitchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/intfloat_simlm-msmarco-reranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/j-hartmann_emotion-english-distilroberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/j-hartmann_purchase-intention-english-roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/j-hartmann_sentiment-roberta-large-english-3-classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/jaehyeong_koelectra-base-v3-generalized-sentiment-analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/jhgan_ko-sbert-multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/jhgan_ko-sroberta-multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/jhgan_ko-sroberta-sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/joeddav_bart-large-mnli-yahoo-answers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/johngiorgi_declutr-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/johngiorgi_declutr-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/jsylee_scibert_scivocab_uncased-finetuned-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_ft_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc-lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/keepitreal_vietnamese-sbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ken11_albert-base-japanese-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/kiheh85202_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/kiri-ai_distiluse-base-multilingual-cased-et.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/laituan245_molt5-large-smiles2caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/law-ai_InLegalBERT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/lcw99_t5-base-korean-chit-chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/liandarizkia_SA01-IndoBert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/madhurjindal_autonlp-Gibberish-Detector-492513457.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/malteos_scincl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/marefa-nlp_marefa-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/matthewburke_korean_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/maxpe_twitter-roberta-base-jun2022_sem_eval_2018_task_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mdhugol_indonesia-bert-sentiment-classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/melll-uff_bertweetbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/michiyasunaga_BioLinkBERT-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/michiyasunaga_BioLinkBERT-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/michiyasunaga_LinkBERT-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_BiomedVLP-CXR-BERT-specialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k-ft22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k-ft22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_codebert-base-mlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_conditional-detr-resnet-50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_cvt-13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_prophetnet-large-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384-in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224-in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window12-384-in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224-in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-small-patch4-window7-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-tiny-patch4-window7-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_swinv2-tiny-patch4-window8-256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_tapex-large-finetuned-tabfact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-base-handwritten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-base-printed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-handwritten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-printed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-small-handwritten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-small-stage1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/microsoft_xprophetnet-large-wiki100-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ml4pubmed_BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext_pub_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ml6team_bert-base-uncased-city-country-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ml6team_distilbert-base-german-cased-toxic-comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/model-attribution-challenge_codegen-350M-multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/model-attribution-challenge_opt-350m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/model-attribution-challenge_xlnet-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/monilouise_ner_news_portuguese.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_TinyBERT-spanish-uncased-finetuned-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-base-german-finetuned-ler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-italian-finedtuned-squadv1-it-alfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-medium-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-multi-cased-finetuned-xquadv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-small-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-small2bert-small-finetuned-cnn_daily_mail-summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-spanish-cased-finetuned-ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-tiny-5-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-tiny-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-german-finetuned-summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-spanish-finetuned-summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-turkish-summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_codebert-base-finetuned-detect-insecure-code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_distill-bert-base-spanish-wwm-cased-finetuned-spa-squad2-es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_electra-small-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_electricidad-base-discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_roberta-base-1B-1-finetuned-squadv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_spanbert-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_spanbert-large-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-common_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-e2m-intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-imdb-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-quartz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-question-generation-ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-span-sentiment-extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-squadv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-wikiSQL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-small-finetuned-quora-for-paraphrasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nateraw_vit-age-classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nateraw_vit-base-patch16-224-cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/navteca_bart-large-mnli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/navteca_nli-deberta-v3-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/navteca_roberta-base-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/navteca_roberta-large-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nbroad_mt5-base-qgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/neuralspace-reverie_indic-transformers-bn-distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/neuraly_bert-base-italian-cased-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/neuropark_sahajBERT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nickmuchi_yolos-small-rego-plates-detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nickprock_xlm-roberta-base-banking77-classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nkoh01_MSRoberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_groupvit-gcc-yfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-ade-512-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-1024-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-512-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-768-768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b1-finetuned-ade-512-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b2-finetuned-cityscapes-1024-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-ade-512-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-cityscapes-1024-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-ade-512-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-cityscapes-1024-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b5-finetuned-cityscapes-1024-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/nytimesrd_paraphrase-MiniLM-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/obrizum_all-MiniLM-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/obrizum_all-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-base-patch16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-base-patch32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-large-patch14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/optimum_all-MiniLM-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/patrickvonplaten_longformer2roberta-cnn_dailymail-fp16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/paust_pko-t5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/paust_pko-t5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/persiannlp_mt5-large-parsinlu-arc-comqa-obqa-multiple-choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/philschmid_BERT-Banking77.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-conll2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-3-class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-4-class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/phiyodr_bart-large-finetuned-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/phiyodr_bert-base-finetuned-squad2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/phpaiola_ptt5-base-summ-cstnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pierreguillou_ner-bert-large-cased-pt-lenerbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pin_senda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pritamdeka_S-BioBert-snli-multinli-stsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pritamdeka_S-Biomed-Roberta-snli-multinli-stsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pritamdeka_S-Bluebert-snli-multinli-stsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pritamdeka_S-PubMedBert-MS-MARCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/projecte-aina_roberta-base-ca-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pszemraj_grammar-synthesis-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pszemraj_grammar-synthesis-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/pvl_labse_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/racai_distilbert-base-romanian-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ramsrigouthamg_t5-large-paraphraser-diverse-high-quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ramsrigouthamg_t5_paraphraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/raynardj_ner-gene-dna-rna-jnlpba-pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/razent_spbert-mlm-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/razent_spbert-mlm-wso-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoBERT-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoBERT-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoGPT2-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoGPT2-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/readerbench_jurBERT-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/recobo_agriculture-bert-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/saattrupdan_nbailab-base-ner-scandi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-lid-lince.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-ner-lince.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-pos-lince.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-spaeng-sentiment-analysis-lince.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sail_poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/salesken_natural_rephrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/salesken_paraphrase_diversity_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/salesken_paraphrase_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/salesken_text_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sampathkethineedi_industry-classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/savasy_bert-base-turkish-ner-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/savasy_bert-base-turkish-sentiment-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sberbank-ai_sbert_large_mt_nlu_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sberbank-ai_sbert_large_nlu_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_LaBSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L12-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L12-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L6-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-MiniLM-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-distilroberta-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-mpnet-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_all-roberta-large-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_allenai-specter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-base-nli-cls-token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-base-nli-max-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-base-nli-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-base-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-base-wikipedia-sections-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-large-nli-max-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-large-nli-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_bert-large-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_clip-ViT-B-32-multilingual-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distilbert-base-nli-stsb-quora-ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distilroberta-base-msmarco-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distilroberta-base-paraphrase-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distiluse-base-multilingual-cased-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_distiluse-base-multilingual-cased-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_facebook-dpr-ctx_encoder-multiset-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_facebook-dpr-ctx_encoder-single-nq-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_facebook-dpr-question_encoder-multiset-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_facebook-dpr-question_encoder-single-nq-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_gtr-t5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_gtr-t5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_gtr-t5-xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L-12-v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L-6-v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L6-cos-v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-bert-base-dot-v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-dot-prod-v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-tas-b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-cos-v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-dot-v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-multilingual-en-de-v2-tmp-lng-aligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-multilingual-en-de-v2-tmp-trained-scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilroberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-ance-firstp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-roberta-base-v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-cos-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-dot-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-distilbert-cos-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-cos-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-dot-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-bert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-distilroberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-roberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nli-roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_nq-distilbert-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L12-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L3-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-MiniLM-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-TinyBERT-L6-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-albert-small-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-distilroberta-base-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-distilroberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-multilingual-MiniLM-L12-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-multilingual-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_paraphrase-xlm-r-multilingual-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_quora-distilbert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_quora-distilbert-multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_roberta-base-nli-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_roberta-base-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_roberta-large-nli-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_roberta-large-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_sentence-t5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_sentence-t5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_sentence-t5-xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_sentence-t5-xxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-bert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-bert-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-distilbert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-distilroberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-mpnet-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-roberta-base-v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_stsb-xlm-r-multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_use-cmlm-multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_xlm-r-100langs-bert-base-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_xlm-r-bert-base-nli-stsb-mean-tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_xlm-r-distilroberta-base-paraphrase-v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/setu4993_LaBSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/setu4993_smaller-LaBSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/siebert_sentiment-roberta-large-english.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sijunhe_nezha-cn-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/sijunhe_nezha-large-wwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/snunlp_KR-SBERT-V40K-klueNLI-augSTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/soheeyang_rdr-ctx_encoder-single-nq-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/soheeyang_rdr-question_encoder-single-nq-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/soleimanian_financial-roberta-large-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/squirro_albert-base-v2-squad_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/strombergnlp_dant5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/svalabs_gbert-large-zeroshot-nli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/t5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/t5-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/t5-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/taeminlee_kogpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/tartuNLP_EstBERT_NER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/tdobrxl_ClinicBERT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/tennessejoyce_titlewave-t5-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/teven_all_bs160_allneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/teven_all_bs192_hardneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/teven_all_bs320_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/thanathorn_mt5-cpe-kmutt-thai-sentence-sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/thunlp_Lawformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/transfo-xl-wt103.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/tugstugi_bert-large-mongolian-uncased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/tuhailong_SimCSE-bert-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_albert-base-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-12_H-128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-12_H-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-2_H-128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-4_H-256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-4_H-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-6_H-128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-6_H-768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-8_H-256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_chinese_roberta_L-8_H-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-chinese-extractive-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-chinanews-chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-cluener2020-chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-dianping-chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-binary-chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-full-chinese.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-word-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_t5-base-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_t5-small-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_t5-v1_1-base-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uer_t5-v1_1-small-chinese-cluecorpussmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/unicamp-dl_translation-pt-en-t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/unitary_multilingual-toxic-xlm-roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/unitary_toxic-bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/unitary_unbiased-toxic-roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ushikado_yuyuyui-chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/uw-madison_nystromformer-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/valhalla_bart-large-finetuned-squadv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/valhalla_t5-base-squad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/vblagoje_dpr-ctx_encoder-single-lfqa-wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/vinvino02_glpn-kitti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/vinvino02_glpn-nyu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_dpr-ctx_encoder-bert-base-multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/voidful_dpr-question_encoder-bert-base-multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/wanyu_IteraTeR-ROBERTA-Intention-Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/whaleloops_phrase-bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/wonrax_phobert-base-vietnamese-sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-clm-ende-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-clm-enfr-1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-mlm-en-2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-roberta-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-roberta-large-finetuned-conll03-german.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlm-roberta-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlnet-base-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/xlnet-large-cased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ybelkada_japanese-roberta-question-answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ydshieh_roberta-large-ner-english.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/ydshieh_vit-gpt2-coco-en.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-fls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-tone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.155531 mlagility-3.0.2/models/selftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/selftest/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/selftest/twolayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.371533 mlagility-3.0.2/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/adv_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/bat_resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_base_patch16_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_large_patch16_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/beit_large_patch16_512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/botnet26t_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/botnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_m36_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_m48_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_s24_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_s24_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_s36_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_xs24_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_xxs24_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_xxs24_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_xxs36_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cait_xxs36_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/coat_lite_mini.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/coat_lite_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/coat_lite_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/coat_mini.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/coat_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convit_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convit_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convmixer_1024_20_ks9_p14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convmixer_1536_20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convmixer_768_32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_base_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_base_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_base_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_large_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_large_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_large_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_nano_hnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_nano_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_small_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_small_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_small_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_tiny_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_tiny_hnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_tiny_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_tiny_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_xlarge_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_xlarge_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/convnext_xlarge_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_15_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_15_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_15_dagger_408.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_18_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_18_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_18_dagger_408.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_9_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_9_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_base_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_small_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/crossvit_tiny_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_focus_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_focus_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_focus_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_focus_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3darknet_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3edgenet_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3se_edgenet_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3sedarknet_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3sedarknet_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cs3sedarknet_xdw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cspdarknet53.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cspresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cspresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cspresnet50w.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/cspresnext50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/darknet17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/darknet21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/darknet53.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/darknetaa53.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_base_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_base_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_huge_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_huge_patch14_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_large_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_large_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_small_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_small_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit3_small_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_base_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_base_distilled_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_small_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_tiny_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/deit_tiny_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet121d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet161.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet169.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet201.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenet264.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/densenetblur121d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla102.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla102x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla102x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla169.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla46_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla46x_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla60.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla60_res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla60_res2next.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dla60x_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dm_nfnet_f6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn68.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn68b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn92.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/dpn98.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_botnext26ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_halonext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_nfnet_l0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_nfnet_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_nfnet_l2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_nfnet_l3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_resnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/eca_vovnet39b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet101d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet269d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnetlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnext26t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ecaresnext50t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/edgenext_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/edgenext_small_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/edgenext_x_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/edgenext_xx_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b0_g16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b0_g8_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b0_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b2a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b3_g8_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b3_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b3a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_b8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_cc_b0_4e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_cc_b0_8e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_cc_b1_8e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_el.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_el_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_es_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_l2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_lite0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_lite1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_lite2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_lite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnet_lite4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_rw_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_rw_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_rw_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/efficientnetv2_xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ens_adv_inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet19b_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet19b_slim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet19b_slim_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet39b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet39b_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet57b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ese_vovnet99b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/fbnetc_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/fbnetv3_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/fbnetv3_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/fbnetv3_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gc_efficientnetv2_rw_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gcresnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gcresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gcresnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gcresnext50ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gernet_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gernet_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gernet_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ghostnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ghostnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ghostnet_130.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet101_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet101_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet101_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet101_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet152_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet152_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet152_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet152_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet18_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet34_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet50_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet50_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet50_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnet50_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_senet154.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_seresnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gluon_xception65.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gmixer_12_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gmixer_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gmlp_b16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gmlp_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/gmlp_ti16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/halo2botnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/halonet26t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/halonet50ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/halonet_h1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/haloregnetz_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hardcorenas_f.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w18_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w18_small_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w40.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w44.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/hrnet_w64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ig_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ig_resnext101_32x32d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ig_resnext101_32x48d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ig_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/inception_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/jx_nest_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/jx_nest_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/jx_nest_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lambda_resnet26rpt_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lambda_resnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lambda_resnet50ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lamhalobotnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lcnet_035.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lcnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lcnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lcnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/lcnet_150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_senet154.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnext26_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/legacy_seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_128s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_192.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_256d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/levit_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_b16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_b16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_b16_224_miil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_b16_224_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_b32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_l16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_l16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_l32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixer_s32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixnet_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixnet_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixnet_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixnet_xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mixnet_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_a1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mnasnet_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_035.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_110d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_120d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv2_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_large_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_large_100_miil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_large_100_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_small_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevit_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevit_xs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevit_xxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_125.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_150_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_150_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_175.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_175_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_175_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_200_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/mobilevitv2_200_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nasnetalarge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nest_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nest_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nest_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_ecaresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_ecaresnet26.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_ecaresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_regnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_resnet26.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_seresnet26.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nf_seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_f7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/nfnet_l0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_b_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_b_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_s_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_s_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_ti_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_ti_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_xs_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pit_xs_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/pnasnet5large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/poolformer_m36.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/poolformer_m48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/poolformer_s24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/poolformer_s36.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetv_040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetv_064.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_032.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_064.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_120.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_160.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetx_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_032.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_040s_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_064.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_120.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_160.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnety_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_040h.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_b16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_b16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_c16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_c16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_d32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_d8_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/regnetz_e8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_a2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b1g4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b2g4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/repvgg_b3g4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net101_26w_4s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net50_14w_8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net50_26w_4s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net50_26w_6s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net50_26w_8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2net50_48w_2s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/res2next50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_12_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_12_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_12_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_24_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_36_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_36_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_big_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_big_24_224_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resmlp_big_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest101e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest14d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest200e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest269e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest26d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest50d_1s4x24d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnest50d_4s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet101d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet10t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet14t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet152d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet18d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet26.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet26d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet32ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet34d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet50_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet51q.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnet61q.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetaa101d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetaa50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetaa50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetblur101d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetblur18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetblur50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetblur50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs270.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs350.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs420.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetrs50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101x1_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101x1_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101x3_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_101x3_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x2_bit_teacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x2_bit_teacher_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x2_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x2_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x4_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_152x4_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50d_evob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50d_evos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50d_frn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50d_gn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50x1_bit_distilled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50x1_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50x1_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50x3_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnetv2_50x3_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/resnext50d_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnet_130.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnet_150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnet_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnetr_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnetr_130.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnetr_150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/rexnetr_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sebotnet33ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sedarknet21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sehalonet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/selecsls42.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/selecsls42b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/selecsls60.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/selecsls60b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/selecsls84.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/semnasnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/semnasnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/semnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/semnasnet_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/semobilevit_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/senet154.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sequencer2d_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sequencer2d_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/sequencer2d_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet152d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet269d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnetaa50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext101d_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext26d_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext26t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext26tn_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/seresnextaa101d_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/skresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/skresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/skresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/skresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/skresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/spnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/ssl_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_base_patch4_window12_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_base_patch4_window12_384_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_base_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_base_patch4_window7_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_large_patch4_window12_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_large_patch4_window12_384_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_large_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_large_patch4_window7_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_s3_base_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_s3_small_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_s3_tiny_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_small_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swin_tiny_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_base_window12_192_22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_base_window12to16_192to256_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_base_window12to24_192to384_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_base_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_base_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_base_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_base_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_base_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_giant_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_giant_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_huge_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_huge_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_large_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_large_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_small_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_small_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_small_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_tiny_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_tiny_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_cr_tiny_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_large_window12_192_22k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_large_window12to16_192to256_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_large_window12to24_192to384_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_small_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_small_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_tiny_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swinv2_tiny_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/swsl_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b0_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b0_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b1_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b1_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b2_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b2_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b3_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b3_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b4_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b4_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b5_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b5_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b6_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b6_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b7_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b7_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_b8_ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_cc_b0_4e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_cc_b0_8e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_cc_b1_8e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_el.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_l2_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_l2_ns_475.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_lite0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_lite1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_lite2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_lite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnet_lite4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_l_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_l_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_m_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_m_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_s_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_s_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_xl_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_efficientnetv2_xl_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mixnet_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mixnet_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mixnet_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_large_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_large_minimal_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tf_mobilenetv3_small_minimal_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tinynet_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tinynet_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tinynet_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tinynet_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tinynet_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tnt_b_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tnt_s_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/tv_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_pcpvt_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_pcpvt_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_pcpvt_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_svt_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_svt_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/twins_svt_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg11_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg13_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg16_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vgg19_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/visformer_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/visformer_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_18x2_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224_miil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_224_sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_plus_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch32_224_sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch32_plus_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch8_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_patch8_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_r26_s32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_r50_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_r50_s16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_r50_s16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_resnet26d_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_resnet50_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_resnet50_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_base_resnet50d_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_giant_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_gigantic_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_huge_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_huge_patch14_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_r50_s32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_r50_s32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_large_r50_s32_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch16_cls_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch16_clsgap_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch16_plus_240.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_base_patch32_plus_rpn_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_cls_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_relpos_small_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_18x2_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_36x1_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_patch8_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_r26_s32_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_r26_s32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_r26_s32_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_resnet26d_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_small_resnet50d_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_srelpos_medium_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_srelpos_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d1_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d1_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d2_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d2_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d3_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d3_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d4_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d4_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d5_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d5_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/volo_d5_512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vovnet39a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/vovnet57a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/wide_resnet101_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/wide_resnet50_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception41.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception41p.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception65.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception65p.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xception71.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_large_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_medium_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_nano_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_small_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/timm/xcit_tiny_24_p8_384_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.403533 mlagility-3.0.2/models/torch_hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/alexnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/convnext_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/convnext_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/convnext_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/convnext_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/dcgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/densenet161.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/densenet169.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/densenet201.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_v2_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_v2_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/efficientnet_v2_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/ghostnet_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/googlenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/hardnet39ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/hardnet68.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/hardnet68ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/hardnet85.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv1_resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_mobilenet_v3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_resnest50_380x380.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mealv2_resnest50_cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/midas_v2.1_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/midas_v3_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/midas_v3_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mnasnet0_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mnasnet0_75.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mnasnet1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mnasnet1_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mobilenet_v3_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/mobilenet_v3_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/proxyless_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/proxyless_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/proxyless_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/proxyless_mobile_14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_16gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_1_6gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_32gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_3_2gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_400mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_800mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_x_8gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_128gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_16gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_1_6gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_32gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_3_2gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_400mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_800mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/regnet_y_8gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest269.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_1s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_1s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_1s4x24d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_2s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_2s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_4s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnest50_fast_4s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet101_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet18_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet18_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet34_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet34_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet50_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnet50_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnext101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/se_resnet101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/shufflenet_v2_x0_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/shufflenet_v2_x1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/shufflenet_v2_x1_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/shufflenet_v2_x2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/squeezenet1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/squeezenet1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/swin_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/swin_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/swin_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg11_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg13_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg16_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vgg19_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vit_b_16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vit_b_32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vit_h_14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vit_l_16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/vit_l_32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/wide_resnet101_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torch_hub/wide_resnet50_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.407534 mlagility-3.0.2/models/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/fasterrcnn_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/fasterrcnn_resnet50_fpn_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/fcos_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/keypointrcnn_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/maskrcnn_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/maskrcnn_resnet50_fpn_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/retinanet_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/retinanet_resnet50_fpn_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/ssd300_vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/torchvision/ssdlite320_mobilenet_v3_large.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.427533 mlagility-3.0.2/models/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bert_for_question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bert_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bert_tiny_for_sequence_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/bigbird_pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/biggan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/blenderbot_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/camembert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/convbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/data2vecaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/data2vectext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/deberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/deit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/deit_base_for_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/deit_tiny_for_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/detr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/detr_for_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/distil_wav2vec2_for_audio_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/distilbert_for_question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/distilhubert_for_audio_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/electra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/electra_for_sequence_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/funnel_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/gpt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/gpt2_doublehead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/ibert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/imagegpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/layoutlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/luke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/m2m_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/marian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/marianmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/megatron_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/minilmv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilebert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilebert_for_sequence_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilevit_small_for_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilevit_x_small_for_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mobilevit_xx_small_for_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mpnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mt5_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mt5_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/mt5_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/openai_doublehead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/perceiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/poolformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/rag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/realm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/rembert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/retribert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/roformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/segformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/sew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/sew_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/speech_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/speech_encoder_decoder_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/speech_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/splinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/squeezebert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/t5_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/t5_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/t5_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/t5_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/unispeech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/unispeech_sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/vision_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/wav2vec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/xglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/xlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/xlm_roberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/xlnet-512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 17:00:56.000000 mlagility-3.0.2/models/transformers/yolos_tiny_for_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 17:00:56.000000 mlagility-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:01:28.443534 mlagility-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-28 17:00:56.000000 mlagility-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.023530 mlagility-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.431534 mlagility-3.0.2/src/mlagility/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.431534 mlagility-3.0.2/src/mlagility/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    18571 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/analysis/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/analysis/tf_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/analysis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.435534 mlagility-3.0.2/src/mlagility/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/execute_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/ortmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/run_ort_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/script_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/setup_ort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/api/trtmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.435534 mlagility-3.0.2/src/mlagility/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16226 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/cli/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.435534 mlagility-3.0.2/src/mlagility/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/common/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/mlagility/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.431534 mlagility-3.0.2/src/mlagility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-28 17:01:27.000000 mlagility-3.0.2/src/mlagility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    89406 2023-04-28 17:01:28.000000 mlagility-3.0.2/src/mlagility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:01:27.000000 mlagility-3.0.2/src/mlagility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 17:01:27.000000 mlagility-3.0.2/src/mlagility.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-28 17:01:27.000000 mlagility-3.0.2/src/mlagility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 17:01:27.000000 mlagility-3.0.2/src/mlagility.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.439534 mlagility-3.0.2/src/onnxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.439534 mlagility-3.0.2/src/onnxflow/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/onnx_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/quantization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/tensor_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/common/tf_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.443534 mlagility-3.0.2/src/onnxflow/justbuildit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5110 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/buildit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/hummingbird.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/justbuildit/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:01:28.443534 mlagility-3.0.2/src/onnxflow/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 17:00:56.000000 mlagility-3.0.2/src/onnxflow/version.py
```

### Comparing `mlagility-3.0.0/LICENSE` & `mlagility-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/PKG-INFO` & `mlagility-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlagility
-Version: 3.0.0
+Version: 3.0.2
 Summary: MLAgility Benchmark and Tools
 Home-page: https://github.com/groq/mlagility
 Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
 Author-email: jfowers@groq.com, dhnoronha@groq.com, rsivakumar@groq.com, vgodsoe@groq.com
 License: MIT
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
```

### Comparing `mlagility-3.0.0/README.md` & `mlagility-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/diffusers/clip_text_encoder.py` & `mlagility-3.0.2/models/diffusers/clip_text_encoder.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/diffusers/safety_clipvision.py` & `mlagility-3.0.2/models/diffusers/safety_clipvision.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/diffusers/unet_2d_condition.py` & `mlagility-3.0.2/models/diffusers/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/diffusers/vae_decoder.py` & `mlagility-3.0.2/models/diffusers/vae_decoder.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/chebconv.py` & `mlagility-3.0.2/models/graph_convolutions/chebconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/dnaconv.py` & `mlagility-3.0.2/models/graph_convolutions/dnaconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/egconv.py` & `mlagility-3.0.2/models/graph_convolutions/egconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/feastconv.py` & `mlagility-3.0.2/models/graph_convolutions/feastconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/gatedgraphconv.py` & `mlagility-3.0.2/models/graph_convolutions/gatedgraphconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/generalconv.py` & `mlagility-3.0.2/models/graph_convolutions/generalconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/leconv.py` & `mlagility-3.0.2/models/graph_convolutions/leconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/pnaconv.py` & `mlagility-3.0.2/models/graph_convolutions/pnaconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/resgatedgraphconv.py` & `mlagility-3.0.2/models/graph_convolutions/resgatedgraphconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/sageconv.py` & `mlagility-3.0.2/models/graph_convolutions/sageconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/graph_convolutions/tagconv.py` & `mlagility-3.0.2/models/graph_convolutions/tagconv.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/0x7194633_keyt5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/0x7194633_keyt5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/AmazonScience_qanlu.py` & `mlagility-3.0.2/models/popular_on_huggingface/AmazonScience_qanlu.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/BM-K_KoSimCSE-roberta.py` & `mlagility-3.0.2/models/popular_on_huggingface/BM-K_KoSimCSE-roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Babelscape_wikineural-multilingual-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/Babelscape_wikineural-multilingual-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Bhuvana_t5-base-spellchecker.py` & `mlagility-3.0.2/models/popular_on_huggingface/Bhuvana_t5-base-spellchecker.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/CompVis_ldm-text2im-large-256.py` & `mlagility-3.0.2/models/popular_on_huggingface/CompVis_ldm-text2im-large-256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/CompVis_stable-diffusion-v1-4.py` & `mlagility-3.0.2/models/popular_on_huggingface/CompVis_stable-diffusion-v1-4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-masakhaner.py` & `mlagility-3.0.2/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-masakhaner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-ner-hrl.py` & `mlagility-3.0.2/models/popular_on_huggingface/Davlan_bert-base-multilingual-cased-ner-hrl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Davlan_distilbert-base-multilingual-cased-ner-hrl.py` & `mlagility-3.0.2/models/popular_on_huggingface/Davlan_distilbert-base-multilingual-cased-ner-hrl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Davlan_xlm-roberta-base-ner-hrl.py` & `mlagility-3.0.2/models/popular_on_huggingface/Davlan_xlm-roberta-base-ner-hrl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Davlan_xlm-roberta-large-ner-hrl.py` & `mlagility-3.0.2/models/popular_on_huggingface/Davlan_xlm-roberta-large-ner-hrl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ElKulako_cryptobert.py` & `mlagility-3.0.2/models/popular_on_huggingface/ElKulako_cryptobert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-base-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-base-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-large-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-large-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Elron_bleurt-tiny-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/Elron_bleurt-tiny-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/FinanceInc_finbert_fls.py` & `mlagility-3.0.2/models/popular_on_huggingface/FinanceInc_finbert_fls.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/HooshvareLab_bert-fa-zwnj-base-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/HooshvareLab_bert-fa-zwnj-base-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/HooshvareLab_distilbert-fa-zwnj-base-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/HooshvareLab_distilbert-fa-zwnj-base-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Huffon_sentence-klue-roberta-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/Huffon_sentence-klue-roberta-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-DeBERTa-v2-710M-Chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-DeBERTa-v2-710M-Chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-NLI.py` & `mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-NLI.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-Sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-110M-Sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Similarity.py` & `mlagility-3.0.2/models/popular_on_huggingface/IDEA-CCNL_Erlangshen-Roberta-330M-Similarity.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IIC_dpr-spanish-passage_encoder-allqa-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/IIC_dpr-spanish-passage_encoder-allqa-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IIC_dpr-spanish-question_encoder-allqa-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/IIC_dpr-spanish-question_encoder-allqa-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IlyaGusev_rubert_telegram_headlines.py` & `mlagility-3.0.2/models/popular_on_huggingface/IlyaGusev_rubert_telegram_headlines.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/IlyaGusev_rut5_base_sum_gazeta.py` & `mlagility-3.0.2/models/popular_on_huggingface/IlyaGusev_rut5_base_sum_gazeta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Intel_dpt-large-ade.py` & `mlagility-3.0.2/models/popular_on_huggingface/Intel_dpt-large-ade.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Intel_dpt-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/Intel_dpt-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_camembert-ner-with-dates.py` & `mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_camembert-ner-with-dates.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_camembert-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_camembert-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Jean-Baptiste_roberta-large-ner-english.py` & `mlagility-3.0.2/models/popular_on_huggingface/Jean-Baptiste_roberta-large-ner-english.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/K024_mt5-zh-ja-en-trimmed.py` & `mlagility-3.0.2/models/popular_on_huggingface/K024_mt5-zh-ja-en-trimmed.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KES_T5-TTParser.py` & `mlagility-3.0.2/models/popular_on_huggingface/KES_T5-TTParser.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KES_TEC-English.py` & `mlagility-3.0.2/models/popular_on_huggingface/KES_TEC-English.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Kamuuung_autonlp-lessons_tagging-606217261.py` & `mlagility-3.0.2/models/popular_on_huggingface/Kamuuung_autonlp-lessons_tagging-606217261.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_bert-base-japanese-upos.py` & `mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_bert-base-japanese-upos.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_bert-large-japanese-wikipedia-ud-head.py` & `mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_bert-large-japanese-wikipedia-ud-head.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_deberta-base-japanese-aozora-ud-head.py` & `mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_deberta-base-japanese-aozora-ud-head.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_deberta-base-thai-ud-head.py` & `mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_deberta-base-thai-ud-head.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/KoichiYasuoka_roberta-base-thai-spm-upos.py` & `mlagility-3.0.2/models/popular_on_huggingface/KoichiYasuoka_roberta-base-thai-spm-upos.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base-finetuned-kinetics.py` & `mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base-finetuned-kinetics.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base-ssv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base-ssv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MCG-NJU_videomae-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/MCG-NJU_videomae-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MaRiOrOsSi_t5-base-finetuned-question-answering.py` & `mlagility-3.0.2/models/popular_on_huggingface/MaRiOrOsSi_t5-base-finetuned-question-answering.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MarcBrun_ixambert-finetuned-squad-eu-en.py` & `mlagility-3.0.2/models/popular_on_huggingface/MarcBrun_ixambert-finetuned-squad-eu-en.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Michau_t5-base-en-generate-headline.py` & `mlagility-3.0.2/models/popular_on_huggingface/Michau_t5-base-en-generate-headline.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-anli.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-anli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-docnli-ling-2c.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-base-mnli-fever-docnli-ling-2c.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-large-mnli-fever-anli-ling-wanli.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-large-mnli-fever-anli-ling-wanli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-xsmall-mnli-fever-anli-ling-binary.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_DeBERTa-v3-xsmall-mnli-fever-anli-ling-binary.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-mnli-xnli.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-mnli-xnli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-xnli-multilingual-nli-2mil7.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_mDeBERTa-v3-base-xnli-multilingual-nli-2mil7.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/MoritzLaurer_policy-distilbert-7d.py` & `mlagility-3.0.2/models/popular_on_huggingface/MoritzLaurer_policy-distilbert-7d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Musixmatch_umberto-commoncrawl-cased-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/Musixmatch_umberto-commoncrawl-cased-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Narrativa_bsc_roberta2roberta_shared-spanish-finetuned-mlsum-summarization.py` & `mlagility-3.0.2/models/popular_on_huggingface/Narrativa_bsc_roberta2roberta_shared-spanish-finetuned-mlsum-summarization.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/NbAiLab_nb-bert-base-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/NbAiLab_nb-bert-base-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/NeuML_bert-small-cord19qa.py` & `mlagility-3.0.2/models/popular_on_huggingface/NeuML_bert-small-cord19qa.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_gpt2-vietnamese.py` & `mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_gpt2-vietnamese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_t5-en-vi-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_t5-en-vi-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/NlpHUST_vibert4news-base-cased.py` & `mlagility-3.0.2/models/popular_on_huggingface/NlpHUST_vibert4news-base-cased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Preetiha_clause_classification.py` & `mlagility-3.0.2/models/popular_on_huggingface/Preetiha_clause_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Recognai_bert-base-spanish-wwm-cased-xnli.py` & `mlagility-3.0.2/models/popular_on_huggingface/Recognai_bert-base-spanish-wwm-cased-xnli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Recognai_zeroshot_selectra_medium.py` & `mlagility-3.0.2/models/popular_on_huggingface/Recognai_zeroshot_selectra_medium.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_t5_xl_bfd.py` & `mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_t5_xl_bfd.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Rostlab_prot_t5_xl_uniref50.py` & `mlagility-3.0.2/models/popular_on_huggingface/Rostlab_prot_t5_xl_uniref50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Sahajtomar_German_Zeroshot.py` & `mlagility-3.0.2/models/popular_on_huggingface/Sahajtomar_German_Zeroshot.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-2B-mono.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-2B-mono.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-2B-multi.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-2B-multi.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-mono.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-mono.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-multi.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-multi.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-350M-nl.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-350M-nl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-6B-mono.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-6B-mono.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codegen-6B-multi.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codegen-6B-multi.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-large-ntp-py.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-large-ntp-py.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_codet5-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_codet5-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Salesforce_mixqg-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/Salesforce_mixqg-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Sehong_t5-large-QuestionGeneration.py` & `mlagility-3.0.2/models/popular_on_huggingface/Sehong_t5-large-QuestionGeneration.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/SenseTime_deformable-detr.py` & `mlagility-3.0.2/models/popular_on_huggingface/SenseTime_deformable-detr.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Sentdex_GPyT.py` & `mlagility-3.0.2/models/popular_on_huggingface/Sentdex_GPyT.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Seznam_small-e-czech.py` & `mlagility-3.0.2/models/popular_on_huggingface/Seznam_small-e-czech.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_roberta_toxicity_classifier.py` & `mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_roberta_toxicity_classifier.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_russian_toxicity_classifier.py` & `mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_russian_toxicity_classifier.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/SkolkovoInstitute_xlmr_formality_classifier.py` & `mlagility-3.0.2/models/popular_on_huggingface/SkolkovoInstitute_xlmr_formality_classifier.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/TristanBehrens_js-fakes-4bars.py` & `mlagility-3.0.2/models/popular_on_huggingface/TristanBehrens_js-fakes-4bars.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/UBC-NLP_AraT5-base-title-generation.py` & `mlagility-3.0.2/models/popular_on_huggingface/UBC-NLP_AraT5-base-title-generation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Unbabel_gec-t5_small.py` & `mlagility-3.0.2/models/popular_on_huggingface/Unbabel_gec-t5_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Visual-Attention-Network_van-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/Visual-Attention-Network_van-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Visual-Attention-Network_van-tiny.py` & `mlagility-3.0.2/models/popular_on_huggingface/Visual-Attention-Network_van-tiny.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/Wikidepia_IndoT5-base-paraphrase.py` & `mlagility-3.0.2/models/popular_on_huggingface/Wikidepia_IndoT5-base-paraphrase.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/abhishek_autonlp-bbc-news-classification-37229289.py` & `mlagility-3.0.2/models/popular_on_huggingface/abhishek_autonlp-bbc-news-classification-37229289.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ahmedrachid_FinancialBERT-Sentiment-Analysis.py` & `mlagility-3.0.2/models/popular_on_huggingface/ahmedrachid_FinancialBERT-Sentiment-Analysis.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ai4bharat_IndicBART.py` & `mlagility-3.0.2/models/popular_on_huggingface/ai4bharat_IndicBART.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ai4bharat_IndicBARTSS.py` & `mlagility-3.0.2/models/popular_on_huggingface/ai4bharat_IndicBARTSS.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-base-cased.py` & `mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-base-cased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/allegro_herbert-large-cased.py` & `mlagility-3.0.2/models/popular_on_huggingface/allegro_herbert-large-cased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/allenai_t5-small-next-word-generator-qoogle.py` & `mlagility-3.0.2/models/popular_on_huggingface/allenai_t5-small-next-word-generator-qoogle.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/allenai_t5-small-squad2-question-generation.py` & `mlagility-3.0.2/models/popular_on_huggingface/allenai_t5-small-squad2-question-generation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/aneuraz_awesome-align-with-co.py` & `mlagility-3.0.2/models/popular_on_huggingface/aneuraz_awesome-align-with-co.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/apple_deeplabv3-mobilevit-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/apple_deeplabv3-mobilevit-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/apple_deeplabv3-mobilevit-xx-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/apple_deeplabv3-mobilevit-xx-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/apple_mobilevit-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/apple_mobilevit-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/apple_mobilevit-xx-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/apple_mobilevit-xx-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/asi_gpt-fr-cased-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/asi_gpt-fr-cased-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/assemblyai_bert-large-uncased-sst2.py` & `mlagility-3.0.2/models/popular_on_huggingface/assemblyai_bert-large-uncased-sst2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/aubmindlab_araelectra-base-discriminator.py` & `mlagility-3.0.2/models/popular_on_huggingface/aubmindlab_araelectra-base-discriminator.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/aujer_ni_model_8_19.py` & `mlagility-3.0.2/models/popular_on_huggingface/aujer_ni_model_8_19.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/aware-ai_bart-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/aware-ai_bart-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/azwierzc_herbert-large-poquad.py` & `mlagility-3.0.2/models/popular_on_huggingface/azwierzc_herbert-large-poquad.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/azwierzc_plt5-base-poquad.py` & `mlagility-3.0.2/models/popular_on_huggingface/azwierzc_plt5-base-poquad.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/azwierzc_plt5-large-poquad.py` & `mlagility-3.0.2/models/popular_on_huggingface/azwierzc_plt5-large-poquad.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/batterydata_batterybert-cased-squad-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/batterydata_batterybert-cased-squad-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-bert-base-aihub-mrc.py` & `mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-bert-base-aihub-mrc.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bespin-global_klue-bert-base-mrc.py` & `mlagility-3.0.2/models/popular_on_huggingface/bespin-global_klue-bert-base-mrc.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_bert-base-uncased-emotion.py` & `mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_bert-base-uncased-emotion.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_distilbert-base-uncased-emotion.py` & `mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_distilbert-base-uncased-emotion.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_electra-base-emotion.py` & `mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_electra-base-emotion.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bhadresh-savani_roberta-base-emotion.py` & `mlagility-3.0.2/models/popular_on_huggingface/bhadresh-savani_roberta-base-emotion.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bigscience_T0.py` & `mlagility-3.0.2/models/popular_on_huggingface/bigscience_T0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/bigscience_T0p.py` & `mlagility-3.0.2/models/popular_on_huggingface/bigscience_T0p.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/blinoff_roberta-base-russian-v0.py` & `mlagility-3.0.2/models/popular_on_huggingface/blinoff_roberta-base-russian-v0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-multi.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-multi.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-single.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_tweet-topic-21-single.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emoji.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emoji.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emotion.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-emotion.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-hate.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-hate.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-irony.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-irony.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-offensive.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-offensive.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/cardiffnlp_twitter-roberta-base-sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/chkla_parlbert-topic-german.py` & `mlagility-3.0.2/models/popular_on_huggingface/chkla_parlbert-topic-german.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/clips_mfaq.py` & `mlagility-3.0.2/models/popular_on_huggingface/clips_mfaq.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-nli.py` & `mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-nli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-qa.py` & `mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-qa.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cmarkea_distilcamembert-base-sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/cmarkea_distilcamembert-base-sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_LaBSE-en-ru.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_LaBSE-en-ru.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-base-cased-nli-threeway.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-base-cased-nli-threeway.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny-sentiment-balanced.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny-sentiment-balanced.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny-toxicity.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny-toxicity.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rubert-tiny2.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rubert-tiny2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rut5-small-chitchat.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rut5-small-chitchat.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cointegrated_rut5-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/cointegrated_rut5-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-MiniLM2-L6-H768.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-MiniLM2-L6-H768.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-xsmall.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-deberta-v3-xsmall.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-distilroberta-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-distilroberta-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/cross-encoder_nli-roberta-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/cross-encoder_nli-roberta-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2m_crossSum.py` & `mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2m_crossSum.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2o_arabic_crossSum.py` & `mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2o_arabic_crossSum.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_m2o_chinese_simplified_crossSum.py` & `mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_m2o_chinese_simplified_crossSum.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/csebuetnlp_mT5_multilingual_XLSum.py` & `mlagility-3.0.2/models/popular_on_huggingface/csebuetnlp_mT5_multilingual_XLSum.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ctrl.py` & `mlagility-3.0.2/models/popular_on_huggingface/ctrl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/d4data_biomedical-ner-all.py` & `mlagility-3.0.2/models/popular_on_huggingface/d4data_biomedical-ner-all.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-nlvr2.py` & `mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-nlvr2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-vqa.py` & `mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-finetuned-vqa.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dandelin_vilt-b32-mlm.py` & `mlagility-3.0.2/models/popular_on_huggingface/dandelin_vilt-b32-mlm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dangvantuan_sentence-camembert-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/dangvantuan_sentence-camembert-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dangvantuan_sentence-camembert-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/dangvantuan_sentence-camembert-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_deberta-v3-base-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_deberta-v3-base-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_deberta-v3-large-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_deberta-v3-large-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_electra-base-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_electra-base-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_roberta-base-squad2-covid.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_roberta-base-squad2-covid.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_roberta-base-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_roberta-base-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_tinyroberta-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_tinyroberta-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_xlm-roberta-base-squad2-distilled.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_xlm-roberta-base-squad2-distilled.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deepset_xlm-roberta-large-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deepset_xlm-roberta-large-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deutsche-telekom_bert-multi-english-german-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deutsche-telekom_bert-multi-english-german-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/deutsche-telekom_electra-base-de-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/deutsche-telekom_electra-base-de-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert-v2.py` & `mlagility-3.0.2/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert-v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert.py` & `mlagility-3.0.2/models/popular_on_huggingface/digitalepidemiologylab_covid-twitter-bert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/distilbert-base-uncased-finetuned-sst-2-english.py` & `mlagility-3.0.2/models/popular_on_huggingface/distilbert-base-uncased-finetuned-sst-2-english.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dkleczek_bert-base-polish-cased-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/dkleczek_bert-base-polish-cased-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dkleczek_bert-base-polish-uncased-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/dkleczek_bert-base-polish-uncased-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/doc2query_all-t5-base-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/doc2query_all-t5-base-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/doc2query_all-with_prefix-t5-base-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/doc2query_all-with_prefix-t5-base-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/doc2query_msmarco-t5-base-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/doc2query_msmarco-t5-base-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dslim_bert-base-NER.py` & `mlagility-3.0.2/models/popular_on_huggingface/dslim_bert-base-NER.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dslim_bert-large-NER.py` & `mlagility-3.0.2/models/popular_on_huggingface/dslim_bert-large-NER.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/dumitrescustefan_bert-base-romanian-cased-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/dumitrescustefan_bert-base-romanian-cased-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/edumunozsala_beto_sentiment_analysis_es.py` & `mlagility-3.0.2/models/popular_on_huggingface/edumunozsala_beto_sentiment_analysis_es.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/edumunozsala_vit_base-224-in21k-ft-cifar100.py` & `mlagility-3.0.2/models/popular_on_huggingface/edumunozsala_vit_base-224-in21k-ft-cifar100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ehdwns1516_klue-roberta-base-kornli.py` & `mlagility-3.0.2/models/popular_on_huggingface/ehdwns1516_klue-roberta-base-kornli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/esiebomajeremiah_autonlp-email-classification-657119381.py` & `mlagility-3.0.2/models/popular_on_huggingface/esiebomajeremiah_autonlp-email-classification-657119381.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_camembert-base-squadFR-fquad-piaf.py` & `mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_camembert-base-squadFR-fquad-piaf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_dpr-ctx_encoder-fr_qa-camembert.py` & `mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_dpr-ctx_encoder-fr_qa-camembert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/etalab-ia_dpr-question_encoder-fr_qa-camembert.py` & `mlagility-3.0.2/models/popular_on_huggingface/etalab-ia_dpr-question_encoder-fr_qa-camembert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/fabiochiu_t5-base-tag-generation.py` & `mlagility-3.0.2/models/popular_on_huggingface/fabiochiu_t5-base-tag-generation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_contriever-msmarco.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_contriever-msmarco.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_contriever.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_contriever.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-base-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-base-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-base-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-base-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-large-224-22k-1k.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-large-224-22k-1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-small-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-small-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-tiny-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-tiny-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-xlarge-224-22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-xlarge-224-22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_convnext-xlarge-384-22k-1k.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_convnext-xlarge-384-22k-1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_data2vec-vision-base-ft1k.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_data2vec-vision-base-ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-distilled-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-base-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-base-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-small-distilled-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-small-distilled-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-small-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-small-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-tiny-distilled-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-tiny-distilled-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_deit-tiny-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_deit-tiny-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_detr-resnet-50-panoptic.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_detr-resnet-50-panoptic.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_detr-resnet-50.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_detr-resnet-50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vitb16.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vitb16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vitb8.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vitb8.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vits16.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vits16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_dino-vits8.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_dino-vits8.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_flava-full.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_flava-full.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_levit-128S.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_levit-128S.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-base-ade.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-base-ade.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-base-coco.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-base-coco.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-large-ade.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-large-ade.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-small-coco.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-small-coco.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_maskformer-swin-tiny-ade.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_maskformer-swin-tiny-ade.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_mbart-large-50.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_mbart-large-50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_regnet-y-040.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_regnet-y-040.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_vit-mae-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_vit-mae-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/facebook_vit-mae-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/facebook_vit-mae-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-community_clip-rsicd-v2.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-community_clip-rsicd-v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-community_t5-large-wikisplit.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-community_t5-large-wikisplit.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_roberta-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v3_roberta-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v4_MiniLM-L6.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_all_datasets_v4_MiniLM-L6.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_st-codesearch-distilroberta-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_st-codesearch-distilroberta-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flax-sentence-embeddings_stackoverflow_mpnet-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/flax-sentence-embeddings_stackoverflow_mpnet-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flexudy_t5-base-multi-sentence-doctor.py` & `mlagility-3.0.2/models/popular_on_huggingface/flexudy_t5-base-multi-sentence-doctor.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/flexudy_t5-small-wav2vec2-grammar-fixer.py` & `mlagility-3.0.2/models/popular_on_huggingface/flexudy_t5-small-wav2vec2-grammar-fixer.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/fran-martinez_scibert_scivocab_cased_ner_jnlpba.py` & `mlagility-3.0.2/models/popular_on_huggingface/fran-martinez_scibert_scivocab_cased_ner_jnlpba.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/gerulata_slovakbert.py` & `mlagility-3.0.2/models/popular_on_huggingface/gerulata_slovakbert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/gilf_french-camembert-postag-model.py` & `mlagility-3.0.2/models/popular_on_huggingface/gilf_french-camembert-postag-model.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/gilf_french-postag-model.py` & `mlagility-3.0.2/models/popular_on_huggingface/gilf_french-postag-model.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_bert2bert_L-24_wmt_de_en.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_bert2bert_L-24_wmt_de_en.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_byt5-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_byt5-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_byt5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_byt5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_byt5-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_byt5-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_canine-c.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_canine-c.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_canine-s.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_canine-s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_ddpm-celebahq-256.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_ddpm-celebahq-256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_ddpm-cifar10-32.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_ddpm-cifar10-32.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_electra-base-discriminator.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_electra-base-discriminator.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_electra-large-discriminator.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_electra-large-discriminator.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_electra-small-discriminator.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_electra-small-discriminator.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-base-patch16.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-base-patch16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-base-patch32.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-base-patch32.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_owlvit-large-patch14.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_owlvit-large-patch14.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_bbc.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_bbc.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_cnn_daily_mail.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_cnn_daily_mail.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_roberta2roberta_L-24_discofuse.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_roberta2roberta_L-24_discofuse.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_t5-small-ssm-nq.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_t5-small-ssm-nq.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-224-in21k.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-224-in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch32-224-in21k.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch32-224-in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-base-patch32-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-base-patch32-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-huge-patch14-224-in21k.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-huge-patch14-224-in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-224-in21k.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-224-in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch32-224-in21k.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch32-224-in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/google_vit-large-patch32-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/google_vit-large-patch32-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hakurei_lit-6B.py` & `mlagility-3.0.2/models/popular_on_huggingface/hakurei_lit-6B.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-dutch-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-dutch-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-polish-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/henryk_bert-base-multilingual-cased-finetuned-polish-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hetpandya_t5-base-tapaco.py` & `mlagility-3.0.2/models/popular_on_huggingface/hetpandya_t5-base-tapaco.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hetpandya_t5-small-tapaco.py` & `mlagility-3.0.2/models/popular_on_huggingface/hetpandya_t5-small-tapaco.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/hustvl_yolos-tiny.py` & `mlagility-3.0.2/models/popular_on_huggingface/hustvl_yolos-tiny.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/imranraad_idiom-xlm-roberta.py` & `mlagility-3.0.2/models/popular_on_huggingface/imranraad_idiom-xlm-roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/inkoziev_rugpt_chitchat.py` & `mlagility-3.0.2/models/popular_on_huggingface/inkoziev_rugpt_chitchat.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/intfloat_simlm-msmarco-reranker.py` & `mlagility-3.0.2/models/popular_on_huggingface/intfloat_simlm-msmarco-reranker.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/jaehyeong_koelectra-base-v3-generalized-sentiment-analysis.py` & `mlagility-3.0.2/models/popular_on_huggingface/jaehyeong_koelectra-base-v3-generalized-sentiment-analysis.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/joeddav_bart-large-mnli-yahoo-answers.py` & `mlagility-3.0.2/models/popular_on_huggingface/joeddav_bart-large-mnli-yahoo-answers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/johngiorgi_declutr-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/johngiorgi_declutr-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/johngiorgi_declutr-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/johngiorgi_declutr-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/jsylee_scibert_scivocab_uncased-finetuned-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/jsylee_scibert_scivocab_uncased-finetuned-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_base.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_base.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_ft_base.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_chinese_sim_char_ft_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_base.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_large.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_small.py` & `mlagility-3.0.2/models/popular_on_huggingface/junnyu_roformer_v2_chinese_char_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc-lt.py` & `mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc-lt.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc.py` & `mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed-pmc.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed.py` & `mlagility-3.0.2/models/popular_on_huggingface/kamalkraj_bioelectra-base-discriminator-pubmed.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ken11_albert-base-japanese-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/ken11_albert-base-japanese-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/kiheh85202_yolo.py` & `mlagility-3.0.2/models/popular_on_huggingface/kiheh85202_yolo.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/laituan245_molt5-large-smiles2caption.py` & `mlagility-3.0.2/models/popular_on_huggingface/laituan245_molt5-large-smiles2caption.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/lcw99_t5-base-korean-chit-chat.py` & `mlagility-3.0.2/models/popular_on_huggingface/lcw99_t5-base-korean-chit-chat.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/liandarizkia_SA01-IndoBert.py` & `mlagility-3.0.2/models/popular_on_huggingface/liandarizkia_SA01-IndoBert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/madhurjindal_autonlp-Gibberish-Detector-492513457.py` & `mlagility-3.0.2/models/popular_on_huggingface/madhurjindal_autonlp-Gibberish-Detector-492513457.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/malteos_scincl.py` & `mlagility-3.0.2/models/popular_on_huggingface/malteos_scincl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/marefa-nlp_marefa-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/marefa-nlp_marefa-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mdhugol_indonesia-bert-sentiment-classification.py` & `mlagility-3.0.2/models/popular_on_huggingface/mdhugol_indonesia-bert-sentiment-classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/melll-uff_bertweetbr.py` & `mlagility-3.0.2/models/popular_on_huggingface/melll-uff_bertweetbr.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_BiomedVLP-CXR-BERT-specialized.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_BiomedVLP-CXR-BERT-specialized.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k-ft22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k-ft22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224-pt22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-base-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-base-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k-ft22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k-ft22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-224-pt22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_beit-large-patch16-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_beit-large-patch16-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_conditional-detr-resnet-50.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_conditional-detr-resnet-50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_cvt-13.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_cvt-13.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_prophetnet-large-uncased.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_prophetnet-large-uncased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-101.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-101.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-152.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-152.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-18.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-18.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-34.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-34.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_resnet-50.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_resnet-50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384-in22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384-in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window12-384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224-in22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224-in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-base-patch4-window7-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window12-384-in22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window12-384-in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224-in22k.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224-in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-large-patch4-window7-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-small-patch4-window7-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-small-patch4-window7-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swin-tiny-patch4-window7-224.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swin-tiny-patch4-window7-224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_swinv2-tiny-patch4-window8-256.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_swinv2-tiny-patch4-window8-256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_tapex-large-finetuned-tabfact.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_tapex-large-finetuned-tabfact.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-base-handwritten.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-base-handwritten.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-base-printed.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-base-printed.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-handwritten.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-handwritten.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-printed.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-printed.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-large-str.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-large-str.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-small-handwritten.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-small-handwritten.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_trocr-small-stage1.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_trocr-small-stage1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/microsoft_xprophetnet-large-wiki100-cased.py` & `mlagility-3.0.2/models/popular_on_huggingface/microsoft_xprophetnet-large-wiki100-cased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ml4pubmed_BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext_pub_section.py` & `mlagility-3.0.2/models/popular_on_huggingface/ml4pubmed_BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext_pub_section.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ml6team_bert-base-uncased-city-country-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/ml6team_bert-base-uncased-city-country-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ml6team_distilbert-base-german-cased-toxic-comments.py` & `mlagility-3.0.2/models/popular_on_huggingface/ml6team_distilbert-base-german-cased-toxic-comments.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/model-attribution-challenge_codegen-350M-multi.py` & `mlagility-3.0.2/models/popular_on_huggingface/model-attribution-challenge_codegen-350M-multi.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/monilouise_ner_news_portuguese.py` & `mlagility-3.0.2/models/popular_on_huggingface/monilouise_ner_news_portuguese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_TinyBERT-spanish-uncased-finetuned-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_TinyBERT-spanish-uncased-finetuned-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-italian-finedtuned-squadv1-it-alfa.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-italian-finedtuned-squadv1-it-alfa.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-medium-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-medium-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-multi-cased-finetuned-xquadv1.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-multi-cased-finetuned-xquadv1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-small-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-small-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-small2bert-small-finetuned-cnn_daily_mail-summarization.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-small2bert-small-finetuned-cnn_daily_mail-summarization.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-spanish-cased-finetuned-ner.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-spanish-cased-finetuned-ner.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-tiny-5-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-tiny-5-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert-tiny-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert-tiny-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-german-finetuned-summarization.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-german-finetuned-summarization.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-spanish-finetuned-summarization.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-spanish-finetuned-summarization.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_bert2bert_shared-turkish-summarization.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_bert2bert_shared-turkish-summarization.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_codebert-base-finetuned-detect-insecure-code.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_codebert-base-finetuned-detect-insecure-code.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_distill-bert-base-spanish-wwm-cased-finetuned-spa-squad2-es.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_distill-bert-base-spanish-wwm-cased-finetuned-spa-squad2-es.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_electra-small-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_electra-small-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_electricidad-base-discriminator.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_electricidad-base-discriminator.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_roberta-base-1B-1-finetuned-squadv1.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_roberta-base-1B-1-finetuned-squadv1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_spanbert-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_spanbert-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_spanbert-large-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_spanbert-large-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-common_gen.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-common_gen.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-e2m-intent.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-e2m-intent.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-imdb-sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-imdb-sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-quartz.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-quartz.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-question-generation-ap.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-question-generation-ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-span-sentiment-extraction.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-span-sentiment-extraction.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-squadv2.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-squadv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-base-finetuned-wikiSQL.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-base-finetuned-wikiSQL.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/mrm8488_t5-small-finetuned-quora-for-paraphrasing.py` & `mlagility-3.0.2/models/popular_on_huggingface/mrm8488_t5-small-finetuned-quora-for-paraphrasing.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nateraw_vit-age-classifier.py` & `mlagility-3.0.2/models/popular_on_huggingface/nateraw_vit-age-classifier.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nateraw_vit-base-patch16-224-cifar10.py` & `mlagility-3.0.2/models/popular_on_huggingface/nateraw_vit-base-patch16-224-cifar10.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/navteca_bart-large-mnli.py` & `mlagility-3.0.2/models/popular_on_huggingface/navteca_bart-large-mnli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/navteca_nli-deberta-v3-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/navteca_nli-deberta-v3-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/navteca_roberta-base-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/navteca_roberta-base-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/navteca_roberta-large-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/navteca_roberta-large-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nbroad_mt5-base-qgen.py` & `mlagility-3.0.2/models/popular_on_huggingface/nbroad_mt5-base-qgen.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/neuralspace-reverie_indic-transformers-bn-distilbert.py` & `mlagility-3.0.2/models/popular_on_huggingface/neuralspace-reverie_indic-transformers-bn-distilbert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/neuraly_bert-base-italian-cased-sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/neuraly_bert-base-italian-cased-sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/neuropark_sahajBERT.py` & `mlagility-3.0.2/models/popular_on_huggingface/neuropark_sahajBERT.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nickmuchi_yolos-small-rego-plates-detection.py` & `mlagility-3.0.2/models/popular_on_huggingface/nickmuchi_yolos-small-rego-plates-detection.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nkoh01_MSRoberta.py` & `mlagility-3.0.2/models/popular_on_huggingface/nkoh01_MSRoberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_groupvit-gcc-yfcc.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_groupvit-gcc-yfcc.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b1.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b2.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b3.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b4.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_mit-b5.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_mit-b5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-ade-512-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-ade-512-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-1024-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-1024-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-512-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-512-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-768-768.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b0-finetuned-cityscapes-768-768.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b1-finetuned-ade-512-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b1-finetuned-ade-512-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b2-finetuned-cityscapes-1024-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b2-finetuned-cityscapes-1024-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-ade-512-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-ade-512-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-cityscapes-1024-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b3-finetuned-cityscapes-1024-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-ade-512-512.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-ade-512-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-cityscapes-1024-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b4-finetuned-cityscapes-1024-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/nvidia_segformer-b5-finetuned-cityscapes-1024-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/nvidia_segformer-b5-finetuned-cityscapes-1024-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-base-patch16.py` & `mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-base-patch16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-base-patch32.py` & `mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-base-patch32.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/openai_clip-vit-large-patch14.py` & `mlagility-3.0.2/models/popular_on_huggingface/openai_clip-vit-large-patch14.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/patrickvonplaten_longformer2roberta-cnn_dailymail-fp16.py` & `mlagility-3.0.2/models/popular_on_huggingface/patrickvonplaten_longformer2roberta-cnn_dailymail-fp16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/paust_pko-t5-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/paust_pko-t5-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/paust_pko-t5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/paust_pko-t5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/persiannlp_mt5-large-parsinlu-arc-comqa-obqa-multiple-choice.py` & `mlagility-3.0.2/models/popular_on_huggingface/persiannlp_mt5-large-parsinlu-arc-comqa-obqa-multiple-choice.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-conll2003.py` & `mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-conll2003.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-3-class.py` & `mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-3-class.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-4-class.py` & `mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann-conll2003-4-class.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann.py` & `mlagility-3.0.2/models/popular_on_huggingface/philschmid_distilroberta-base-ner-wikiann.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/phiyodr_bart-large-finetuned-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/phiyodr_bart-large-finetuned-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/phiyodr_bert-base-finetuned-squad2.py` & `mlagility-3.0.2/models/popular_on_huggingface/phiyodr_bert-base-finetuned-squad2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/phpaiola_ptt5-base-summ-cstnews.py` & `mlagility-3.0.2/models/popular_on_huggingface/phpaiola_ptt5-base-summ-cstnews.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/pierreguillou_ner-bert-large-cased-pt-lenerbr.py` & `mlagility-3.0.2/models/popular_on_huggingface/pierreguillou_ner-bert-large-cased-pt-lenerbr.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/pin_senda.py` & `mlagility-3.0.2/models/popular_on_huggingface/pin_senda.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/projecte-aina_roberta-base-ca-v2.py` & `mlagility-3.0.2/models/popular_on_huggingface/projecte-aina_roberta-base-ca-v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/pvl_labse_bert.py` & `mlagility-3.0.2/models/popular_on_huggingface/pvl_labse_bert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/racai_distilbert-base-romanian-uncased.py` & `mlagility-3.0.2/models/popular_on_huggingface/racai_distilbert-base-romanian-uncased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ramsrigouthamg_t5-large-paraphraser-diverse-high-quality.py` & `mlagility-3.0.2/models/popular_on_huggingface/ramsrigouthamg_t5-large-paraphraser-diverse-high-quality.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ramsrigouthamg_t5_paraphraser.py` & `mlagility-3.0.2/models/popular_on_huggingface/ramsrigouthamg_t5_paraphraser.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoBERT-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoBERT-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoBERT-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoBERT-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoGPT2-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoGPT2-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/readerbench_RoGPT2-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/readerbench_RoGPT2-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/readerbench_jurBERT-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/readerbench_jurBERT-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-lid-lince.py` & `mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-lid-lince.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-ner-lince.py` & `mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-ner-lince.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-pos-lince.py` & `mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-hineng-pos-lince.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sagorsarker_codeswitch-spaeng-sentiment-analysis-lince.py` & `mlagility-3.0.2/models/popular_on_huggingface/sagorsarker_codeswitch-spaeng-sentiment-analysis-lince.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sail_poolformer_s12.py` & `mlagility-3.0.2/models/popular_on_huggingface/sail_poolformer_s12.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/salesken_natural_rephrase.py` & `mlagility-3.0.2/models/popular_on_huggingface/salesken_natural_rephrase.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/salesken_paraphrase_diversity_ranker.py` & `mlagility-3.0.2/models/popular_on_huggingface/salesken_paraphrase_diversity_ranker.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/salesken_paraphrase_generation.py` & `mlagility-3.0.2/models/popular_on_huggingface/salesken_paraphrase_generation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/salesken_text_generate.py` & `mlagility-3.0.2/models/popular_on_huggingface/salesken_text_generate.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sampathkethineedi_industry-classification.py` & `mlagility-3.0.2/models/popular_on_huggingface/sampathkethineedi_industry-classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/savasy_bert-base-turkish-sentiment-cased.py` & `mlagility-3.0.2/models/popular_on_huggingface/savasy_bert-base-turkish-sentiment-cased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sberbank-ai_sbert_large_mt_nlu_ru.py` & `mlagility-3.0.2/models/popular_on_huggingface/sberbank-ai_sbert_large_mt_nlu_ru.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sberbank-ai_sbert_large_nlu_ru.py` & `mlagility-3.0.2/models/popular_on_huggingface/sberbank-ai_sbert_large_nlu_ru.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_clip-ViT-B-32-multilingual-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_clip-ViT-B-32-multilingual-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L6-cos-v5.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-MiniLM-L6-cos-v5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-bert-base-dot-v5.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-bert-base-dot-v5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-tas-b.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-base-tas-b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-cos-v5.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-cos-v5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-dot-v5.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_msmarco-distilbert-dot-v5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-cos-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-cos-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-dot-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-MiniLM-L6-dot-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-distilbert-cos-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-distilbert-cos-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-cos-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-cos-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-dot-v1.py` & `mlagility-3.0.2/models/popular_on_huggingface/sentence-transformers_multi-qa-mpnet-base-dot-v1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/setu4993_LaBSE.py` & `mlagility-3.0.2/models/popular_on_huggingface/setu4993_LaBSE.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/setu4993_smaller-LaBSE.py` & `mlagility-3.0.2/models/popular_on_huggingface/setu4993_smaller-LaBSE.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/soheeyang_rdr-question_encoder-single-nq-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/soheeyang_rdr-question_encoder-single-nq-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/squirro_albert-base-v2-squad_v2.py` & `mlagility-3.0.2/models/popular_on_huggingface/squirro_albert-base-v2-squad_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/strombergnlp_dant5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/strombergnlp_dant5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/svalabs_gbert-large-zeroshot-nli.py` & `mlagility-3.0.2/models/popular_on_huggingface/svalabs_gbert-large-zeroshot-nli.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/t5-base.py` & `mlagility-3.0.2/models/popular_on_huggingface/t5-base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/t5-large.py` & `mlagility-3.0.2/models/popular_on_huggingface/t5-large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/t5-small.py` & `mlagility-3.0.2/models/popular_on_huggingface/t5-small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/taeminlee_kogpt2.py` & `mlagility-3.0.2/models/popular_on_huggingface/taeminlee_kogpt2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/tartuNLP_EstBERT_NER.py` & `mlagility-3.0.2/models/popular_on_huggingface/tartuNLP_EstBERT_NER.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/tdobrxl_ClinicBERT.py` & `mlagility-3.0.2/models/popular_on_huggingface/tdobrxl_ClinicBERT.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/thanathorn_mt5-cpe-kmutt-thai-sentence-sum.py` & `mlagility-3.0.2/models/popular_on_huggingface/thanathorn_mt5-cpe-kmutt-thai-sentence-sum.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/tugstugi_bert-large-mongolian-uncased.py` & `mlagility-3.0.2/models/popular_on_huggingface/tugstugi_bert-large-mongolian-uncased.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-chinese-extractive-qa.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-chinese-extractive-qa.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-chinanews-chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-chinanews-chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-cluener2020-chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-cluener2020-chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-dianping-chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-dianping-chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-binary-chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-binary-chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-full-chinese.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_roberta-base-finetuned-jd-full-chinese.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_t5-base-chinese-cluecorpussmall.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_t5-base-chinese-cluecorpussmall.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_t5-small-chinese-cluecorpussmall.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_t5-small-chinese-cluecorpussmall.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_t5-v1_1-base-chinese-cluecorpussmall.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_t5-v1_1-base-chinese-cluecorpussmall.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/uer_t5-v1_1-small-chinese-cluecorpussmall.py` & `mlagility-3.0.2/models/popular_on_huggingface/uer_t5-v1_1-small-chinese-cluecorpussmall.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/unitary_multilingual-toxic-xlm-roberta.py` & `mlagility-3.0.2/models/popular_on_huggingface/unitary_multilingual-toxic-xlm-roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/unitary_toxic-bert.py` & `mlagility-3.0.2/models/popular_on_huggingface/unitary_toxic-bert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/unitary_unbiased-toxic-roberta.py` & `mlagility-3.0.2/models/popular_on_huggingface/unitary_unbiased-toxic-roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ushikado_yuyuyui-chatbot.py` & `mlagility-3.0.2/models/popular_on_huggingface/ushikado_yuyuyui-chatbot.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/valhalla_bart-large-finetuned-squadv1.py` & `mlagility-3.0.2/models/popular_on_huggingface/valhalla_bart-large-finetuned-squadv1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/valhalla_t5-base-squad.py` & `mlagility-3.0.2/models/popular_on_huggingface/valhalla_t5-base-squad.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/vblagoje_dpr-ctx_encoder-single-lfqa-wiki.py` & `mlagility-3.0.2/models/popular_on_huggingface/vblagoje_dpr-ctx_encoder-single-lfqa-wiki.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/vinvino02_glpn-kitti.py` & `mlagility-3.0.2/models/popular_on_huggingface/vinvino02_glpn-kitti.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/vinvino02_glpn-nyu.py` & `mlagility-3.0.2/models/popular_on_huggingface/vinvino02_glpn-nyu.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_base.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_large.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_small.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_albert_chinese_tiny.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_albert_chinese_tiny.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_dpr-ctx_encoder-bert-base-multilingual.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_dpr-ctx_encoder-bert-base-multilingual.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/voidful_dpr-question_encoder-bert-base-multilingual.py` & `mlagility-3.0.2/models/popular_on_huggingface/voidful_dpr-question_encoder-bert-base-multilingual.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/wanyu_IteraTeR-ROBERTA-Intention-Classifier.py` & `mlagility-3.0.2/models/popular_on_huggingface/wanyu_IteraTeR-ROBERTA-Intention-Classifier.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/wonrax_phobert-base-vietnamese-sentiment.py` & `mlagility-3.0.2/models/popular_on_huggingface/wonrax_phobert-base-vietnamese-sentiment.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/xlm-clm-ende-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/xlm-clm-ende-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/xlm-clm-enfr-1024.py` & `mlagility-3.0.2/models/popular_on_huggingface/xlm-clm-enfr-1024.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/xlm-roberta-large-finetuned-conll03-german.py` & `mlagility-3.0.2/models/popular_on_huggingface/xlm-roberta-large-finetuned-conll03-german.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ybelkada_japanese-roberta-question-answering.py` & `mlagility-3.0.2/models/popular_on_huggingface/ybelkada_japanese-roberta-question-answering.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ydshieh_roberta-large-ner-english.py` & `mlagility-3.0.2/models/popular_on_huggingface/ydshieh_roberta-large-ner-english.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/ydshieh_vit-gpt2-coco-en.py` & `mlagility-3.0.2/models/popular_on_huggingface/ydshieh_vit-gpt2-coco-en.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-esg.py` & `mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-esg.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-fls.py` & `mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-fls.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/popular_on_huggingface/yiyanghkust_finbert-tone.py` & `mlagility-3.0.2/models/popular_on_huggingface/yiyanghkust_finbert-tone.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/selftest/linear.py` & `mlagility-3.0.2/models/selftest/linear.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/selftest/twolayer.py` & `mlagility-3.0.2/models/selftest/twolayer.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_base_patch16_224.py` & `mlagility-3.0.2/models/timm/beit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_base_patch16_224_in22k.py` & `mlagility-3.0.2/models/timm/beit_base_patch16_224_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_base_patch16_384.py` & `mlagility-3.0.2/models/timm/beit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_large_patch16_224.py` & `mlagility-3.0.2/models/timm/beit_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_large_patch16_224_in22k.py` & `mlagility-3.0.2/models/timm/beit_large_patch16_224_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_large_patch16_384.py` & `mlagility-3.0.2/models/timm/beit_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/beit_large_patch16_512.py` & `mlagility-3.0.2/models/timm/beit_large_patch16_512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convmixer_1024_20_ks9_p14.py` & `mlagility-3.0.2/models/timm/convmixer_1024_20_ks9_p14.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convmixer_1536_20.py` & `mlagility-3.0.2/models/timm/convmixer_1536_20.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_base_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_base_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_base_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_base_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_base_in22k.py` & `mlagility-3.0.2/models/timm/convnext_base_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_large_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_large_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_large_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_large_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_large_in22k.py` & `mlagility-3.0.2/models/timm/convnext_large_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_nano_hnf.py` & `mlagility-3.0.2/models/timm/convnext_nano_hnf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_nano_ols.py` & `mlagility-3.0.2/models/timm/convnext_nano_ols.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_small_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_small_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_small_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_small_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_small_in22k.py` & `mlagility-3.0.2/models/timm/convnext_small_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_tiny_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_tiny_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_tiny_hnf.py` & `mlagility-3.0.2/models/timm/convnext_tiny_hnf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_tiny_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_tiny_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_tiny_in22k.py` & `mlagility-3.0.2/models/timm/convnext_tiny_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_xlarge_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_xlarge_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_xlarge_in22ft1k.py` & `mlagility-3.0.2/models/timm/convnext_xlarge_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/convnext_xlarge_in22k.py` & `mlagility-3.0.2/models/timm/convnext_xlarge_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_15_dagger_240.py` & `mlagility-3.0.2/models/timm/crossvit_15_dagger_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_15_dagger_408.py` & `mlagility-3.0.2/models/timm/crossvit_15_dagger_408.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_18_dagger_240.py` & `mlagility-3.0.2/models/timm/crossvit_18_dagger_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_18_dagger_408.py` & `mlagility-3.0.2/models/timm/crossvit_18_dagger_408.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_9_dagger_240.py` & `mlagility-3.0.2/models/timm/crossvit_9_dagger_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_base_240.py` & `mlagility-3.0.2/models/timm/crossvit_base_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_small_240.py` & `mlagility-3.0.2/models/timm/crossvit_small_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/crossvit_tiny_240.py` & `mlagility-3.0.2/models/timm/crossvit_tiny_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/cs3darknet_focus_l.py` & `mlagility-3.0.2/models/timm/cs3darknet_focus_l.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/cs3darknet_focus_m.py` & `mlagility-3.0.2/models/timm/cs3darknet_focus_m.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/cs3darknet_focus_s.py` & `mlagility-3.0.2/models/timm/cs3darknet_focus_s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/cs3darknet_focus_x.py` & `mlagility-3.0.2/models/timm/cs3darknet_focus_x.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_base_patch16_224.py` & `mlagility-3.0.2/models/timm/deit3_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_base_patch16_224_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_base_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_base_patch16_384.py` & `mlagility-3.0.2/models/timm/deit3_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_base_patch16_384_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_base_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_huge_patch14_224.py` & `mlagility-3.0.2/models/timm/deit3_huge_patch14_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_huge_patch14_224_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_huge_patch14_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_large_patch16_224.py` & `mlagility-3.0.2/models/timm/deit3_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_large_patch16_224_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_large_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_large_patch16_384.py` & `mlagility-3.0.2/models/timm/deit3_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_large_patch16_384_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_large_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_small_patch16_224.py` & `mlagility-3.0.2/models/timm/deit3_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_small_patch16_224_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_small_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_small_patch16_384.py` & `mlagility-3.0.2/models/timm/deit3_small_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit3_small_patch16_384_in21ft1k.py` & `mlagility-3.0.2/models/timm/deit3_small_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_base_distilled_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_base_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_base_distilled_patch16_384.py` & `mlagility-3.0.2/models/timm/deit_base_distilled_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_base_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_base_patch16_384.py` & `mlagility-3.0.2/models/timm/deit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_small_distilled_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_small_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_small_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_tiny_distilled_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_tiny_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/deit_tiny_patch16_224.py` & `mlagility-3.0.2/models/timm/deit_tiny_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/eca_botnext26ts_256.py` & `mlagility-3.0.2/models/timm/eca_botnext26ts_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ecaresnext26t_32x4d.py` & `mlagility-3.0.2/models/timm/ecaresnext26t_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ecaresnext50t_32x4d.py` & `mlagility-3.0.2/models/timm/ecaresnext50t_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/edgenext_small_rw.py` & `mlagility-3.0.2/models/timm/edgenext_small_rw.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/edgenext_xx_small.py` & `mlagility-3.0.2/models/timm/edgenext_xx_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_b0_g16_evos.py` & `mlagility-3.0.2/models/timm/efficientnet_b0_g16_evos.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_b0_g8_gn.py` & `mlagility-3.0.2/models/timm/efficientnet_b0_g8_gn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_b0_gn.py` & `mlagility-3.0.2/models/timm/efficientnet_b0_gn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_b3_g8_gn.py` & `mlagility-3.0.2/models/timm/efficientnet_b3_g8_gn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_b3_gn.py` & `mlagility-3.0.2/models/timm/efficientnet_b3_gn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_cc_b0_4e.py` & `mlagility-3.0.2/models/timm/efficientnet_cc_b0_4e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_cc_b0_8e.py` & `mlagility-3.0.2/models/timm/efficientnet_cc_b0_8e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_cc_b1_8e.py` & `mlagility-3.0.2/models/timm/efficientnet_cc_b1_8e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_el_pruned.py` & `mlagility-3.0.2/models/timm/efficientnet_el_pruned.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_es_pruned.py` & `mlagility-3.0.2/models/timm/efficientnet_es_pruned.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_lite0.py` & `mlagility-3.0.2/models/timm/efficientnet_lite0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_lite1.py` & `mlagility-3.0.2/models/timm/efficientnet_lite1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_lite2.py` & `mlagility-3.0.2/models/timm/efficientnet_lite2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_lite3.py` & `mlagility-3.0.2/models/timm/efficientnet_lite3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnet_lite4.py` & `mlagility-3.0.2/models/timm/efficientnet_lite4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnetv2_rw_m.py` & `mlagility-3.0.2/models/timm/efficientnetv2_rw_m.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnetv2_rw_s.py` & `mlagility-3.0.2/models/timm/efficientnetv2_rw_s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnetv2_rw_t.py` & `mlagility-3.0.2/models/timm/efficientnetv2_rw_t.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/efficientnetv2_xl.py` & `mlagility-3.0.2/models/timm/efficientnetv2_xl.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ens_adv_inception_resnet_v2.py` & `mlagility-3.0.2/models/timm/ens_adv_inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ese_vovnet19b_slim.py` & `mlagility-3.0.2/models/timm/ese_vovnet19b_slim.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ese_vovnet19b_slim_dw.py` & `mlagility-3.0.2/models/timm/ese_vovnet19b_slim_dw.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ese_vovnet39b_evos.py` & `mlagility-3.0.2/models/timm/ese_vovnet39b_evos.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gc_efficientnetv2_rw_t.py` & `mlagility-3.0.2/models/timm/gc_efficientnetv2_rw_t.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_inception_v3.py` & `mlagility-3.0.2/models/timm/gluon_inception_v3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet101_v1b.py` & `mlagility-3.0.2/models/timm/gluon_resnet101_v1b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet101_v1c.py` & `mlagility-3.0.2/models/timm/gluon_resnet101_v1c.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet101_v1d.py` & `mlagility-3.0.2/models/timm/gluon_resnet101_v1d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet101_v1s.py` & `mlagility-3.0.2/models/timm/gluon_resnet101_v1s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet152_v1b.py` & `mlagility-3.0.2/models/timm/gluon_resnet152_v1b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet152_v1c.py` & `mlagility-3.0.2/models/timm/gluon_resnet152_v1c.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet152_v1d.py` & `mlagility-3.0.2/models/timm/gluon_resnet152_v1d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet152_v1s.py` & `mlagility-3.0.2/models/timm/gluon_resnet152_v1s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet18_v1b.py` & `mlagility-3.0.2/models/timm/gluon_resnet18_v1b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet34_v1b.py` & `mlagility-3.0.2/models/timm/gluon_resnet34_v1b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet50_v1b.py` & `mlagility-3.0.2/models/timm/gluon_resnet50_v1b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet50_v1c.py` & `mlagility-3.0.2/models/timm/gluon_resnet50_v1c.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet50_v1d.py` & `mlagility-3.0.2/models/timm/gluon_resnet50_v1d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnet50_v1s.py` & `mlagility-3.0.2/models/timm/gluon_resnet50_v1s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnext101_32x4d.py` & `mlagility-3.0.2/models/timm/gluon_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnext101_64x4d.py` & `mlagility-3.0.2/models/timm/gluon_resnext101_64x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_resnext50_32x4d.py` & `mlagility-3.0.2/models/timm/gluon_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_seresnext101_32x4d.py` & `mlagility-3.0.2/models/timm/gluon_seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_seresnext101_64x4d.py` & `mlagility-3.0.2/models/timm/gluon_seresnext101_64x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/gluon_seresnext50_32x4d.py` & `mlagility-3.0.2/models/timm/gluon_seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/halo2botnet50ts_256.py` & `mlagility-3.0.2/models/timm/halo2botnet50ts_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/hrnet_w18_small_v2.py` & `mlagility-3.0.2/models/timm/hrnet_w18_small_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ig_resnext101_32x16d.py` & `mlagility-3.0.2/models/timm/ig_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ig_resnext101_32x32d.py` & `mlagility-3.0.2/models/timm/ig_resnext101_32x32d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ig_resnext101_32x48d.py` & `mlagility-3.0.2/models/timm/ig_resnext101_32x48d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ig_resnext101_32x8d.py` & `mlagility-3.0.2/models/timm/ig_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/inception_resnet_v2.py` & `mlagility-3.0.2/models/timm/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/lambda_resnet26rpt_256.py` & `mlagility-3.0.2/models/timm/lambda_resnet26rpt_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/lambda_resnet50ts.py` & `mlagility-3.0.2/models/timm/lambda_resnet50ts.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/lamhalobotnet50ts_256.py` & `mlagility-3.0.2/models/timm/lamhalobotnet50ts_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnet101.py` & `mlagility-3.0.2/models/timm/legacy_seresnet101.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnet152.py` & `mlagility-3.0.2/models/timm/legacy_seresnet152.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnet18.py` & `mlagility-3.0.2/models/timm/legacy_seresnet18.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnet34.py` & `mlagility-3.0.2/models/timm/legacy_seresnet34.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnet50.py` & `mlagility-3.0.2/models/timm/legacy_seresnet50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnext101_32x4d.py` & `mlagility-3.0.2/models/timm/legacy_seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnext26_32x4d.py` & `mlagility-3.0.2/models/timm/legacy_seresnext26_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/legacy_seresnext50_32x4d.py` & `mlagility-3.0.2/models/timm/legacy_seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mixer_b16_224_in21k.py` & `mlagility-3.0.2/models/timm/mixer_b16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mixer_b16_224_miil.py` & `mlagility-3.0.2/models/timm/mixer_b16_224_miil.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mixer_b16_224_miil_in21k.py` & `mlagility-3.0.2/models/timm/mixer_b16_224_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mixer_l16_224_in21k.py` & `mlagility-3.0.2/models/timm/mixer_l16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_large_075.py` & `mlagility-3.0.2/models/timm/mobilenetv3_large_075.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_large_100.py` & `mlagility-3.0.2/models/timm/mobilenetv3_large_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_large_100_miil.py` & `mlagility-3.0.2/models/timm/mobilenetv3_large_100_miil.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_large_100_miil_in21k.py` & `mlagility-3.0.2/models/timm/mobilenetv3_large_100_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_small_050.py` & `mlagility-3.0.2/models/timm/mobilenetv3_small_050.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_small_075.py` & `mlagility-3.0.2/models/timm/mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilenetv3_small_100.py` & `mlagility-3.0.2/models/timm/mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_150_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_150_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_150_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_150_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_175_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_175_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_175_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_175_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_200_384_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_200_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/mobilevitv2_200_in22ft1k.py` & `mlagility-3.0.2/models/timm/mobilevitv2_200_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/pit_b_distilled_224.py` & `mlagility-3.0.2/models/timm/pit_b_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/pit_s_distilled_224.py` & `mlagility-3.0.2/models/timm/pit_s_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/pit_ti_distilled_224.py` & `mlagility-3.0.2/models/timm/pit_ti_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/pit_xs_distilled_224.py` & `mlagility-3.0.2/models/timm/pit_xs_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/res2net101_26w_4s.py` & `mlagility-3.0.2/models/timm/res2net101_26w_4s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_12_224_dino.py` & `mlagility-3.0.2/models/timm/resmlp_12_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_12_distilled_224.py` & `mlagility-3.0.2/models/timm/resmlp_12_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_24_224_dino.py` & `mlagility-3.0.2/models/timm/resmlp_24_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_24_distilled_224.py` & `mlagility-3.0.2/models/timm/resmlp_24_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_36_distilled_224.py` & `mlagility-3.0.2/models/timm/resmlp_36_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_big_24_224.py` & `mlagility-3.0.2/models/timm/resmlp_big_24_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_big_24_224_in22ft1k.py` & `mlagility-3.0.2/models/timm/resmlp_big_24_224_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resmlp_big_24_distilled_224.py` & `mlagility-3.0.2/models/timm/resmlp_big_24_distilled_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnest50d_1s4x24d.py` & `mlagility-3.0.2/models/timm/resnest50d_1s4x24d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnest50d_4s2x40d.py` & `mlagility-3.0.2/models/timm/resnest50d_4s2x40d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_101x1_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_101x1_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_101x1_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_101x1_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_101x3_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_101x3_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_101x3_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_101x3_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x2_bit_teacher.py` & `mlagility-3.0.2/models/timm/resnetv2_152x2_bit_teacher.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x2_bit_teacher_384.py` & `mlagility-3.0.2/models/timm/resnetv2_152x2_bit_teacher_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x2_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_152x2_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x2_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_152x2_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x4_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_152x4_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_152x4_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_152x4_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50d_evob.py` & `mlagility-3.0.2/models/timm/resnetv2_50d_evob.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50d_evos.py` & `mlagility-3.0.2/models/timm/resnetv2_50d_evos.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50x1_bit_distilled.py` & `mlagility-3.0.2/models/timm/resnetv2_50x1_bit_distilled.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50x1_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_50x1_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50x1_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_50x1_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50x3_bitm.py` & `mlagility-3.0.2/models/timm/resnetv2_50x3_bitm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/resnetv2_50x3_bitm_in21k.py` & `mlagility-3.0.2/models/timm/resnetv2_50x3_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext101_32x4d.py` & `mlagility-3.0.2/models/timm/seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext101_32x8d.py` & `mlagility-3.0.2/models/timm/seresnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext101d_32x8d.py` & `mlagility-3.0.2/models/timm/seresnext101d_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext26d_32x4d.py` & `mlagility-3.0.2/models/timm/seresnext26d_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext26t_32x4d.py` & `mlagility-3.0.2/models/timm/seresnext26t_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext26tn_32x4d.py` & `mlagility-3.0.2/models/timm/seresnext26tn_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnext50_32x4d.py` & `mlagility-3.0.2/models/timm/seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/seresnextaa101d_32x8d.py` & `mlagility-3.0.2/models/timm/seresnextaa101d_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/skresnext50_32x4d.py` & `mlagility-3.0.2/models/timm/skresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ssl_resnext101_32x16d.py` & `mlagility-3.0.2/models/timm/ssl_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ssl_resnext101_32x4d.py` & `mlagility-3.0.2/models/timm/ssl_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ssl_resnext101_32x8d.py` & `mlagility-3.0.2/models/timm/ssl_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/ssl_resnext50_32x4d.py` & `mlagility-3.0.2/models/timm/ssl_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_base_patch4_window12_384.py` & `mlagility-3.0.2/models/timm/swin_base_patch4_window12_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_base_patch4_window12_384_in22k.py` & `mlagility-3.0.2/models/timm/swin_base_patch4_window12_384_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_base_patch4_window7_224.py` & `mlagility-3.0.2/models/timm/swin_base_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_base_patch4_window7_224_in22k.py` & `mlagility-3.0.2/models/timm/swin_base_patch4_window7_224_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_large_patch4_window12_384.py` & `mlagility-3.0.2/models/timm/swin_large_patch4_window12_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_large_patch4_window12_384_in22k.py` & `mlagility-3.0.2/models/timm/swin_large_patch4_window12_384_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_large_patch4_window7_224.py` & `mlagility-3.0.2/models/timm/swin_large_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_large_patch4_window7_224_in22k.py` & `mlagility-3.0.2/models/timm/swin_large_patch4_window7_224_in22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_s3_small_224.py` & `mlagility-3.0.2/models/timm/swin_s3_small_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_small_patch4_window7_224.py` & `mlagility-3.0.2/models/timm/swin_small_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swin_tiny_patch4_window7_224.py` & `mlagility-3.0.2/models/timm/swin_tiny_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_base_window12_192_22k.py` & `mlagility-3.0.2/models/timm/swinv2_base_window12_192_22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_base_window12to16_192to256_22kft1k.py` & `mlagility-3.0.2/models/timm/swinv2_base_window12to16_192to256_22kft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_base_window12to24_192to384_22kft1k.py` & `mlagility-3.0.2/models/timm/swinv2_base_window12to24_192to384_22kft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_base_window16_256.py` & `mlagility-3.0.2/models/timm/swinv2_base_window16_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_base_window8_256.py` & `mlagility-3.0.2/models/timm/swinv2_base_window8_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_base_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_base_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_base_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_base_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_base_ns_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_base_ns_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_giant_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_giant_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_giant_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_giant_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_huge_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_huge_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_huge_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_huge_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_large_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_large_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_large_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_large_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_small_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_small_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_small_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_small_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_small_ns_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_small_ns_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_tiny_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_tiny_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_tiny_384.py` & `mlagility-3.0.2/models/timm/swinv2_cr_tiny_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_cr_tiny_ns_224.py` & `mlagility-3.0.2/models/timm/swinv2_cr_tiny_ns_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_large_window12_192_22k.py` & `mlagility-3.0.2/models/timm/swinv2_large_window12_192_22k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_large_window12to16_192to256_22kft1k.py` & `mlagility-3.0.2/models/timm/swinv2_large_window12to16_192to256_22kft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_large_window12to24_192to384_22kft1k.py` & `mlagility-3.0.2/models/timm/swinv2_large_window12to24_192to384_22kft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_small_window16_256.py` & `mlagility-3.0.2/models/timm/swinv2_small_window16_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_small_window8_256.py` & `mlagility-3.0.2/models/timm/swinv2_small_window8_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_tiny_window16_256.py` & `mlagility-3.0.2/models/timm/swinv2_tiny_window16_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swinv2_tiny_window8_256.py` & `mlagility-3.0.2/models/timm/swinv2_tiny_window8_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swsl_resnext101_32x16d.py` & `mlagility-3.0.2/models/timm/swsl_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swsl_resnext101_32x4d.py` & `mlagility-3.0.2/models/timm/swsl_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swsl_resnext101_32x8d.py` & `mlagility-3.0.2/models/timm/swsl_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/swsl_resnext50_32x4d.py` & `mlagility-3.0.2/models/timm/swsl_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b0.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b0_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b0_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b0_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b0_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b1.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b1_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b1_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b1_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b1_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b2.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b2_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b2_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b2_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b2_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b3.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b3_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b3_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b3_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b3_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b4.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b4_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b4_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b4_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b4_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b5.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b5_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b5_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b5_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b5_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b6.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b6.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b6_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b6_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b6_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b6_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b7.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b7.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b7_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b7_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b7_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b7_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b8.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b8.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_b8_ap.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_b8_ap.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_cc_b0_4e.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_cc_b0_4e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_cc_b0_8e.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_cc_b0_8e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_cc_b1_8e.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_cc_b1_8e.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_el.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_el.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_em.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_em.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_es.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_es.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_l2_ns.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_l2_ns.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_l2_ns_475.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_l2_ns_475.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_lite0.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_lite0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_lite1.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_lite1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_lite2.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_lite2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_lite3.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_lite3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnet_lite4.py` & `mlagility-3.0.2/models/timm/tf_efficientnet_lite4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_b0.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_b0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_b1.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_b1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_b2.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_b2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_b3.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_b3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_l.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_l.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_l_in21ft1k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_l_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_l_in21k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_l_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_m.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_m.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_m_in21ft1k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_m_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_m_in21k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_m_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_s.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_s_in21ft1k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_s_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_s_in21k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_s_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_xl_in21ft1k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_xl_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_efficientnetv2_xl_in21k.py` & `mlagility-3.0.2/models/timm/tf_efficientnetv2_xl_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_large_075.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_large_075.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_large_100.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_large_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_large_minimal_100.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_large_minimal_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_small_075.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_small_100.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tf_mobilenetv3_small_minimal_100.py` & `mlagility-3.0.2/models/timm/tf_mobilenetv3_small_minimal_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tnt_b_patch16_224.py` & `mlagility-3.0.2/models/timm/tnt_b_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tnt_s_patch16_224.py` & `mlagility-3.0.2/models/timm/tnt_s_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/tv_resnext50_32x4d.py` & `mlagility-3.0.2/models/timm/tv_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/twins_pcpvt_large.py` & `mlagility-3.0.2/models/timm/twins_pcpvt_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/twins_pcpvt_small.py` & `mlagility-3.0.2/models/timm/twins_pcpvt_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_18x2_224.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_18x2_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224_dino.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224_miil.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224_miil.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224_miil_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_224_sam.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_224_sam.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_384.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_plus_240.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_plus_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch16_rpn_224.py` & `mlagility-3.0.2/models/timm/vit_base_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch32_224.py` & `mlagility-3.0.2/models/timm/vit_base_patch32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch32_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch32_224_sam.py` & `mlagility-3.0.2/models/timm/vit_base_patch32_224_sam.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch32_384.py` & `mlagility-3.0.2/models/timm/vit_base_patch32_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch32_plus_256.py` & `mlagility-3.0.2/models/timm/vit_base_patch32_plus_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch8_224.py` & `mlagility-3.0.2/models/timm/vit_base_patch8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch8_224_dino.py` & `mlagility-3.0.2/models/timm/vit_base_patch8_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_patch8_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_patch8_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_r26_s32_224.py` & `mlagility-3.0.2/models/timm/vit_base_r26_s32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_r50_s16_224.py` & `mlagility-3.0.2/models/timm/vit_base_r50_s16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_r50_s16_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_r50_s16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_r50_s16_384.py` & `mlagility-3.0.2/models/timm/vit_base_r50_s16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_resnet26d_224.py` & `mlagility-3.0.2/models/timm/vit_base_resnet26d_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_resnet50_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_base_resnet50_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_resnet50_384.py` & `mlagility-3.0.2/models/timm/vit_base_resnet50_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_base_resnet50d_224.py` & `mlagility-3.0.2/models/timm/vit_base_resnet50d_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_giant_patch14_224.py` & `mlagility-3.0.2/models/timm/vit_giant_patch14_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_gigantic_patch14_224.py` & `mlagility-3.0.2/models/timm/vit_gigantic_patch14_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_huge_patch14_224.py` & `mlagility-3.0.2/models/timm/vit_huge_patch14_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_huge_patch14_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_huge_patch14_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch14_224.py` & `mlagility-3.0.2/models/timm/vit_large_patch14_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch16_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_large_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch16_384.py` & `mlagility-3.0.2/models/timm/vit_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch32_224.py` & `mlagility-3.0.2/models/timm/vit_large_patch32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch32_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_large_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_patch32_384.py` & `mlagility-3.0.2/models/timm/vit_large_patch32_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_r50_s32_224.py` & `mlagility-3.0.2/models/timm/vit_large_r50_s32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_r50_s32_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_large_r50_s32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_large_r50_s32_384.py` & `mlagility-3.0.2/models/timm/vit_large_r50_s32_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch16_cls_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch16_cls_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch16_clsgap_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch16_clsgap_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch16_plus_240.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch16_plus_240.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch16_rpn_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_base_patch32_plus_rpn_256.py` & `mlagility-3.0.2/models/timm/vit_relpos_base_patch32_plus_rpn_256.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_cls_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_cls_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_medium_patch16_rpn_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_medium_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_small_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_relpos_small_patch16_rpn_224.py` & `mlagility-3.0.2/models/timm/vit_relpos_small_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_18x2_224.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_18x2_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_224_dino.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_36x1_224.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_36x1_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch16_384.py` & `mlagility-3.0.2/models/timm/vit_small_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch32_224.py` & `mlagility-3.0.2/models/timm/vit_small_patch32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch32_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_small_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch32_384.py` & `mlagility-3.0.2/models/timm/vit_small_patch32_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_patch8_224_dino.py` & `mlagility-3.0.2/models/timm/vit_small_patch8_224_dino.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_r26_s32_224.py` & `mlagility-3.0.2/models/timm/vit_small_r26_s32_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_r26_s32_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_small_r26_s32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_r26_s32_384.py` & `mlagility-3.0.2/models/timm/vit_small_r26_s32_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_resnet26d_224.py` & `mlagility-3.0.2/models/timm/vit_small_resnet26d_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_small_resnet50d_s16_224.py` & `mlagility-3.0.2/models/timm/vit_small_resnet50d_s16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_srelpos_medium_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_srelpos_medium_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_srelpos_small_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_srelpos_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_patch16_224.py` & `mlagility-3.0.2/models/timm/vit_tiny_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_patch16_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_tiny_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_patch16_384.py` & `mlagility-3.0.2/models/timm/vit_tiny_patch16_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_224.py` & `mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_224_in21k.py` & `mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_224_in21k.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/vit_tiny_r_s16_p8_384.py` & `mlagility-3.0.2/models/timm/vit_tiny_r_s16_p8_384.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_large_24_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_large_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_medium_24_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_medium_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_nano_12_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_nano_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_12_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_small_24_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_small_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_12_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p16_224.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p16_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p16_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p8_224.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p8_224_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/timm/xcit_tiny_24_p8_384_dist.py` & `mlagility-3.0.2/models/timm/xcit_tiny_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/alexnet.py` & `mlagility-3.0.2/models/torch_hub/alexnet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/convnext_base.py` & `mlagility-3.0.2/models/torch_hub/convnext_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/convnext_large.py` & `mlagility-3.0.2/models/torch_hub/convnext_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/convnext_small.py` & `mlagility-3.0.2/models/torch_hub/convnext_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/convnext_tiny.py` & `mlagility-3.0.2/models/torch_hub/convnext_tiny.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/densenet121.py` & `mlagility-3.0.2/models/torch_hub/densenet121.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/densenet161.py` & `mlagility-3.0.2/models/torch_hub/densenet161.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/densenet169.py` & `mlagility-3.0.2/models/torch_hub/densenet169.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/densenet201.py` & `mlagility-3.0.2/models/torch_hub/densenet201.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b0.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b1.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b2.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b3.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b4.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b4.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b5.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b6.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b6.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_b7.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_b7.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_v2_l.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_v2_l.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_v2_m.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_v2_m.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/efficientnet_v2_s.py` & `mlagility-3.0.2/models/torch_hub/efficientnet_v2_s.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/ghostnet.py` & `mlagility-3.0.2/models/torch_hub/ghostnet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/ghostnet_1x.py` & `mlagility-3.0.2/models/torch_hub/ghostnet_1x.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/googlenet.py` & `mlagility-3.0.2/models/torch_hub/googlenet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/hardnet39ds.py` & `mlagility-3.0.2/models/torch_hub/hardnet39ds.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/hardnet68.py` & `mlagility-3.0.2/models/torch_hub/hardnet68.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/hardnet68ds.py` & `mlagility-3.0.2/models/torch_hub/hardnet68ds.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/hardnet85.py` & `mlagility-3.0.2/models/torch_hub/hardnet85.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/inception_v3.py` & `mlagility-3.0.2/models/torch_hub/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv1_resnest50.py` & `mlagility-3.0.2/models/torch_hub/mealv1_resnest50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_efficientnet_b0.py` & `mlagility-3.0.2/models/torch_hub/mealv2_efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_mobilenet_v3_large_100.py` & `mlagility-3.0.2/models/torch_hub/mealv2_mobilenet_v3_large_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_mobilenetv3_small_075.py` & `mlagility-3.0.2/models/torch_hub/mealv2_mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_mobilenetv3_small_100.py` & `mlagility-3.0.2/models/torch_hub/mealv2_mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_resnest50.py` & `mlagility-3.0.2/models/torch_hub/mealv2_resnest50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_resnest50_380x380.py` & `mlagility-3.0.2/models/torch_hub/mealv2_resnest50_380x380.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mealv2_resnest50_cutmix.py` & `mlagility-3.0.2/models/torch_hub/mealv2_resnest50_cutmix.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/midas_v2.1_small.py` & `mlagility-3.0.2/models/torch_hub/midas_v2.1_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/midas_v3_hybrid.py` & `mlagility-3.0.2/models/torch_hub/midas_v3_hybrid.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/midas_v3_large.py` & `mlagility-3.0.2/models/torch_hub/midas_v3_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mnasnet0_5.py` & `mlagility-3.0.2/models/torch_hub/mnasnet0_5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mnasnet0_75.py` & `mlagility-3.0.2/models/torch_hub/mnasnet0_75.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mnasnet1_0.py` & `mlagility-3.0.2/models/torch_hub/mnasnet1_0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mnasnet1_3.py` & `mlagility-3.0.2/models/torch_hub/mnasnet1_3.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mobilenet_v2.py` & `mlagility-3.0.2/models/torch_hub/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mobilenet_v3_large.py` & `mlagility-3.0.2/models/torch_hub/mobilenet_v3_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/mobilenet_v3_small.py` & `mlagility-3.0.2/models/torch_hub/mobilenet_v3_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/proxyless_cpu.py` & `mlagility-3.0.2/models/torch_hub/proxyless_cpu.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/proxyless_gpu.py` & `mlagility-3.0.2/models/torch_hub/proxyless_gpu.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/proxyless_mobile.py` & `mlagility-3.0.2/models/torch_hub/proxyless_mobile.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/proxyless_mobile_14.py` & `mlagility-3.0.2/models/torch_hub/proxyless_mobile_14.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_16gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_16gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_1_6gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_1_6gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_32gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_32gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_3_2gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_3_2gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_400mf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_400mf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_800mf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_800mf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_x_8gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_x_8gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_128gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_128gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_16gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_16gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_1_6gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_1_6gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_32gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_32gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_3_2gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_3_2gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_400mf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_400mf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_800mf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_800mf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/regnet_y_8gf.py` & `mlagility-3.0.2/models/torch_hub/regnet_y_8gf.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest101.py` & `mlagility-3.0.2/models/torch_hub/resnest101.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest200.py` & `mlagility-3.0.2/models/torch_hub/resnest200.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest269.py` & `mlagility-3.0.2/models/torch_hub/resnest269.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50.py` & `mlagility-3.0.2/models/torch_hub/resnest50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_1s1x64d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_1s1x64d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_1s2x40d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_1s2x40d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_1s4x24d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_1s4x24d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_2s1x64d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_2s1x64d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_2s2x40d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_2s2x40d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_4s1x64d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_4s1x64d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnest50_fast_4s2x40d.py` & `mlagility-3.0.2/models/torch_hub/resnest50_fast_4s2x40d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet101.py` & `mlagility-3.0.2/models/torch_hub/resnet101.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet101_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/resnet101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet101_ibn_b.py` & `mlagility-3.0.2/models/torch_hub/resnet101_ibn_b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet152.py` & `mlagility-3.0.2/models/torch_hub/resnet152.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet18.py` & `mlagility-3.0.2/models/torch_hub/resnet18.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet18_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/resnet18_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet18_ibn_b.py` & `mlagility-3.0.2/models/torch_hub/resnet18_ibn_b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet34.py` & `mlagility-3.0.2/models/torch_hub/resnet34.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet34_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/resnet34_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet34_ibn_b.py` & `mlagility-3.0.2/models/torch_hub/resnet34_ibn_b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet50.py` & `mlagility-3.0.2/models/torch_hub/resnet50.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet50_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/resnet50_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnet50_ibn_b.py` & `mlagility-3.0.2/models/torch_hub/resnet50_ibn_b.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnext101_32x8d.py` & `mlagility-3.0.2/models/torch_hub/resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnext101_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/resnext101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/resnext50_32x4d.py` & `mlagility-3.0.2/models/torch_hub/resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/se_resnet101_ibn_a.py` & `mlagility-3.0.2/models/torch_hub/se_resnet101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/shufflenet_v2_x0_5.py` & `mlagility-3.0.2/models/torch_hub/shufflenet_v2_x0_5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/shufflenet_v2_x1_0.py` & `mlagility-3.0.2/models/torch_hub/shufflenet_v2_x1_0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/shufflenet_v2_x1_5.py` & `mlagility-3.0.2/models/torch_hub/shufflenet_v2_x1_5.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/shufflenet_v2_x2_0.py` & `mlagility-3.0.2/models/torch_hub/shufflenet_v2_x2_0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/squeezenet1_0.py` & `mlagility-3.0.2/models/torch_hub/squeezenet1_0.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/squeezenet1_1.py` & `mlagility-3.0.2/models/torch_hub/squeezenet1_1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/unet.py` & `mlagility-3.0.2/models/torch_hub/unet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg11.py` & `mlagility-3.0.2/models/torch_hub/vgg11.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg11_bn.py` & `mlagility-3.0.2/models/torch_hub/vgg11_bn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg13.py` & `mlagility-3.0.2/models/torch_hub/vgg13.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg13_bn.py` & `mlagility-3.0.2/models/torch_hub/vgg13_bn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg16.py` & `mlagility-3.0.2/models/torch_hub/vgg16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg16_bn.py` & `mlagility-3.0.2/models/torch_hub/vgg16_bn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg19.py` & `mlagility-3.0.2/models/torch_hub/vgg19.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vgg19_bn.py` & `mlagility-3.0.2/models/torch_hub/vgg19_bn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vit_b_16.py` & `mlagility-3.0.2/models/torch_hub/vit_b_16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vit_b_32.py` & `mlagility-3.0.2/models/torch_hub/vit_b_32.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vit_h_14.py` & `mlagility-3.0.2/models/torch_hub/vit_h_14.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vit_l_16.py` & `mlagility-3.0.2/models/torch_hub/vit_l_16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/vit_l_32.py` & `mlagility-3.0.2/models/torch_hub/vit_l_32.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/wide_resnet101_2.py` & `mlagility-3.0.2/models/torch_hub/wide_resnet101_2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torch_hub/wide_resnet50_2.py` & `mlagility-3.0.2/models/torch_hub/wide_resnet50_2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py` & `mlagility-3.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py` & `mlagility-3.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/fasterrcnn_resnet50_fpn.py` & `mlagility-3.0.2/models/torchvision/fasterrcnn_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/fasterrcnn_resnet50_fpn_v2.py` & `mlagility-3.0.2/models/torchvision/fasterrcnn_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/fcos_resnet50_fpn.py` & `mlagility-3.0.2/models/torchvision/fcos_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/keypointrcnn_resnet50_fpn.py` & `mlagility-3.0.2/models/torchvision/keypointrcnn_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/maskrcnn_resnet50_fpn.py` & `mlagility-3.0.2/models/torchvision/maskrcnn_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/maskrcnn_resnet50_fpn_v2.py` & `mlagility-3.0.2/models/torchvision/maskrcnn_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/retinanet_resnet50_fpn.py` & `mlagility-3.0.2/models/torchvision/retinanet_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/retinanet_resnet50_fpn_v2.py` & `mlagility-3.0.2/models/torchvision/retinanet_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/ssd300_vgg16.py` & `mlagility-3.0.2/models/torchvision/ssd300_vgg16.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/torchvision/ssdlite320_mobilenet_v3_large.py` & `mlagility-3.0.2/models/torchvision/ssdlite320_mobilenet_v3_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bart.py` & `mlagility-3.0.2/models/transformers/bart.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/beit.py` & `mlagility-3.0.2/models/transformers/beit.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bert.py` & `mlagility-3.0.2/models/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bert_for_question_answering.py` & `mlagility-3.0.2/models/transformers/bert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bert_generation.py` & `mlagility-3.0.2/models/transformers/bert_generation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bert_tiny_for_sequence_classification.py` & `mlagility-3.0.2/models/transformers/bert_tiny_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/bigbird_pegasus.py` & `mlagility-3.0.2/models/transformers/bigbird_pegasus.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/biggan.py` & `mlagility-3.0.2/models/transformers/biggan.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/blenderbot_small.py` & `mlagility-3.0.2/models/transformers/blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/camembert.py` & `mlagility-3.0.2/models/transformers/camembert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/convbert.py` & `mlagility-3.0.2/models/transformers/convbert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/convnext.py` & `mlagility-3.0.2/models/transformers/convnext.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/data2vecaudio.py` & `mlagility-3.0.2/models/transformers/data2vecaudio.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/data2vectext.py` & `mlagility-3.0.2/models/transformers/data2vectext.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/deberta.py` & `mlagility-3.0.2/models/transformers/deberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/deit.py` & `mlagility-3.0.2/models/transformers/deit.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/deit_base_for_image_classification.py` & `mlagility-3.0.2/models/transformers/deit_base_for_image_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/deit_tiny_for_image_classification.py` & `mlagility-3.0.2/models/transformers/deit_tiny_for_image_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/detr.py` & `mlagility-3.0.2/models/transformers/detr.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/detr_for_object_detection.py` & `mlagility-3.0.2/models/transformers/detr_for_object_detection.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/distil_wav2vec2_for_audio_classification.py` & `mlagility-3.0.2/models/transformers/distil_wav2vec2_for_audio_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/distilbert.py` & `mlagility-3.0.2/models/transformers/distilbert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/distilbert_for_question_answering.py` & `mlagility-3.0.2/models/transformers/distilbert_for_question_answering.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/distilhubert_for_audio_classification.py` & `mlagility-3.0.2/models/transformers/distilhubert_for_audio_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/electra.py` & `mlagility-3.0.2/models/transformers/electra.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/electra_for_sequence_classification.py` & `mlagility-3.0.2/models/transformers/electra_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/encoder_decoder.py` & `mlagility-3.0.2/models/transformers/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/flaubert.py` & `mlagility-3.0.2/models/transformers/flaubert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/funnel.py` & `mlagility-3.0.2/models/transformers/funnel.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/funnel_base.py` & `mlagility-3.0.2/models/transformers/funnel_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/gpt1.py` & `mlagility-3.0.2/models/transformers/gpt1.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/gpt2.py` & `mlagility-3.0.2/models/transformers/gpt2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/gpt2_doublehead.py` & `mlagility-3.0.2/models/transformers/gpt2_doublehead.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/hubert.py` & `mlagility-3.0.2/models/transformers/hubert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/ibert.py` & `mlagility-3.0.2/models/transformers/ibert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/imagegpt.py` & `mlagility-3.0.2/models/transformers/imagegpt.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/layoutlm.py` & `mlagility-3.0.2/models/transformers/layoutlm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/luke.py` & `mlagility-3.0.2/models/transformers/luke.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/m2m_100.py` & `mlagility-3.0.2/models/transformers/m2m_100.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/marian.py` & `mlagility-3.0.2/models/transformers/marian.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/marianmt.py` & `mlagility-3.0.2/models/transformers/marianmt.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/megatron_bert.py` & `mlagility-3.0.2/models/transformers/megatron_bert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/minilmv2.py` & `mlagility-3.0.2/models/transformers/minilmv2.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilebert.py` & `mlagility-3.0.2/models/transformers/mobilebert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilebert_for_sequence_classification.py` & `mlagility-3.0.2/models/transformers/mobilebert_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilevit.py` & `mlagility-3.0.2/models/transformers/mobilevit.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilevit_small_for_semantic_segmentation.py` & `mlagility-3.0.2/models/transformers/mobilevit_small_for_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilevit_x_small_for_semantic_segmentation.py` & `mlagility-3.0.2/models/transformers/mobilevit_x_small_for_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mobilevit_xx_small_for_semantic_segmentation.py` & `mlagility-3.0.2/models/transformers/mobilevit_xx_small_for_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mpnet.py` & `mlagility-3.0.2/models/transformers/mpnet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mt5_base.py` & `mlagility-3.0.2/models/transformers/mt5_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/mt5_small.py` & `mlagility-3.0.2/models/transformers/mt5_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/openai_doublehead.py` & `mlagility-3.0.2/models/transformers/openai_doublehead.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/pegasus.py` & `mlagility-3.0.2/models/transformers/pegasus.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/perceiver.py` & `mlagility-3.0.2/models/transformers/perceiver.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/poolformer.py` & `mlagility-3.0.2/models/transformers/poolformer.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/rag.py` & `mlagility-3.0.2/models/transformers/rag.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/realm.py` & `mlagility-3.0.2/models/transformers/realm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/rembert.py` & `mlagility-3.0.2/models/transformers/rembert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/retribert.py` & `mlagility-3.0.2/models/transformers/retribert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/roberta.py` & `mlagility-3.0.2/models/transformers/roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/roformer.py` & `mlagility-3.0.2/models/transformers/roformer.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/segformer.py` & `mlagility-3.0.2/models/transformers/segformer.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/speech_encoder_decoder.py` & `mlagility-3.0.2/models/transformers/speech_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/speech_encoder_decoder_pretrained.py` & `mlagility-3.0.2/models/transformers/speech_encoder_decoder_pretrained.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/speech_to_text.py` & `mlagility-3.0.2/models/transformers/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/splinter.py` & `mlagility-3.0.2/models/transformers/splinter.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/squeezebert.py` & `mlagility-3.0.2/models/transformers/squeezebert.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/t5_base.py` & `mlagility-3.0.2/models/transformers/t5_base.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/t5_large.py` & `mlagility-3.0.2/models/transformers/t5_large.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/t5_small.py` & `mlagility-3.0.2/models/transformers/t5_small.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/unispeech.py` & `mlagility-3.0.2/models/transformers/unispeech.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/unispeech_sat.py` & `mlagility-3.0.2/models/transformers/unispeech_sat.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/vision_encoder_decoder.py` & `mlagility-3.0.2/models/transformers/vision_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/vit.py` & `mlagility-3.0.2/models/transformers/vit.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/xglm.py` & `mlagility-3.0.2/models/transformers/xglm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/xlm.py` & `mlagility-3.0.2/models/transformers/xlm.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/xlm_roberta.py` & `mlagility-3.0.2/models/transformers/xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/xlnet-512.py` & `mlagility-3.0.2/models/transformers/xlnet-512.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/xlnet.py` & `mlagility-3.0.2/models/transformers/xlnet.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/models/transformers/yolos_tiny_for_object_detection.py` & `mlagility-3.0.2/models/transformers/yolos_tiny_for_object_detection.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/setup.py` & `mlagility-3.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,9 +62,12 @@
             "benchit=mlagility:benchitcli",
         ]
     },
     python_requires=">=3.8, <3.11",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     include_package_data=True,
-    package_data={"mlagility.api": ["Dockerfile"]},
+    package_data={
+        "mlagility.api": ["Dockerfile"],
+        "mlagility_models": ["requirements.txt", "readme.md"],
+    },
 )
```

### Comparing `mlagility-3.0.0/src/mlagility/analysis/analysis.py` & `mlagility-3.0.2/src/mlagility/analysis/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     device: str
     backend: str
     runtime: str
     actions: List[Action]
     lean_cache: bool
     targets: List[str]
     max_depth: int
+    onnx_opset: int
     cache_dir: str
     rebuild: str
     groq_compiler_flags: List[str]
     groq_assembler_flags: List[str]
     groq_num_chips: int
     groqview: bool
     models_found: Dict[str, util.ModelInfo] = dataclasses.field(default_factory=dict)
@@ -129,14 +130,15 @@
             build_only=Action.BENCHMARK not in tracer_args.actions,
             lean_cache=tracer_args.lean_cache,
             groq_num_chips=tracer_args.groq_num_chips,
             groq_compiler_flags=tracer_args.groq_compiler_flags,
             groq_assembler_flags=tracer_args.groq_assembler_flags,
             groqview=tracer_args.groqview,
             sequence=tracer_args.sequence,
+            onnx_opset=tracer_args.onnx_opset,
         )
 
         if Action.BENCHMARK in tracer_args.actions:
             model_info.status_message = "Model successfully benchmarked!"
             model_info.performance = perf
         else:
             model_info.status_message = "Model successfully built!"
```

### Comparing `mlagility-3.0.0/src/mlagility/analysis/status.py` & `mlagility-3.0.2/src/mlagility/analysis/status.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/analysis/tf_helpers.py` & `mlagility-3.0.2/src/mlagility/analysis/tf_helpers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/analysis/util.py` & `mlagility-3.0.2/src/mlagility/analysis/util.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/devices.py` & `mlagility-3.0.2/src/mlagility/api/devices.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/execute_trt.py` & `mlagility-3.0.2/src/mlagility/api/execute_trt.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/model_api.py` & `mlagility-3.0.2/src/mlagility/api/model_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     cache_dir: str = filesystem.DEFAULT_CACHE_DIR,
     device: str = "x86",
     runtime: str = "ort",
     backend: str = "local",
     build_only: bool = False,
     lean_cache: bool = False,
     rebuild: str = MLAGILITY_DEFAULT_REBUILD_POLICY,
+    onnx_opset: int = build.DEFAULT_ONNX_OPSET,
     groq_compiler_flags: Optional[List[str]] = None,
     groq_assembler_flags: Optional[List[str]] = None,
     groq_num_chips: Optional[int] = None,
     groqview: bool = False,
     sequence: Sequence = None,
 ) -> MeasuredPerformance:
     """
@@ -63,14 +64,21 @@
         if device == "groq":
             # pylint: disable=import-error
             from groqflow import groqit
             import onnxflow.justbuildit.export as export
             import onnxflow.justbuildit.stage as stage
             import groqflow.justgroqit.export as gf_export
             import groqflow.justgroqit.compile as gf_compile
+            import groqflow.common.build as gf_build
+
+            if onnx_opset != gf_build.DEFAULT_ONNX_OPSET:
+                raise ValueError(
+                    "ONNX opset for Groq builds must match GroqFlow's ONNX opset, "
+                    f"{gf_build.DEFAULT_ONNX_OPSET}, however onnx_opset is set to {onnx_opset}"
+                )
 
             # Set the GroqFlow sequence to execute Stages in the same order
             # as build_model()
 
             if sequence is None:
                 groqflow_sequence = stage.Sequence(
                     "groqflow_sequence",
@@ -121,14 +129,15 @@
             omodel = build_model(
                 model=model,
                 inputs=inputs,
                 build_name=build_name,
                 cache_dir=cache_dir,
                 rebuild=rebuild,
                 sequence=sequence,
+                onnx_opset=onnx_opset,
             )
 
             if not build_only:
                 printing.log_info(f"Benchmarking on {backend} {device}...")
                 gpu_model = trtmodel.TRTModel(
                     cache_dir=omodel.state.cache_dir,
                     build_name=omodel.state.config.build_name,
@@ -139,14 +148,15 @@
             omodel = build_model(
                 model=model,
                 inputs=inputs,
                 build_name=build_name,
                 cache_dir=cache_dir,
                 rebuild=rebuild,
                 sequence=sequence,
+                onnx_opset=onnx_opset,
             )
 
             if not build_only:
                 printing.log_info(f"Benchmarking on {backend} {device}...")
                 cpu_model = ortmodel.ORTModel(
                     build_name=omodel.state.config.build_name,
                     cache_dir=omodel.state.cache_dir,
```

### Comparing `mlagility-3.0.0/src/mlagility/api/ortmodel.py` & `mlagility-3.0.2/src/mlagility/api/ortmodel.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/performance.py` & `mlagility-3.0.2/src/mlagility/api/performance.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/run_ort_model.py` & `mlagility-3.0.2/src/mlagility/api/run_ort_model.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/script_api.py` & `mlagility-3.0.2/src/mlagility/api/script_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import os
 import types
 import importlib.machinery
 from typing import Tuple, List, Dict, Optional, Union
 import onnxflow.common.printing as printing
+import onnxflow.common.build as build
 import onnxflow.common.exceptions as exceptions
 import onnxflow.justbuildit.stage as stage
 import onnxflow.justbuildit.export as export
 import mlagility.cli.slurm as slurm
 import mlagility.common.filesystem as filesystem
 import mlagility.common.labels as labels_library
 from mlagility.api.model_api import benchmark_model
@@ -88,14 +89,15 @@
     backend: str = "local",
     runtimes: List[str] = None,
     analyze_only: bool = False,
     build_only: bool = False,
     resume: bool = False,
     script_args: Optional[str] = None,
     max_depth: int = 0,
+    onnx_opset: int = build.DEFAULT_ONNX_OPSET,
     sequence: Union[str, stage.Sequence] = None,
     groq_compiler_flags: Optional[List[str]] = None,
     groq_assembler_flags: Optional[List[str]] = None,
     groq_num_chips: Optional[int] = None,
     groqview: bool = False,
 ):
 
@@ -203,28 +205,30 @@
                     groq_compiler_flags=groq_compiler_flags,
                     groq_assembler_flags=groq_assembler_flags,
                     groq_num_chips=groq_num_chips,
                     groqview=groqview,
                     device=device,
                     runtimes=[runtime],
                     max_depth=max_depth,
+                    onnx_opset=onnx_opset,
                     analyze_only=analyze_only,
                     build_only=build_only,
                     lean_cache=lean_cache,
                 )
 
             else:
 
                 # Instantiate an object that holds all of the arguments
                 # for analysis, build, and benchmarking
                 tracer_args = TracerArgs(
                     input=script_path,
                     lean_cache=lean_cache,
                     targets=targets,
                     max_depth=max_depth,
+                    onnx_opset=onnx_opset,
                     cache_dir=cache_dir,
                     rebuild=rebuild,
                     groq_compiler_flags=groq_compiler_flags,
                     groq_assembler_flags=groq_assembler_flags,
                     groq_num_chips=groq_num_chips,
                     groqview=groqview,
                     device=device,
@@ -262,16 +266,17 @@
     rebuild: Optional[str] = None,
     device: str = None,
     backend: str = "local",
     runtimes: List[str] = None,
     analyze_only: bool = False,
     build_only: bool = False,
     resume: bool = False,
-    script_args: str = "",
+    script_args: Optional[str] = None,
     max_depth: int = 0,
+    onnx_opset: int = build.DEFAULT_ONNX_OPSET,
     sequence: Union[str, stage.Sequence] = None,
     groq_compiler_flags: Optional[List[str]] = None,
     groq_assembler_flags: Optional[List[str]] = None,
     groq_num_chips: Optional[int] = None,
     groqview: bool = False,
 ):
 
@@ -303,14 +308,15 @@
             backend=backend,
             runtimes=runtimes,
             analyze_only=analyze_only,
             build_only=build_only,
             resume=resume,
             script_args=script_args,
             max_depth=max_depth,
+            onnx_opset=onnx_opset,
             sequence=sequence,
             groq_compiler_flags=groq_compiler_flags,
             groq_assembler_flags=groq_assembler_flags,
             groq_num_chips=groq_num_chips,
             groqview=groqview,
         )
 
@@ -337,13 +343,14 @@
                 cache_dir=cache_dir,
                 device=device,
                 backend=backend,
                 runtime=runtime,
                 build_only=build_only,
                 lean_cache=lean_cache,
                 rebuild=rebuild,
+                onnx_opset=onnx_opset,
                 groq_compiler_flags=groq_compiler_flags,
                 groq_assembler_flags=groq_assembler_flags,
                 groq_num_chips=groq_num_chips,
                 groqview=groqview,
                 sequence=onnx_sequence,
             )
```

### Comparing `mlagility-3.0.0/src/mlagility/api/setup_ort.py` & `mlagility-3.0.2/src/mlagility/api/setup_ort.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/api/trtmodel.py` & `mlagility-3.0.2/src/mlagility/api/trtmodel.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/cli/cli.py` & `mlagility-3.0.2/src/mlagility/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         backend=args.backend,
         runtimes=args.runtimes,
         analyze_only=args.analyze_only,
         build_only=args.build_only,
         resume=args.resume,
         script_args=args.script_args,
         max_depth=args.max_depth,
+        onnx_opset=args.onnx_opset,
         sequence=args.sequence_file,
         groq_compiler_flags=args.groq_compiler_flags,
         groq_assembler_flags=args.groq_assembler_flags,
         groq_num_chips=args.groq_num_chips,
         groqview=args.groqview,
     )
 
@@ -223,14 +224,22 @@
         dest="max_depth",
         type=int,
         default=0,
         help="Maximum depth to analyze within the model structure of the target script(s)",
     )
 
     benchmark_parser.add_argument(
+        "--onnx-opset",
+        dest="onnx_opset",
+        type=int,
+        default=build.DEFAULT_ONNX_OPSET,
+        help=f"ONNX opset used when creating ONNX files (default={build.DEFAULT_ONNX_OPSET})",
+    )
+
+    benchmark_parser.add_argument(
         "--groq-compiler-flags",
         nargs="+",
         dest="groq_compiler_flags",
         help="Sets the groqit(compiler_flags=...) arg (default behavior is to use groqit()'s "
         "default compiler flags)",
         required=False,
         default=None,
```

### Comparing `mlagility-3.0.0/src/mlagility/cli/login.py` & `mlagility-3.0.2/src/mlagility/cli/login.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/cli/report.py` & `mlagility-3.0.2/src/mlagility/cli/report.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/cli/slurm.py` & `mlagility-3.0.2/src/mlagility/cli/slurm.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     rebuild: Optional[str] = None,
     groq_compiler_flags: Optional[List[str]] = None,
     groq_assembler_flags: Optional[List[str]] = None,
     groq_num_chips: Optional[int] = None,
     groqview: Optional[bool] = None,
     runtimes: Optional[List[str]] = None,
     max_depth: Optional[int] = None,
+    onnx_opset: Optional[int] = None,
     analyze_only: Optional[bool] = None,
     build_only: Optional[bool] = None,
     lean_cache: Optional[bool] = None,
     working_dir: str = os.getcwd(),
     ml_cache_dir: Optional[str] = os.environ.get("SLURM_ML_CACHE"),
     max_jobs: int = 50,
 ):
@@ -84,22 +85,23 @@
     rebuild_str = value_arg(rebuild, "--rebuild")
     compiler_flags_str = list_arg(groq_compiler_flags, "--groq-compiler-flags")
     assembler_flags_str = list_arg(groq_assembler_flags, "--groq-assembler-flags")
     num_chips_str = value_arg(groq_num_chips, "--groq-num-chips")
     groqview_str = bool_arg(groqview, "--groqview")
     runtimes_str = list_arg(runtimes, "--runtimes")
     max_depth_str = value_arg(max_depth, "--max-depth")
+    onnx_opset_str = value_arg(onnx_opset, "--onnx-opset")
     analyze_only_str = bool_arg(analyze_only, "--analyze-only")
     build_only_str = bool_arg(build_only, "--build-only")
     lean_cache_str = bool_arg(lean_cache, "--lean-cache")
 
     args = (
         f"{op} {script} --device {device} {cache_dir_str}{rebuild_str}"
         f"{compiler_flags_str}{assembler_flags_str}{num_chips_str}{groqview_str}"
-        f"{runtimes_str}{max_depth_str}{analyze_only_str}"
+        f"{runtimes_str}{max_depth_str}{onnx_opset_str}{analyze_only_str}"
         f"{build_only_str}{lean_cache_str}"
     )
 
     # Remove the .py extension from the build name
     job_name = filesystem.clean_script_name(script)
 
     while len(jobs_in_queue()) >= max_jobs:
```

### Comparing `mlagility-3.0.0/src/mlagility/common/filesystem.py` & `mlagility-3.0.2/src/mlagility/common/filesystem.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/common/labels.py` & `mlagility-3.0.2/src/mlagility/common/labels.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility/parser.py` & `mlagility-3.0.2/src/mlagility/parser.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/mlagility.egg-info/PKG-INFO` & `mlagility-3.0.2/src/mlagility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlagility
-Version: 3.0.0
+Version: 3.0.2
 Summary: MLAgility Benchmark and Tools
 Home-page: https://github.com/groq/mlagility
 Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
 Author-email: jfowers@groq.com, dhnoronha@groq.com, rsivakumar@groq.com, vgodsoe@groq.com
 License: MIT
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
```

### Comparing `mlagility-3.0.0/src/mlagility.egg-info/SOURCES.txt` & `mlagility-3.0.2/src/mlagility.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 models/__init__.py
+models/readme.md
+models/requirements.txt
 models/diffusers/__init__.py
 models/diffusers/clip_text_encoder.py
 models/diffusers/safety_clipvision.py
 models/diffusers/unet_2d_condition.py
 models/diffusers/vae_decoder.py
 models/graph_convolutions/__init__.py
 models/graph_convolutions/chebconv.py
```

### Comparing `mlagility-3.0.0/src/onnxflow/common/build.py` & `mlagility-3.0.2/src/onnxflow/common/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
     str,
     torch.nn.Module,
     torch.jit.ScriptModule,
     "tf.keras.Model",
     sklearn.base.BaseEstimator,
 ]
 
-DEFAULT_ONNX_OPSET = 14
+if os.environ.get("MLAGILITY_ONNX_OPSET"):
+    DEFAULT_ONNX_OPSET = int(os.environ.get("MLAGILITY_ONNX_OPSET"))
+else:
+    DEFAULT_ONNX_OPSET = 14
+
 MINIMUM_ONNX_OPSET = 11
 
 DEFAULT_CACHE_DIR = os.getcwd()
 DEFAULT_REBUILD_POLICY = "if_needed"
 
 
 class Backend(enum.Enum):
@@ -194,14 +198,15 @@
     version number of the onnxflow package if you do make a build-
     breaking change.
     """
 
     build_name: str
     auto_name: bool
     sequence: List[str]
+    onnx_opset: int
 
 
 @dataclasses.dataclass
 class Info:
     """
     Information about a build that may be useful for analysis
     or debugging purposes.
@@ -214,15 +219,14 @@
     backend: Backend = Backend.AUTO
     base_onnx_exported: Optional[bool] = None
     opt_onnx_exported: Optional[bool] = None
     opt_onnx_ops: Optional[List[str]] = None
     converted_onnx_exported: Optional[bool] = None
     quantized_onnx_exported: Optional[bool] = None
     skipped_stages: int = 0
-    opset: Optional[int] = DEFAULT_ONNX_OPSET
     all_build_stages: List[str] = dataclasses.field(default_factory=list)
     current_build_stage: str = None
     completed_build_stages: List[str] = dataclasses.field(default_factory=list)
     build_stage_execution_times: Dict[str, float] = dataclasses.field(
         default_factory=dict
     )
 
@@ -304,36 +308,36 @@
     def onnx_dir(self):
         return os.path.join(output_dir(self.cache_dir, self.config.build_name), "onnx")
 
     @property
     def base_onnx_file(self):
         return os.path.join(
             self.onnx_dir,
-            f"{self.config.build_name}-op{self.info.opset}-base.onnx",
+            f"{self.config.build_name}-op{self.config.onnx_opset}-base.onnx",
         )
 
     @property
     def opt_onnx_file(self):
         return os.path.join(
             self.onnx_dir,
-            f"{self.config.build_name}-op{self.info.opset}-opt.onnx",
+            f"{self.config.build_name}-op{self.config.onnx_opset}-opt.onnx",
         )
 
     @property
     def converted_onnx_file(self):
         return os.path.join(
             self.onnx_dir,
-            f"{self.config.build_name}-op{self.info.opset}-opt-f16.onnx",
+            f"{self.config.build_name}-op{self.config.onnx_opset}-opt-f16.onnx",
         )
 
     @property
     def quantized_onnx_file(self):
         return os.path.join(
             self.onnx_dir,
-            f"{self.config.build_name}-op{self.info.opset}-opt-quantized_int8.onnx",
+            f"{self.config.build_name}-op{self.config.onnx_opset}-opt-quantized_int8.onnx",
         )
 
     def prepare_file_system(self):
         # Create output folder if it doesn't exist
         os.makedirs(output_dir(self.cache_dir, self.config.build_name), exist_ok=True)
         os.makedirs(self.onnx_dir, exist_ok=True)
```

### Comparing `mlagility-3.0.0/src/onnxflow/common/cache.py` & `mlagility-3.0.2/src/onnxflow/common/cache.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/exceptions.py` & `mlagility-3.0.2/src/onnxflow/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/onnx_helpers.py` & `mlagility-3.0.2/src/onnxflow/common/onnx_helpers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/printing.py` & `mlagility-3.0.2/src/onnxflow/common/printing.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/quantization_helpers.py` & `mlagility-3.0.2/src/onnxflow/common/quantization_helpers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/tensor_helpers.py` & `mlagility-3.0.2/src/onnxflow/common/tensor_helpers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/common/tf_helpers.py` & `mlagility-3.0.2/src/onnxflow/common/tf_helpers.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/justbuildit/buildit.py` & `mlagility-3.0.2/src/onnxflow/justbuildit/buildit.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     inputs: Optional[Dict[str, Any]] = None,
     build_name: Optional[str] = None,
     cache_dir: str = build.DEFAULT_CACHE_DIR,
     monitor: bool = True,
     rebuild: Optional[str] = None,
     sequence: Optional[List[stage.Stage]] = None,
     quantization_samples: Collection = None,
+    onnx_opset: int = build.DEFAULT_ONNX_OPSET,
 ) -> omodel.BaseModel:
 
     """Use build a model instance into an optimized ONNX file.
 
     Args:
         model: Model to be mapped to an optimized ONNX file, which can be a PyTorch
             model instance, Keras model instance, Hummingbird model instance,
@@ -45,24 +46,26 @@
         sequence: Override the default sequence of build stages. Power
             users only.
         quantization_samples: If set, performs post-training quantization
             on the ONNX model using the provided samplesIf the previous build used samples
             that are different to the samples used in current build, the "rebuild"
             argument needs to be manually set to "always" in the current build
             in order to create a new ONNX file.
+        onnx_opset: ONNX opset to use during ONNX export.
     """
 
     # Support "~" in the cache_dir argument
     parsed_cache_dir = os.path.expanduser(cache_dir)
 
     # Validate and lock in the config (user arguments that
     # configure the build) that will be used by the rest of the toolchain
     config = ignition.lock_config(
         build_name=build_name,
         sequence=sequence,
+        onnx_opset=onnx_opset,
     )
 
     # Analyze the user's model argument and lock in the model, inputs,
     # and sequence that will be used by the rest of the toolchain
     (model_locked, inputs_locked, sequence_locked, model_type,) = ignition.model_intake(
         model,
         inputs,
```

### Comparing `mlagility-3.0.0/src/onnxflow/justbuildit/export.py` & `mlagility-3.0.2/src/onnxflow/justbuildit/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import inspect
 import shutil
-import re
 import warnings
 import sys
 import copy
 from typing import Union
 import torch
 import onnxruntime
 import onnxmltools
@@ -82,16 +81,15 @@
             raise exp.StageError(msg)
 
         dummy_inputs = tuple(state.inputs.values())
         dummy_input_names = tuple(state.inputs.keys())
         state.inputs = dict(zip(dummy_input_names, dummy_inputs))
 
         model = onnx.load(state.model)
-        opset_str = str(model.opset_import)  # pylint: disable=no-member
-        opset = int(re.search(r"\d+", opset_str).group())
+        opset = getattr(model.opset_import[0], "version", None)
         input_shapes = [
             [d.dim_value for d in _input.type.tensor_type.shape.dim]
             for _input in model.graph.input  # pylint: disable=no-member
         ]
 
         # Save output node names
         state.expected_output_names = get_output_names(model)
@@ -219,29 +217,27 @@
 
         else:  # state.model is a torch.jit.ScriptModule
             dummy_inputs = tuple(state.inputs.values())
 
             # Collect input names
             dummy_input_names = tuple(state.inputs.keys())
 
-        state.info.opset = build.DEFAULT_ONNX_OPSET
-
         # Send torch export warnings to stdout (and therefore the log file)
         # so that they don't fill up the command line
         default_warnings = warnings.showwarning
         warnings.showwarning = _warn_to_stdout
 
         # Export the model to ONNX
         torch.onnx.export(
             state.model,
             dummy_inputs,
             state.base_onnx_file,
             input_names=dummy_input_names,
             do_constant_folding=True,
-            opset_version=state.info.opset,
+            opset_version=state.config.onnx_opset,
             verbose=False,
         )
 
         # Save output names to ensure we are preserving the order of the outputs
         state.expected_output_names = get_output_names(state.base_onnx_file)
 
         # Restore default warnings behavior
@@ -349,21 +345,19 @@
                 dtype = tf.int32
             if inp.shape[0] is None:
                 print("Found batch size None and setting it to 1")
                 shape = (1, shape[1:])
 
             input_specs.append(tf.TensorSpec(shape, dtype, name))
 
-        state.info.opset = build.DEFAULT_ONNX_OPSET
-
         # Export the model to ONNX
         tf2onnx.convert.from_keras(
             state.model,
             input_signature=input_specs,
-            opset=state.info.opset,
+            opset=state.config.onnx_opset,
             output_path=state.base_onnx_file,
         )
 
         # Save output names to ensure we are preserving the order of the outputs
         state.expected_output_names = get_output_names(state.base_onnx_file)
 
         state.inputs = dict(zip(tuple(input_names), tuple(inputs)))
```

### Comparing `mlagility-3.0.0/src/onnxflow/justbuildit/hummingbird.py` & `mlagility-3.0.2/src/onnxflow/justbuildit/hummingbird.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,14 @@
               - sklearn.tree.DecisionTreeClassifier
 
             Supported xgboost models:
               - xgboost.XGBClassifier
             """
             raise exp.StageError(msg)
 
-        state.info.opset = build.DEFAULT_ONNX_OPSET
         # TODO: By default the strategy will be chosen wih Hummingbird's logic.
         # Ideally, this would also be a parameter.
         tree_implementation_strategy = "gemm"  # or "tree_trav" or "perf_tree_trav"
 
         inputs = state.inputs
         if inputs is None:
             raise exp.StageError(
@@ -138,15 +137,15 @@
             raise exp.StageError(
                 "Fitting a model with float64 inputs can cause issues"
                 " with conversion and compilation. This can be corrected by changing"
                 " code like model.fit(X, y) to model.fit(X.astype(numpy.float32), y)."
             )
 
         extra_config = {
-            "onnx_target_opset": state.info.opset,
+            "onnx_target_opset": state.config.onnx_opset,
             "tree_implementation": tree_implementation_strategy,
         }
 
         try:
             onnx_model = hummingbird.ml.convert(
                 state.model, "onnx", test_X, extra_config=extra_config
             ).model
```

### Comparing `mlagility-3.0.0/src/onnxflow/justbuildit/ignition.py` & `mlagility-3.0.2/src/onnxflow/justbuildit/ignition.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     "--ifetch-slice-ordering=round-robin",
 ]
 
 
 def lock_config(
     build_name: Optional[str] = None,
     sequence: stage.Sequence = None,
+    onnx_opset: int = build.DEFAULT_ONNX_OPSET,
 ) -> build.Config:
 
     """
     Process the user's configuration arguments to build_model():
     1. Raise exceptions for illegal arguments
     2. Replace unset arguments with default values
     3. Lock the configuration into an immutable object
@@ -104,14 +105,15 @@
         stage_names = sequence.get_names()
 
     # Store the args that should be immutable
     config = build.Config(
         build_name=build_name,
         auto_name=auto_name,
         sequence=stage_names,
+        onnx_opset=onnx_opset,
     )
 
     return config
 
 
 def decode_version_number(version: str) -> Dict[str, int]:
     numbers = [int(x) for x in version.split(".")]
```

### Comparing `mlagility-3.0.0/src/onnxflow/justbuildit/stage.py` & `mlagility-3.0.2/src/onnxflow/justbuildit/stage.py`

 * *Files identical despite different names*

### Comparing `mlagility-3.0.0/src/onnxflow/model/model.py` & `mlagility-3.0.2/src/onnxflow/model/model.py`

 * *Files identical despite different names*


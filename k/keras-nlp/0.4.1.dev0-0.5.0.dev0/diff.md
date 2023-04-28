# Comparing `tmp/keras-nlp-0.4.1.dev0.tar.gz` & `tmp/keras-nlp-0.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nlp-0.4.1.dev0.tar", last modified: Wed Feb 22 04:15:46 2023, max compression
+gzip compressed data, was "keras-nlp-0.5.0.dev0.tar", last modified: Fri Apr 28 17:50:55 2023, max compression
```

## Comparing `keras-nlp-0.4.1.dev0.tar` & `keras-nlp-0.5.0.dev0.tar`

### file list

```diff
@@ -1,280 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.209206 keras-nlp-0.4.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-02-22 04:15:46.209206 keras-nlp-0.4.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.161206 keras-nlp-0.4.1.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.161206 keras-nlp-0.4.1.dev0/examples/bert_pretraining/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/bert_pretraining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/examples/machine_translation/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/machine_translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/machine_translation/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/machine_translation/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/machine_translation/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/machine_translation/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/examples/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/tools/split_sentences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/tools/train_word_piece_vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/examples/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/examples/utils/scripting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/keras_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/keras_nlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/benchmarks/sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/benchmarks/text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.173206 keras-nlp-0.4.1.dev0/keras_nlp/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/f_net_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/f_net_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/multi_segment_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/random_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/random_deletion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/random_swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/random_swap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/sine_position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/sine_position_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/start_end_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/start_end_packer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/token_and_position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/token_and_position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_layer_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.173206 keras-nlp-0.4.1.dev0/keras_nlp/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/bleu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/edit_distance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/perplexity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_l_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_n_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.173206 keras-nlp-0.4.1.dev0/keras_nlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.177206 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.181206 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.181206 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.185206 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/relative_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.185206 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.189206 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.189206 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.193206 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.193206 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.197206 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.201206 keras-nlp-0.4.1.dev0/keras_nlp/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/beam_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/beam_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/greedy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/greedy_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_k_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_k_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_p_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_p_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.201206 keras-nlp-0.4.1.dev0/keras_nlp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.201206 keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/docstring_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.201206 keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/basic_usage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/import_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.205206 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22780 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.205206 keras-nlp-0.4.1.dev0/keras_nlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/keras_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/keras_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/pipeline_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28571 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37824 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/text_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/keras_nlp/utils/tf_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.165206 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-02-22 04:15:46.000000 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-02-22 04:15:46.000000 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 04:15:46.000000 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-22 04:15:46.000000 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 04:15:46.000000 keras-nlp-0.4.1.dev0/keras_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-22 04:15:46.209206 keras-nlp-0.4.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.205206 keras-nlp-0.4.1.dev0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 04:15:46.209206 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/checkpoint_conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_albert_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_bart_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_distilbert_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_f_net_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_gpt2_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_opt_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_roberta_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-22 04:15:36.000000 keras-nlp-0.4.1.dev0/tools/count_preset_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/bert_pretraining/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/machine_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/machine_translation/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/split_sentences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/tools/train_word_piece_vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/examples/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/examples/utils/scripting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/basic_usage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/integration_tests/import_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/keras_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.300500 keras-nlp-0.5.0.dev0/keras_nlp/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/cached_multi_head_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.304500 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.308500 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.312500 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/relative_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.316500 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.320500 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.320500 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.324500 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17266 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_causal_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.328500 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.328500 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/task_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.332500 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/whisper_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/contrastive_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/greedy_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.336500 keras-nlp-0.5.0.dev0/keras_nlp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.340499 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24873 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/keras_nlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23195 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.296500 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 17:50:55.000000 keras-nlp-0.5.0.dev0/keras_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.344499 keras-nlp-0.5.0.dev0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:50:55.348500 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/checkpoint_conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_albert_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_bart_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_distilbert_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_f_net_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_gpt2_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_opt_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_roberta_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 17:50:47.000000 keras-nlp-0.5.0.dev0/tools/count_preset_params.py
```

### Comparing `keras-nlp-0.4.1.dev0/LICENSE` & `keras-nlp-0.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/PKG-INFO` & `keras-nlp-0.5.0.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.4.1.dev0
+Version: 0.5.0.dev0
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +36,15 @@
 that have state-of-the-art preset weights and architectures when used 
 out-of-the-box and are easily customizable when more control is needed. We 
 emphasize in-graph computation for all workflows so that developers can expect 
 easy productionization using the TensorFlow ecosystem.
 
 This library is an extension of the core Keras API; all high-level modules are 
 [`Layers`](https://keras.io/api/layers/) or 
-[`Models`](https://keras.io/api/models/) that recieve that same level of polish 
+[`Models`](https://keras.io/api/models/) that receive that same level of polish 
 as core Keras. If you are familiar with Keras, congratulations! You already 
 understand most of KerasNLP.
 
 See our [Getting Started guide](https://keras.io/guides/keras_nlp/getting_started) 
 for example usage of our modular API starting with evaluating pretrained models 
 and building up to designing a novel transformer architecture and training a 
 tokenizer from scratch.  
@@ -69,57 +69,48 @@
 - [Call for Contributions](https://github.com/keras-team/keras-nlp/issues?q=is%3Aissue+is%3Aopen+label%3A%22contributions+welcome%22)
 
 ## Installation
 
 To install the latest official release:
 
 ```
-pip install keras-nlp tensorflow --upgrade
+pip install keras-nlp --upgrade
 ```
 
 To install the latest unreleased changes to the library, we recommend using
 pip to install directly from the master branch on github:
 
 ```
-pip install git+https://github.com/keras-team/keras-nlp.git tensorflow --upgrade
+pip install git+https://github.com/keras-team/keras-nlp.git --upgrade
 ```
 
 ## Quickstart
 
 Fine-tune BERT on a small sentiment analysis task using the 
 [`keras_nlp.models`](https://keras.io/api/keras_nlp/models/) API:
 
 ```python
 import keras_nlp
-from tensorflow import keras
 import tensorflow_datasets as tfds
 
 imdb_train, imdb_test = tfds.load(
     "imdb_reviews",
     split=["train", "test"],
     as_supervised=True,
     batch_size=16,
 )
+# Load a BERT model.
 classifier = keras_nlp.models.BertClassifier.from_preset(
-    "bert_base_en_uncased",
+    "bert_base_en_uncased", 
+    num_classes=2,
 )
-classifier.compile(
-    loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    optimizer=keras.optimizers.Adam(5e-5),
-    metrics=keras.metrics.SparseCategoricalAccuracy(),
-    jit_compile=True,
-)
-classifier.fit(
-    imdb_train,
-    validation_data=imdb_test,
-    epochs=1,
-)
-
-# Predict a new example
-classifier.predict(["What an amazing movie, three hours of pure bliss!"])
+# Fine-tune on IMDb movie reviews.
+classifier.fit(imdb_train, validation_data=imdb_test)
+# Predict two new examples.
+classifier.predict(["What an amazing movie!", "A total waste of my time."])
 ```
 
 For more in depth guides and examples, visit https://keras.io/keras_nlp/.
 
 ## Compatibility
 
 We follow [Semantic Versioning](https://semver.org/), and plan to
@@ -129,15 +120,15 @@
 
 ## Disclaimer
 
 KerasNLP provides access to pre-trained models via the `keras_nlp.models` API.
 These pre-trained models are provided on an "as is" basis, without warranties
 or conditions of any kind. The following underlying models are provided by third
 parties, and subject to separate licenses:
-DistilBERT, RoBERTa, XLM-RoBERTa, DeBERTa, and GPT-2.
+BART, DeBERTa, DistilBERT, GPT-2, OPT, RoBERTa, Whisper, and XLM-RoBERTa.
 
 ## Citing KerasNLP
 
 If KerasNLP helps your research, we appreciate your citations.
 Here is the BibTeX entry:
 
 ```bibtex
```

### Comparing `keras-nlp-0.4.1.dev0/README.md` & `keras-nlp-0.5.0.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 that have state-of-the-art preset weights and architectures when used 
 out-of-the-box and are easily customizable when more control is needed. We 
 emphasize in-graph computation for all workflows so that developers can expect 
 easy productionization using the TensorFlow ecosystem.
 
 This library is an extension of the core Keras API; all high-level modules are 
 [`Layers`](https://keras.io/api/layers/) or 
-[`Models`](https://keras.io/api/models/) that recieve that same level of polish 
+[`Models`](https://keras.io/api/models/) that receive that same level of polish 
 as core Keras. If you are familiar with Keras, congratulations! You already 
 understand most of KerasNLP.
 
 See our [Getting Started guide](https://keras.io/guides/keras_nlp/getting_started) 
 for example usage of our modular API starting with evaluating pretrained models 
 and building up to designing a novel transformer architecture and training a 
 tokenizer from scratch.  
@@ -43,57 +43,48 @@
 - [Call for Contributions](https://github.com/keras-team/keras-nlp/issues?q=is%3Aissue+is%3Aopen+label%3A%22contributions+welcome%22)
 
 ## Installation
 
 To install the latest official release:
 
 ```
-pip install keras-nlp tensorflow --upgrade
+pip install keras-nlp --upgrade
 ```
 
 To install the latest unreleased changes to the library, we recommend using
 pip to install directly from the master branch on github:
 
 ```
-pip install git+https://github.com/keras-team/keras-nlp.git tensorflow --upgrade
+pip install git+https://github.com/keras-team/keras-nlp.git --upgrade
 ```
 
 ## Quickstart
 
 Fine-tune BERT on a small sentiment analysis task using the 
 [`keras_nlp.models`](https://keras.io/api/keras_nlp/models/) API:
 
 ```python
 import keras_nlp
-from tensorflow import keras
 import tensorflow_datasets as tfds
 
 imdb_train, imdb_test = tfds.load(
     "imdb_reviews",
     split=["train", "test"],
     as_supervised=True,
     batch_size=16,
 )
+# Load a BERT model.
 classifier = keras_nlp.models.BertClassifier.from_preset(
-    "bert_base_en_uncased",
+    "bert_base_en_uncased", 
+    num_classes=2,
 )
-classifier.compile(
-    loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    optimizer=keras.optimizers.Adam(5e-5),
-    metrics=keras.metrics.SparseCategoricalAccuracy(),
-    jit_compile=True,
-)
-classifier.fit(
-    imdb_train,
-    validation_data=imdb_test,
-    epochs=1,
-)
-
-# Predict a new example
-classifier.predict(["What an amazing movie, three hours of pure bliss!"])
+# Fine-tune on IMDb movie reviews.
+classifier.fit(imdb_train, validation_data=imdb_test)
+# Predict two new examples.
+classifier.predict(["What an amazing movie!", "A total waste of my time."])
 ```
 
 For more in depth guides and examples, visit https://keras.io/keras_nlp/.
 
 ## Compatibility
 
 We follow [Semantic Versioning](https://semver.org/), and plan to
@@ -103,15 +94,15 @@
 
 ## Disclaimer
 
 KerasNLP provides access to pre-trained models via the `keras_nlp.models` API.
 These pre-trained models are provided on an "as is" basis, without warranties
 or conditions of any kind. The following underlying models are provided by third
 parties, and subject to separate licenses:
-DistilBERT, RoBERTa, XLM-RoBERTa, DeBERTa, and GPT-2.
+BART, DeBERTa, DistilBERT, GPT-2, OPT, RoBERTa, Whisper, and XLM-RoBERTa.
 
 ## Citing KerasNLP
 
 If KerasNLP helps your research, we appreciate your citations.
 Here is the BibTeX entry:
 
 ```bibtex
```

### Comparing `keras-nlp-0.4.1.dev0/examples/__init__.py` & `keras-nlp-0.5.0.dev0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/bert_pretraining/__init__.py` & `keras-nlp-0.5.0.dev0/examples/bert_pretraining/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_config.py` & `keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_config.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_create_pretraining_data.py` & `keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/bert_pretraining/bert_pretrain.py` & `keras-nlp-0.5.0.dev0/examples/bert_pretraining/bert_pretrain.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/machine_translation/__init__.py` & `keras-nlp-0.5.0.dev0/examples/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/machine_translation/data.py` & `keras-nlp-0.5.0.dev0/examples/machine_translation/data.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/machine_translation/inference.py` & `keras-nlp-0.5.0.dev0/examples/machine_translation/inference.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/machine_translation/model.py` & `keras-nlp-0.5.0.dev0/examples/machine_translation/model.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/machine_translation/train.py` & `keras-nlp-0.5.0.dev0/examples/machine_translation/train.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/tools/__init__.py` & `keras-nlp-0.5.0.dev0/examples/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/tools/split_sentences.py` & `keras-nlp-0.5.0.dev0/examples/tools/split_sentences.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/tools/train_word_piece_vocab.py` & `keras-nlp-0.5.0.dev0/examples/tools/train_word_piece_vocab.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/utils/__init__.py` & `keras-nlp-0.5.0.dev0/examples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/utils/data_utils.py` & `keras-nlp-0.5.0.dev0/examples/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/examples/utils/scripting_utils.py` & `keras-nlp-0.5.0.dev0/examples/utils/scripting_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,11 +19,12 @@
     import sentencepiece
 except ImportError:
     pass
 
 from keras_nlp import layers
 from keras_nlp import metrics
 from keras_nlp import models
+from keras_nlp import samplers
 from keras_nlp import tokenizers
 from keras_nlp import utils
 
-__version__ = "0.4.1.dev0"
+__version__ = "0.5.0.dev0"
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/benchmarks/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/conftest.py` & `keras-nlp-0.5.0.dev0/keras_nlp/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 import os
 import sys
 
 import pytest
 import tensorflow as tf
 from packaging import version
+from tensorflow import keras
 
 
 @pytest.fixture(scope="session")
 def tpu_strategy():
     tpu_name = os.getenv("KUBE_GOOGLE_CLOUD_TPU_ENDPOINTS")
     resolver = tf.distribute.cluster_resolver.TPUClusterResolver.connect(
         tpu=tpu_name,
@@ -49,17 +50,25 @@
     )
     parser.addoption(
         "--run_tpu",
         action="store_true",
         default=False,
         help="run tpu tests",
     )
+    parser.addoption(
+        "--mixed_precision",
+        action="store_true",
+        default=False,
+        help="run with mixed precision",
+    )
 
 
 def pytest_configure(config):
+    if config.getoption("--mixed_precision"):
+        keras.mixed_precision.set_global_policy("mixed_float16")
     config.addinivalue_line(
         "markers", "large: mark test as being slow or requiring a network"
     )
     config.addinivalue_line(
         "markers",
         "extra_large: mark test as being too large to run continuously",
     )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from keras_nlp.layers.cached_multi_head_attention import (
+    CachedMultiHeadAttention,
+)
 from keras_nlp.layers.f_net_encoder import FNetEncoder
 from keras_nlp.layers.masked_lm_head import MaskedLMHead
 from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
 from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
 from keras_nlp.layers.position_embedding import PositionEmbedding
 from keras_nlp.layers.random_deletion import RandomDeletion
 from keras_nlp.layers.random_swap import RandomSwap
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/f_net_encoder.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # limitations under the License.
 
 """FNet encoder block implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.keras_utils import clone_initializer
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.FNetEncoder")
 class FNetEncoder(keras.layers.Layer):
     """FNet encoder.
 
     This class follows the architecture of FNet encoder layer in the
     [FNet paper](https://arxiv.org/abs/2105.03824). Users can instantiate
     multiple instances of this class to stack up the encoder.
 
@@ -127,17 +128,17 @@
             A Tensor of the same shape as the `inputs`.
         """
 
         def fourier_transform(input):
             # Apply FFT on the input and take the real part.
             # Before we apply fourier transform, let's convert the dtype of the
             # input tensor to complex64.
-            input = tf.cast(input, tf.complex64)
-            mixing_output = tf.math.real(tf.signal.fft2d(input))
-            return mixing_output
+            x = tf.cast(input, tf.complex64)
+            mixing_output = tf.math.real(tf.signal.fft2d(x))
+            return tf.cast(mixing_output, input.dtype)
 
         def add_and_norm(input1, input2, norm_layer):
             return norm_layer(input1 + input2)
 
         def feed_forward(input):
             x = self._intermediate_dense(input)
             x = self._output_dense(x)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/f_net_encoder_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/f_net_encoder_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,13 +129,15 @@
                     intermediate_dim=4,
                 ),
             ]
         )
         data = tf.random.uniform(shape=[2, 4, 6])
         model(data)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model(data)
         loaded_model_output = loaded_model(data)
         self.assertAllClose(model_output, loaded_model_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_head.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 """Masked Language Model (MaskedLM) head."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-# TODO(mattdangerw): register this class as serializable.
+
+@keras_nlp_export("keras_nlp.layers.MaskedLMHead")
 class MaskedLMHead(keras.layers.Layer):
     """Masked Language Model (MaskedLM) head.
 
     This layer takes two inputs:
 
      - `inputs`: which should be a tensor of encoded tokens with shape
        `(batch_size, sequence_length, encoding_dim)`.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_head_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_head_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Transformer Encoder."""
 
 import os
 
 import tensorflow as tf
+from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.layers import masked_lm_head
 
 
-class MaskedLMHeadTest(tf.test.TestCase):
+class MaskedLMHeadTest(tf.test.TestCase, parameterized.TestCase):
     def test_valid_call(self):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
             activation="softmax",
         )
         encoded_tokens = keras.Input(shape=(10, 16))
         positions = keras.Input(shape=(5,), dtype="int32")
@@ -152,28 +153,34 @@
         save_path = checkpoint.save(self.get_temp_dir())
         checkpoint2.restore(save_path)
 
         head1_output = head1(token_data, mask_positions=position_data)
         head2_output = head2(token_data, mask_positions=position_data)
         self.assertAllClose(head1_output, head2_output)
 
-    def test_saving_model(self):
+    @parameterized.named_parameters(
+        ("tf_format", "tf", "model"),
+        ("keras_format", "keras_v3", "model.keras"),
+    )
+    def test_saved_model(self, save_format, filename):
         head = masked_lm_head.MaskedLMHead(
             vocabulary_size=100,
             activation="softmax",
         )
         encoded_tokens = keras.Input(shape=(10, 16))
         positions = keras.Input(shape=(5,), dtype="int32")
         outputs = head(encoded_tokens, mask_positions=positions)
         model = keras.Model((encoded_tokens, positions), outputs)
 
         token_data = tf.random.uniform(shape=(4, 10, 16))
         position_data = tf.random.uniform(
             shape=(4, 5), maxval=10, dtype="int32"
         )
         model_output = model((token_data, position_data))
-        save_path = os.path.join(self.get_temp_dir(), "model")
-        model.save(save_path)
-        restored = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
-        restored_output = restored((token_data, position_data))
+        restored_output = restored_model((token_data, position_data))
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_mask_generator.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.MaskedLMMaskGenerator")
 class MaskedLMMaskGenerator(keras.layers.Layer):
     """Layer that applies language model masking.
 
-    This layer is useful for preparing inputs for masked languaged modeling
+    This layer is useful for preparing inputs for masked language modeling
     (MaskedLM) tasks. It follows the masking strategy described in the [original BERT
     paper](https://arxiv.org/abs/1810.04805). Given tokenized text,
     it randomly selects certain number of tokens for masking. Then for each
     selected token, it has a chance (configurable) to be replaced by
     "mask token" or random token, or stay unchanged.
 
     Users should use this layer with `tf.data` to generate masks.
@@ -76,24 +77,50 @@
                 `mask_ids`. Each element in `mask_weights` should be 0 or 1,
                 1 means the corresponding position in `mask_positions` is an
                 actual mask, 0 means it is a pad.
 
     Examples:
 
     Basic usage.
-    >>> masker = keras_nlp.layers.MaskedLMMaskGenerator(
-    ...     vocabulary_size=10, mask_selection_rate=0.2, mask_token_id=0,
-    ...     mask_selection_length=5)
-    >>> masker(tf.constant([1, 2, 3, 4, 5]))
-
-    Ragged Input:
-    >>> masker = keras_nlp.layers.MaskedLMMaskGenerator(
-    ...     vocabulary_size=10, mask_selection_rate=0.5, mask_token_id=0,
-    ...     mask_selection_length=5)
-    >>> masker(tf.ragged.constant([[1, 2], [1, 2, 3, 4]]))
+    ```python
+    masker = keras_nlp.layers.MaskedLMMaskGenerator(
+        vocabulary_size=10,
+        mask_selection_rate=0.2,
+        mask_token_id=0,
+        mask_selection_length=5
+    )
+    # Dense input.
+    masker(tf.constant([1, 2, 3, 4, 5]))
+
+    # Ragged input.
+    masker(tf.ragged.constant([[1, 2], [1, 2, 3, 4]]))
+    ```
+
+    Masking a batch that contains special tokens.
+    ```python
+    pad_id, cls_id, sep_id, mask_id = 0, 1, 2, 3
+    batch = tf.constant([
+        [cls_id,   4,    5,      6, sep_id,    7,    8, sep_id, pad_id, pad_id],
+        [cls_id,   4,    5, sep_id,      6,    7,    8,      9, sep_id, pad_id],
+    ])
+
+    masker = keras_nlp.layers.MaskedLMMaskGenerator(
+        vocabulary_size = 10,
+        mask_selection_rate = 0.2,
+        mask_selection_length = 5,
+        mask_token_id = mask_id,
+        unselectable_token_ids = [
+            cls_id,
+            sep_id,
+            pad_id,
+        ]
+    )
+
+    masker(batch)
+    ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         mask_selection_rate,
         mask_token_id,
@@ -158,15 +185,15 @@
         )
 
         if not input_is_ragged:
             # If we converted the input from dense to ragged, convert back.
             token_ids = token_ids.to_tensor()
 
         mask_weights = tf.ones_like(mask_positions, self.compute_dtype)
-        # If mask_selection_length is set, covert to raggeds to dense.
+        # If `mask_selection_length` is set, convert to dense.
         if self.mask_selection_length:
             target_shape = tf.cast([-1, self.mask_selection_length], tf.int64)
             mask_positions = mask_positions.to_tensor(shape=target_shape)
             mask_ids = mask_ids.to_tensor(shape=target_shape)
             mask_weights = mask_weights.to_tensor(shape=target_shape)
 
         if input_is_1d:
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/masked_lm_mask_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/multi_segment_packer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # limitations under the License.
 
 """BERT token packing layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.MultiSegmentPacker")
 class MultiSegmentPacker(keras.layers.Layer):
     """Packs multiple sequences into a single fixed width model input.
 
     This layer packs multiple input sequences into a single fixed width sequence
     containing start and end delimeters, forming an dense input suitable for a
     classification task for BERT and BERT-like models.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/multi_segment_packer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/multi_segment_packer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,13 +174,15 @@
         inputs = (
             keras.Input(dtype="string", ragged=True, shape=(None,)),
             keras.Input(dtype="string", ragged=True, shape=(None,)),
         )
         outputs = packer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model((seq1, seq2)),
             restored_model((seq1, seq2)),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/position_embedding.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 
 """Position embedding implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-SEQUENCE_AXIS = -2
+from keras_nlp.api_export import keras_nlp_export
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.PositionEmbedding")
 class PositionEmbedding(keras.layers.Layer):
     """A layer which learns a position embedding for inputs sequences.
 
     This class assumes that in the input tensor, the last dimension corresponds
     to the features, and the dimension before the last corresponds to the
     sequence.
 
@@ -99,30 +99,37 @@
             shape=[self.sequence_length, feature_size],
             initializer=self.initializer,
             trainable=True,
         )
 
         super().build(input_shape)
 
-    def call(self, inputs):
+    def call(self, inputs, start_index=0):
         if isinstance(inputs, tf.RaggedTensor):
             bounding_shape = inputs.bounding_shape()
             position_embeddings = self._trim_and_broadcast_position_embeddings(
                 bounding_shape,
+                start_index,
             )
             # then apply row lengths to recreate the same ragged shape as inputs
             return tf.RaggedTensor.from_tensor(
                 position_embeddings,
                 inputs.nested_row_lengths(),
             )
         else:
             return self._trim_and_broadcast_position_embeddings(
                 tf.shape(inputs),
+                start_index,
             )
 
-    def _trim_and_broadcast_position_embeddings(self, shape):
-        input_length = shape[SEQUENCE_AXIS]
+    def _trim_and_broadcast_position_embeddings(self, shape, start_index):
+        feature_length = shape[-1]
+        sequence_length = shape[-2]
         # trim to match the length of the input sequence, which might be less
         # than the sequence_length of the layer.
-        position_embeddings = self.position_embeddings[:input_length, :]
+        position_embeddings = tf.slice(
+            self.position_embeddings,
+            (start_index, 0),
+            (sequence_length, feature_length),
+        )
         # then broadcast to add the missing dimensions to match "shape"
         return tf.broadcast_to(position_embeddings, shape)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/position_embedding_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/position_embedding_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         input_tensor = keras.Input(shape=(sequence_length, feature_size))
         output_tensor = test_layer(input_tensor)
 
         # When using static position embedding shapes, the output is expected
         # to be the same as the input shape in all dimensions save batch.
         expected_output_shape = [None, sequence_length, feature_size]
         self.assertEqual(expected_output_shape, output_tensor.shape.as_list())
-        # The default output dtype for this layer should be tf.float32.
-        self.assertEqual(tf.float32, output_tensor.dtype)
+        # The output dtype for this layer should match the compute dtype.
+        self.assertEqual(test_layer.compute_dtype, output_tensor.dtype)
 
     def test_more_than_3_dimensions_static(self):
         # Create a 4-dimensional input (the first dimension is implicit).
         sequence_length = 21
         feature_size = 30
         test_layer = position_embedding.PositionEmbedding(
             sequence_length=sequence_length
@@ -64,16 +64,16 @@
         expected_output_shape = [
             None,
             feature_size,
             sequence_length,
             feature_size,
         ]
         self.assertEqual(expected_output_shape, output_tensor.shape.as_list())
-        # The default output dtype for this layer should be tf.float32.
-        self.assertEqual(tf.float32, output_tensor.dtype)
+        # The output dtype for this layer should match the compute dtype.
+        self.assertEqual(test_layer.compute_dtype, output_tensor.dtype)
 
     def test_float16_dtype(self):
         # Create a 3-dimensional input (the first dimension is implicit).
         sequence_length = 21
         feature_size = 30
         test_layer = position_embedding.PositionEmbedding(
             sequence_length=sequence_length, dtype="float16"
@@ -280,32 +280,20 @@
         self.assertNotAllClose(
             trainable_variables_before, model.trainable_variables[0]
         )
 
     def test_get_config_and_from_config(self):
         max_sequence_length = 40
         test_layer = position_embedding.PositionEmbedding(
-            sequence_length=max_sequence_length
+            sequence_length=max_sequence_length,
+            initializer="zeros",
         )
         config = test_layer.get_config()
-        expected_config_subset = {
-            "sequence_length": max_sequence_length,
-            "initializer": {
-                "class_name": "GlorotUniform",
-                "config": {"seed": None},
-            },
-        }
-        self.assertEqual(config, {**config, **expected_config_subset})
-
-        restored_encoder = position_embedding.PositionEmbedding.from_config(
-            config,
-        )
-        self.assertEqual(
-            restored_encoder.get_config(), {**config, **expected_config_subset}
-        )
+        restored = position_embedding.PositionEmbedding.from_config(config)
+        self.assertEqual(restored.get_config(), config)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         max_sequence_length = 4
@@ -317,15 +305,17 @@
         outputs = test_layer(inputs)
         model = keras.Model(inputs=inputs, outputs=outputs)
 
         data = tf.zeros(shape=[2, max_sequence_length, feature_size])
         model(data)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model.predict(data)
         loaded_model_output = loaded_model.predict(data)
         self.assertAllClose(model_output, loaded_model_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/random_deletion.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import random
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+
+@keras_nlp_export("keras_nlp.layers.RandomDeletion")
 class RandomDeletion(keras.layers.Layer):
     """Augments input by randomly deleting tokens.
 
     This layer comes in handy when you need to generate new data using deletion
     augmentation as described in the paper [EDA: Easy Data Augmentation
     Techniques for Boosting Performance on Text Classification Tasks]
     (https://arxiv.org/pdf/1901.11196.pdf). The layer expects the inputs to be
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/random_deletion_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_deletion_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for RandomDeletion Layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers import RandomDeletion
+from keras_nlp.layers.random_deletion import RandomDeletion
 
 
 class RandomDeletionTest(tf.test.TestCase):
     def test_shape_and_output_from_word_deletion(self):
         keras.utils.set_random_seed(1337)
         inputs = ["Hey I like", "Keras and Tensorflow"]
         split = tf.strings.split(inputs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/random_swap.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import random
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
+
+@keras_nlp_export("keras_nlp.layers.RandomSwap")
 class RandomSwap(keras.layers.Layer):
     """Augments input by randomly swapping words.
 
     This layer comes in handy when you need to generate new data using swap
     augmentations as described in the paper [EDA: Easy Data Augmentation
     Techniques for Boosting Performance on Text Classification Tasks]
     (https://arxiv.org/pdf/1901.11196.pdf). The layer expects the inputs to be
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/random_swap_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/random_swap_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for RandomSwaps Layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers import RandomSwap
+from keras_nlp.layers.random_swap import RandomSwap
 
 
 class RandomSwapTest(tf.test.TestCase):
     def test_shape_and_output_from_word_swap(self):
         keras.utils.set_random_seed(1337)
         inputs = ["Hey I like", "Keras and Tensorflow"]
         split = tf.strings.split(inputs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/sine_position_encoding.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 """Sinusoidal position embedding layer."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+
+@keras_nlp_export("keras_nlp.layers.SinePositionEncoding")
 class SinePositionEncoding(keras.layers.Layer):
     """Sinusoidal positional encoding layer.
 
     This layer calculates the position encoding as a mix of sine and cosine
     functions with geometrically increasing wavelengths. Defined and formulized
     in [Attention is All You Need](https://arxiv.org/abs/1706.03762).
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/sine_position_encoding_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/sine_position_encoding_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,84 +75,75 @@
                 pos_encoding,
             ]
         )
         input = tf.random.uniform(shape=[1, 4, 6])
         output = model(input)
 
         # comapre position encoding values for position 0 and 3
-        expected_encoding_position_0 = [0.0, 1.0, 0.0, 1.0, 0.0, 1.0]
-        expected_encoding_position_3 = [
-            0.14112,
-            -0.9899925,
-            0.1387981,
-            0.9903207,
-            0.00646326,
-            0.99997914,
-        ]
-        self.assertAllClose(output[0, 0, :], expected_encoding_position_0)
-        self.assertAllClose(output[0, 3, :], expected_encoding_position_3)
+        expected_0 = [0.0, 1.0, 0.0, 1.0, 0.0, 1.0]
+        expected_3 = [0.14112, -0.98999, 0.13879, 0.99032, 0.00646, 0.99997]
+        self.assertAllClose(output[0, 0, :], expected_0, atol=0.01, rtol=0.01)
+        self.assertAllClose(output[0, 3, :], expected_3, atol=0.01, rtol=0.01)
 
     def test_ragged_tensor_with_3_dimensions(self):
         feature_size = 2
         test_layer = sine_position_encoding.SinePositionEncoding()
         # Create a 3-dimensional ragged input (the first dimension is implicit).
-        input_tensor = keras.Input(
-            shape=(None, feature_size), dtype=tf.float32, ragged=True
-        )
+        input_tensor = keras.Input(shape=(None, feature_size), ragged=True)
         output_tensor = test_layer(input_tensor)
         model = keras.Model(input_tensor, output_tensor)
 
-        input_data = tf.ragged.constant(
+        inputs = tf.ragged.constant(
             [
                 [[1.0, 1.0], [1.0, 1.0]],
                 [],
                 [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]],
                 [[1.0, 1.0]],
             ],
             ragged_rank=1,
             inner_shape=(2,),
         )
-        expected_output_data = tf.ragged.constant(
+        expected_outputs = tf.ragged.constant(
             [
                 [[0.0, 1.0], [0.84147096, 0.5403023]],
                 [],
                 [[0.0, 1.0], [0.84147096, 0.5403023], [0.9092974, -0.41614684]],
                 [[0.0, 1.0]],
             ],
             ragged_rank=1,
             inner_shape=(2,),
         )
-        output_data = model.predict(input_data)
-        self.assertAllClose(output_data, expected_output_data)
+        outputs = model.predict(inputs)
+        self.assertAllClose(outputs, expected_outputs, atol=0.01, rtol=0.01)
 
     def test_ragged_tensor_with_4_dimensions(self):
         feature_size = 2
         test_layer = sine_position_encoding.SinePositionEncoding()
         # Create a 4-dimensional ragged input (the first dimension is implicit).
         input_tensor = keras.Input(
-            shape=(None, None, feature_size), dtype=tf.float32, ragged=True
+            shape=(None, None, feature_size), ragged=True
         )
         output_tensor = test_layer(input_tensor)
         model = keras.Model(input_tensor, output_tensor)
 
-        input_data = tf.ragged.constant(
+        inputs = tf.ragged.constant(
             [
                 [
                     [[1.0, 1.0], [1.0, 1.0]],
                     [],
                 ],
                 [
                     [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]],
                     [[1.0, 1.0]],
                 ],
             ],
             ragged_rank=2,
             inner_shape=(2,),
         )
-        expected_output_data = tf.ragged.constant(
+        expected_outputs = tf.ragged.constant(
             [
                 [
                     [[0.0, 1.0], [0.84147096, 0.5403023]],
                     [],
                 ],
                 [
                     [
@@ -162,16 +153,16 @@
                     ],
                     [[0.0, 1.0]],
                 ],
             ],
             ragged_rank=2,
             inner_shape=(2,),
         )
-        output_data = model.predict(input_data)
-        self.assertAllClose(output_data, expected_output_data)
+        outputs = model.predict(inputs)
+        self.assertAllClose(outputs, expected_outputs, atol=0.01, rtol=0.01)
 
     def test_get_config_and_from_config(self):
         pos_encoding = sine_position_encoding.SinePositionEncoding(
             max_wavelength=1000,
         )
         config = pos_encoding.get_config()
         expected_config_subset = {
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/start_end_packer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,150 +8,125 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Start End Packer implementation based on `keras.layers.Layer`."""
+"""Creates an Embedding Layer and adds Positional Embeddings"""
 
-import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.position_embedding import PositionEmbedding
+from keras_nlp.utils.keras_utils import clone_initializer
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class StartEndPacker(keras.layers.Layer):
-    """Adds start and end tokens to a sequence and pads to a fixed length.
-
-    This layer is useful when tokenizing inputs for tasks like translation,
-    where each sequence should include a start and end marker. It should
-    be called after tokenization. The layer will first trim inputs to fit, then
-    add start/end tokens, and finally pad, if necessary, to `sequence_length`.
 
-    Input should be either a `tf.RaggedTensor` or a dense `tf.Tensor`, and
-    either rank-1 or rank-2.
+@keras_nlp_export("keras_nlp.layers.TokenAndPositionEmbedding")
+class TokenAndPositionEmbedding(keras.layers.Layer):
+    """A layer which sums a token and position embedding.
+
+    Token and position embeddings are ways of representing words and their order
+    in a sentence. This layer creates a `keras.layers.Embedding` token embedding
+    and a `keras_nlp.layers.PositionEmbedding` position embedding and sums their
+    output when called. This layer assumes that the last dimension in the input
+    corresponds to the sequence dimension.
 
     Args:
-        sequence_length: int. The desired output length.
-        start_value: int/str. The ID or token that is to be placed at the start
-            of each sequence. The dtype must match the dtype of the input
-            tensors to the layer. If None, no start value will be added.
-        end_value: int/str. The ID or token that is to be placed at the end of
-            each input segment. The dtype must match the dtype of the input
-            tensors to the layer. If None, no end value will be added.
-        pad_value: int/str. The ID or token that is to be placed into the
-            unused positions after the last segment in the sequence. If None,
-            0 or "" will be added depending on the dtype of the input tensor.
+        vocabulary_size: The size of the vocabulary.
+        sequence_length: The maximum length of input sequence
+        embedding_dim: The output dimension of the embedding layer
+        embeddings_initializer: The initializer to use for the Embedding
+            Layers
+        mask_zero: Boolean, whether or not the input value 0 is a special
+            "padding" value that should be masked out.
+            This is useful when using recurrent layers which may take variable
+            length input. If this is True, then all subsequent layers in the
+            model need to support masking or an exception will be raised.
+            If mask_zero` is set to True, as a consequence, index 0 cannot be
+            used in the vocabulary
+            (input_dim should equal size of vocabulary + 1).
 
     Examples:
-
-    Unbatched input (int).
-    >>> input_data = tf.constant([5, 6, 7])
-    >>> start_end_packer = keras_nlp.layers.StartEndPacker(
-    ...     sequence_length=7, start_value=1, end_value=2,
-    ... )
-    >>> start_end_packer(input_data)
-    <tf.Tensor: shape=(7,), dtype=int32, numpy=
-    array([1, 5, 6, 7, 2, 0, 0], dtype=int32)>
-
-    Batched input (int).
-    >>> input_data = tf.ragged.constant([[5, 6, 7], [8, 9, 10, 11, 12, 13, 14]])
-    >>> start_end_packer = keras_nlp.layers.StartEndPacker(
-    ...     sequence_length=6, start_value=1, end_value=2,
-    ... )
-    >>> start_end_packer(input_data)
-    <tf.Tensor: shape=(2, 6), dtype=int32, numpy=
-    array([[ 1,  5,  6,  7,  2,  0],
-           [ 1,  8,  9, 10, 11,  2]], dtype=int32)>
-
-    Unbatched input (str).
-    >>> input_data = tf.constant(["this", "is", "fun"])
-    >>> start_end_packer = keras_nlp.layers.StartEndPacker(
-    ...     sequence_length=6, start_value="<s>", end_value="</s>",
-    ...     pad_value="<pad>"
-    ... )
-    >>> start_end_packer(input_data)
-    <tf.Tensor: shape=(6,), dtype=string, numpy=
-    array([b'<s>', b'this', b'is', b'fun', b'</s>', b'<pad>'], dtype=object)>
-
-    Batched input (str).
-    >>> input_data = tf.ragged.constant([["this", "is", "fun"], ["awesome"]])
-    >>> start_end_packer = keras_nlp.layers.StartEndPacker(
-    ...     sequence_length=6, start_value="<s>", end_value="</s>",
-    ...     pad_value="<pad>"
-    ... )
-    >>> start_end_packer(input_data)
-    <tf.Tensor: shape=(2, 6), dtype=string, numpy=
-    array([[b'<s>', b'this', b'is', b'fun', b'</s>', b'<pad>'],
-           [b'<s>', b'awesome', b'</s>', b'<pad>', b'<pad>', b'<pad>']],
-          dtype=object)>
+    ```python
+    inputs = tf.ones(shape=(1, 50), dtype=tf.int64)
+    embedding_layer = keras_nlp.layers.TokenAndPositionEmbedding(
+        vocabulary_size=10_000,
+        sequence_length=50,
+        embedding_dim=128,
+    )
+    outputs = embedding_layer(inputs)
+    ```
     """
 
     def __init__(
         self,
+        vocabulary_size,
         sequence_length,
-        start_value=None,
-        end_value=None,
-        pad_value=None,
-        name=None,
-        **kwargs,
+        embedding_dim,
+        embeddings_initializer="glorot_uniform",
+        mask_zero=False,
+        **kwargs
     ):
-        super().__init__(name=name, **kwargs)
-
-        self.sequence_length = sequence_length
-        self.start_value = start_value
-        self.end_value = end_value
-        self.pad_value = pad_value
-
-    def call(self, inputs):
-        if not isinstance(inputs, (tf.Tensor, tf.RaggedTensor)):
-            inputs = tf.convert_to_tensor(inputs)
-
-        input_is_1d = False
-        if inputs.shape.rank < 1 or inputs.shape.rank > 2:
+        super().__init__(**kwargs)
+        if vocabulary_size is None:
+            raise ValueError(
+                "`vocabulary_size` must be an Integer, received `None`."
+            )
+        if sequence_length is None:
+            raise ValueError(
+                "`sequence_length` must be an Integer, received `None`."
+            )
+        if embedding_dim is None:
             raise ValueError(
-                "Input must either be rank 1 or rank 2. Received input with "
-                f"rank={inputs.shape.rank}"
+                "`embedding_dim` must be an Integer, received `None`."
             )
-        elif inputs.shape.rank == 1:
-            input_is_1d = True
-            # Add a new axis at the beginning.
-            inputs = tf.expand_dims(inputs, axis=0)
-        if isinstance(inputs, tf.Tensor):
-            # Convert to ragged tensor.
-            inputs = tf.RaggedTensor.from_tensor(inputs)
-
-        batch_size = tf.shape(inputs)[0]
-
-        # Concatenate start and end tokens.
-        if self.start_value is not None:
-            start_token_id_tensor = tf.fill((batch_size, 1), self.start_value)
-            inputs = tf.concat([start_token_id_tensor, inputs], axis=-1)
-        if self.end_value is not None:
-            end_token_id_tensor = tf.fill((batch_size, 1), self.end_value)
-
-            # Trim to leave room for end token.
-            inputs = inputs[..., : self.sequence_length - 1]
-            inputs = tf.concat([inputs, end_token_id_tensor], axis=-1)
-
-        # Pad to desired length.
-        inputs = inputs.to_tensor(
-            default_value=self.pad_value,
-            shape=(batch_size, self.sequence_length),
+        self.vocabulary_size = int(vocabulary_size)
+        self.sequence_length = int(sequence_length)
+        self.embedding_dim = int(embedding_dim)
+        self.embeddings_initializer = keras.initializers.get(
+            embeddings_initializer
         )
-
-        if input_is_1d:
-            inputs = tf.squeeze(inputs, axis=0)
-
-        return inputs
+        self.token_embedding = keras.layers.Embedding(
+            vocabulary_size,
+            embedding_dim,
+            embeddings_initializer=clone_initializer(
+                self.embeddings_initializer
+            ),
+            mask_zero=mask_zero,
+            name="token_embedding"
+            + str(keras.backend.get_uid("token_embedding")),
+        )
+        self.position_embedding = PositionEmbedding(
+            sequence_length=sequence_length,
+            initializer=clone_initializer(self.embeddings_initializer),
+            name="position_embedding"
+            + str(keras.backend.get_uid("position_embedding")),
+        )
+        self.supports_masking = self.token_embedding.supports_masking
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
+                "vocabulary_size": self.vocabulary_size,
                 "sequence_length": self.sequence_length,
-                "start_value": self.start_value,
-                "end_value": self.end_value,
-                "pad_value": self.pad_value,
-            }
+                "embedding_dim": self.embedding_dim,
+                "embeddings_initializer": keras.initializers.serialize(
+                    self.embeddings_initializer
+                ),
+                "mask_zero": self.token_embedding.mask_zero,
+            },
         )
         return config
+
+    def call(self, inputs, start_index=0):
+        embedded_tokens = self.token_embedding(inputs)
+        embedded_positions = self.position_embedding(
+            embedded_tokens,
+            start_index=start_index,
+        )
+        outputs = embedded_tokens + embedded_positions
+        return outputs
+
+    def compute_mask(self, inputs, mask=None):
+        return self.token_embedding.compute_mask(inputs, mask=mask)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/start_end_packer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/start_end_packer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,22 @@
         output = ds.take(1).get_single_element()
 
         exp_output = [[1, 5, 6, 7, 2, 3, 3], [1, 8, 9, 10, 11, 2, 3]]
 
         for i in range(output.shape[0]):
             self.assertAllEqual(output[i], exp_output[i])
 
+    def test_call_overrides(self):
+        x = tf.constant([5, 6, 7])
+        packer = StartEndPacker(start_value=1, end_value=2, sequence_length=4)
+        self.assertAllEqual(packer(x), [1, 5, 6, 2])
+        self.assertAllEqual(packer(x, add_start_value=False), [5, 6, 7, 2])
+        self.assertAllEqual(packer(x, add_end_value=False), [1, 5, 6, 7])
+        self.assertAllEqual(packer(x, sequence_length=2), [1, 2])
+
     def test_get_config(self):
         start_end_packer = StartEndPacker(
             sequence_length=512,
             start_value=10,
             end_value=20,
             pad_value=100,
             name="start_end_packer_test",
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/token_and_position_embedding_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/token_and_position_embedding_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.layers import TokenAndPositionEmbedding
+from keras_nlp.layers.token_and_position_embedding import (
+    TokenAndPositionEmbedding,
+)
 
 
 class TokenAndPositionEmbeddingTest(tf.test.TestCase, parameterized.TestCase):
     def test_get_config_and_from_config(self):
         token_and_position_embed = TokenAndPositionEmbedding(
             vocabulary_size=5,
             sequence_length=10,
@@ -144,13 +146,15 @@
         outputs = test_layer(inputs)
         model = keras.Model(inputs=inputs, outputs=outputs)
 
         data = tf.zeros(shape=[2, sequence_length])
         model(data)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model.predict(data)
         loaded_model_output = loaded_model.predict(data)
         self.assertAllClose(model_output, loaded_model_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_decoder.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 # limitations under the License.
 
 """Transformer decoder block implementation based on `keras.layers.Layer`."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.cached_multi_head_attention import (
+    CachedMultiHeadAttention,
+)
 from keras_nlp.utils.keras_utils import clone_initializer
 
 from keras_nlp.layers.transformer_layer_utils import (  # isort:skip
     compute_causal_mask,
     merge_padding_and_attention_mask,
 )
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.TransformerDecoder")
 class TransformerDecoder(keras.layers.Layer):
     """Transformer decoder.
 
     This class follows the architecture of the transformer decoder layer in the
     paper [Attention is All You Need](https://arxiv.org/abs/1706.03762). Users
     can instantiate multiple instances of this class to stack up a decoder.
 
@@ -137,15 +141,15 @@
         self._has_cross_attention = has_cross_attention
         # Infer the dimension of our hidden feature size from the build shape.
         hidden_dim = input_shape[-1]
         # Attention head size is `hidden_dim` over the number of heads.
         head_dim = int(hidden_dim // self.num_heads)
 
         # Self attention layers.
-        self._self_attention_layer = keras.layers.MultiHeadAttention(
+        self._self_attention_layer = CachedMultiHeadAttention(
             num_heads=self.num_heads,
             key_dim=head_dim,
             dropout=self.dropout,
             kernel_initializer=clone_initializer(self.kernel_initializer),
             bias_initializer=clone_initializer(self.bias_initializer),
         )
         self._self_attention_layer._build_from_signature(
@@ -204,14 +208,16 @@
         self,
         decoder_sequence,
         encoder_sequence=None,
         decoder_padding_mask=None,
         decoder_attention_mask=None,
         encoder_padding_mask=None,
         encoder_attention_mask=None,
+        cache=None,
+        cache_index=0,
     ):
         """Forward pass of the TransformerDecoder.
 
         Args:
             decoder_sequence: a Tensor. The decoder input sequence.
             encoder_sequence: a Tensor. The encoder input sequence. For decoder
                 only models (like GPT2), this should be left None. Once the
@@ -223,16 +229,22 @@
                 sequence mask, must of shape
                 [batch_size, decoder_sequence_length, decoder_sequence_length].
             encoder_padding_mask: a boolean Tensor, the padding mask of encoder
                 sequence, must of shape [batch_size, encoder_sequence_length].
             encoder_attention_mask: a boolean Tensor. Customized encoder
                 sequence mask, must of shape
                 [batch_size, encoder_sequence_length, encoder_sequence_length].
+            cache: a dense float Tensor. The cache of key/value of leading
+                tokens. `cache` is of shape [B, 2, max_seq_len, num_heads,
+                key_dims].
+            cache_index: a int or int Tensor, the index of the current token
+                being processed.
         Returns:
-            A Tensor of the same shape as the `decoder_sequence`.
+            Either a tuple of (outputs, cache) if a cache was passed, or a
+            single value outputs if a cache was not passed.
         """
 
         has_encoder_sequence = encoder_sequence is not None
         if not self._built:
             self._build(decoder_sequence.shape, has_encoder_sequence)
 
         is_cross_attention = self._cross_attention_layer is not None
@@ -256,28 +268,42 @@
                 "This layer has been built with cross attention, but "
                 "you did not provide encoder_sequence."
             )
 
         x = decoder_sequence  # Intermediate result.
 
         # Compute self attention mask.
-        self_attention_mask = compute_causal_mask(decoder_sequence)
+        batch_size = tf.shape(decoder_sequence)[0]
+        input_length = output_length = tf.shape(decoder_sequence)[1]
+        # We need to handle a rectangular causal mask when doing cached
+        # decoding. For generative inference, `decoder_sequence` will
+        # generally be length 1, and `cache` will be the full generation length.
+        if cache is not None:
+            input_length = tf.shape(cache)[2]
+        self_attention_mask = compute_causal_mask(
+            batch_size,
+            input_length,
+            output_length,
+            cache_index,
+        )
         decoder_mask = merge_padding_and_attention_mask(
             decoder_sequence, decoder_padding_mask, decoder_attention_mask
         )
         if decoder_mask is not None:
             self_attention_mask = tf.minimum(decoder_mask, self_attention_mask)
 
         # Self attention block.
         residual = x
         if self.normalize_first:
             x = self._self_attention_layernorm(x)
-        x = self._self_attention_layer(
+        x, cache = self._self_attention_layer(
             query=x,
             value=x,
+            cache=cache,
+            cache_index=cache_index,
             attention_mask=self_attention_mask,
         )
         x = self._self_attention_dropout(x)
         x = x + residual
         if not self.normalize_first:
             x = self._self_attention_layernorm(x)
 
@@ -309,15 +335,17 @@
         x = self._feedforward_intermediate_dense(x)
         x = self._feedforward_output_dense(x)
         x = self._feedforward_dropout(x)
         x = x + residual
         if not self.normalize_first:
             x = self._feedforward_layernorm(x)
 
-        return x
+        if cache is None:
+            return x
+        return (x, cache)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "intermediate_dim": self.intermediate_dim,
                 "num_heads": self.num_heads,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_decoder_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_decoder_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Tests for Transformer Decoder."""
 
 import os
 
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
+from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
 from keras_nlp.layers import transformer_decoder
 
 
 class TransformerDecoderTest(tf.test.TestCase, parameterized.TestCase):
     @parameterized.named_parameters(
         ("without_norm_first", False),
@@ -262,14 +263,64 @@
         decoder_sequence = tf.random.uniform(shape=[1, 4, 6])
         mask = tf.constant([[True, True, False, False]])
         decoder_sequence._keras_mask = mask
         outputs = decoder(decoder_sequence)
         self.assertAllEqual(outputs._keras_mask, mask)
 
     @parameterized.named_parameters(
+        ("graph", False),
+        ("eager", True),
+    )
+    def test_cached_decoding_is_correct(self, eager):
+        batch_size = 2
+        seq_len = 5
+        num_heads = 2
+        head_dim = 4
+
+        layer = transformer_decoder.TransformerDecoder(
+            intermediate_dim=4,
+            num_heads=num_heads,
+        )
+        dtype = layer.compute_dtype
+        x = tf.random.uniform(
+            shape=[batch_size, seq_len, num_heads * head_dim], dtype=dtype
+        )
+        cache = tf.zeros(
+            [batch_size, 2, seq_len, num_heads, head_dim], dtype=dtype
+        )
+        outputs = tf.zeros_like(x)
+
+        def call(outputs, cache):
+            def loop_body(i, outputs, cache):
+                # Compute the rest tokens.
+                next_input = x[:, i : i + 1, :]
+                next_output, cache = layer(
+                    decoder_sequence=next_input,
+                    cache=cache,
+                    cache_index=i,
+                )
+                outputs = dynamic_update_slice(outputs, next_output, [0, i, 0])
+                return i + 1, outputs, cache
+
+            _, outputs, cache = tf.while_loop(
+                cond=lambda i, outputs, cache: i < seq_len,
+                body=loop_body,
+                loop_vars=[0, outputs, cache],
+            )
+            return outputs, cache
+
+        call = call if eager else tf.function(call)
+        output, cache = call(outputs, cache)
+
+        no_loop_outputs = layer(x)
+        _, no_loop_cache = layer(x, cache=cache)
+        self.assertAllClose(output, no_loop_outputs)
+        self.assertAllClose(cache, no_loop_cache)
+
+    @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         encoder_input = keras.Input(shape=[4, 6])
         decoder_input = keras.Input(shape=[4, 6])
         decoder = transformer_decoder.TransformerDecoder(
@@ -282,15 +333,17 @@
             inputs=[decoder_input, encoder_input],
             outputs=output,
         )
         encoder_sequence = tf.random.uniform(shape=[2, 4, 6])
         decoder_sequence = tf.random.uniform(shape=[2, 4, 6])
         model([decoder_sequence, encoder_sequence])
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         loaded_model = keras.models.load_model(path)
         model_output = model([decoder_sequence, encoder_sequence])
         loaded_model_output = loaded_model([decoder_sequence, encoder_sequence])
         self.assertAllClose(model_output, loaded_model_output)
 
     @parameterized.named_parameters(
@@ -308,13 +361,15 @@
         model = keras.Model(
             inputs=decoder_input,
             outputs=output,
         )
         decoder_sequence = tf.random.uniform(shape=[2, 4, 6])
         model(decoder_sequence)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         loaded_model = keras.models.load_model(path)
 
         model_output = model(decoder_sequence)
         loaded_model_output = loaded_model(decoder_sequence)
         self.assertAllClose(model_output, loaded_model_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_encoder.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Transformer encoder block implementation based on `keras.layers.Layer`."""
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.keras_utils import clone_initializer
 
 from keras_nlp.layers.transformer_layer_utils import (  # isort:skip
     merge_padding_and_attention_mask,
 )
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.layers.TransformerEncoder")
 class TransformerEncoder(keras.layers.Layer):
     """Transformer encoder.
 
     This class follows the architecture of the transformer encoder layer in the
     paper [Attention is All You Need](https://arxiv.org/abs/1706.03762). Users
     can instantiate multiple instances of this class to stack up an encoder.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_encoder_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_encoder_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,12 +172,14 @@
                     normalize_first=True,
                 ),
             ]
         )
         data = tf.random.uniform(shape=[2, 4, 6])
         model_output = model(data)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         loaded_model = keras.models.load_model(path)
         loaded_model_output = loaded_model(data)
         self.assertAllClose(model_output, loaded_model_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/layers/transformer_layer_utils.py` & `keras-nlp-0.5.0.dev0/keras_nlp/layers/transformer_layer_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,49 +14,77 @@
 
 """ Utility functions for `TransformerEncoder` and `TransformerDecoder`."""
 
 import tensorflow as tf
 from absl import logging
 
 
-def compute_causal_mask(inputs):
-    input_shape = tf.shape(inputs)
-    batch_size, sequence_length = input_shape[0], input_shape[1]
-    i = tf.range(sequence_length)[:, tf.newaxis]
-    j = tf.range(sequence_length)
-    mask = tf.cast(i >= j, dtype="int32")
-    mask = tf.reshape(mask, (1, input_shape[1], input_shape[1]))
-    mult = tf.concat(
-        [
-            tf.expand_dims(batch_size, -1),
-            tf.constant([1, 1], dtype=tf.int32),
-        ],
-        axis=0,
-    )
-    return tf.tile(mask, mult)
+def _check_masks_shapes(inputs, padding_mask, attention_mask):
+    mask = padding_mask
+    if hasattr(inputs, "_keras_mask") and mask is None:
+        mask = inputs._keras_mask
+    if mask is not None:
+        if mask._rank() != 2:
+            raise ValueError(
+                "`padding_mask` should have shape "
+                "(batch_size, target_length). "
+                f"Received shape `{mask.shape}`."
+            )
+    if attention_mask is not None:
+        if attention_mask._rank() != 3:
+            raise ValueError(
+                "`attention_mask` should have shape "
+                "(batch_size, target_length, source_length). "
+                f"Received shape `{mask.shape}`."
+            )
+
+
+def compute_causal_mask(batch_size, input_length, output_length, cache_index=0):
+    """Compute a causal attention mask for a transformer decoder.
+
+    Args:
+        batch_size: batch size for the mask.
+        input_length: the length of key/value tensors in the attention layer.
+        output_length: the length of query tensors in the attention layer.
+        cache_index: the current index for cached generation. If passed, the
+            query sequence will be considered to start at `cache_index` rather
+            than zero. For example, a causal mask with `output_length=1` and
+            `cache_index=5` would allow the query tensor to attend to the first
+            five positions of the key/value tensors.
+
+    Return:
+        A causal attention mask with shape
+        `(batch_size, output_length, input_length)` that can be passed to a
+        attention layer.
+    """
+    i = tf.range(output_length)[:, tf.newaxis] + cache_index
+    j = tf.range(input_length)
+    mask = tf.cast(i >= j, dtype="int32")[tf.newaxis, :, :]
+    return tf.broadcast_to(mask, (batch_size, output_length, input_length))
 
 
 def merge_padding_and_attention_mask(
     inputs,
     padding_mask,
     attention_mask,
 ):
-    """Merge padding mask with users' customized mask.
+    """Merge the padding mask with a customized attention mask.
 
     Args:
         inputs: the input sequence.
         padding_mask: the 1D padding mask, of shape
             [batch_size, sequence_length].
         attention_mask: the 2D customized mask, of shape
             [batch_size, sequence1_length, sequence2_length].
 
     Return:
         A merged 2D mask or None. If only `padding_mask` is provided, the
         returned mask is padding_mask with one additional axis.
     """
+    _check_masks_shapes(inputs, padding_mask, attention_mask)
     mask = padding_mask
     if hasattr(inputs, "_keras_mask"):
         if mask is None:
             # If no padding mask is explicitly provided, we look for padding
             # mask from the input data.
             mask = inputs._keras_mask
         else:
@@ -69,12 +97,9 @@
         # (not including the batch axis).
         mask = tf.cast(mask[:, tf.newaxis, :], dtype=tf.int32)
     if attention_mask is not None:
         attention_mask = tf.cast(attention_mask, dtype=tf.int32)
         if mask is None:
             return attention_mask
         else:
-            return tf.minimum(
-                mask[:, tf.newaxis, :],
-                attention_mask,
-            )
+            return tf.minimum(mask, attention_mask)
     return mask
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/bleu.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import collections
 import math
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.tf_utils import tensor_to_list
 
 REPLACE_SUBSTRINGS = [
     ("<skipped>", ""),
     ("-\n", ""),
     ("\n", " "),
     ("&quot;", '"'),
@@ -45,15 +46,15 @@
     # If last character is "." or ",", add space.
     (r"[\.,]$", r" \0 \1"),
     # one space only between words
     (r"\s+", r" "),
 ]
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.metrics.Bleu")
 class Bleu(keras.metrics.Metric):
     """BLEU metric.
 
     This class implements the BLEU metric. BLEU is generally used to evaluate
     machine translation systems. By default, this implementation replicates
     SacreBLEU, but user-defined tokenizers can be passed to deal with other
     languages.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/bleu_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/bleu_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 """Tests for Bleu."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics import Bleu
-from keras_nlp.tokenizers import ByteTokenizer
+from keras_nlp.metrics.bleu import Bleu
+from keras_nlp.tokenizers.byte_tokenizer import ByteTokenizer
 
 
 class BleuTest(tf.test.TestCase):
     def test_initialization(self):
         bleu = Bleu()
         result = bleu.result()
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/edit_distance.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 """Edit Distance metric."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+
+@keras_nlp_export("keras_nlp.metrics.EditDistance")
 class EditDistance(keras.metrics.Metric):
     """Edit Distance metric.
 
     This class implements the edit distance metric, sometimes called
     Levenshtein Distance, as a `keras.metrics.Metric`. Essentially, edit
     distance is the least number of operations required to convert one string to
     another, where an operation can be one of substitution, deletion or
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/edit_distance_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/edit_distance_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for EditDistance."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics import EditDistance
+from keras_nlp.metrics.edit_distance import EditDistance
 
 
 class EditDistanceTest(tf.test.TestCase):
     def test_initialization(self):
         edit_distance = EditDistance()
         result = edit_distance.result()
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/perplexity.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 """Perplexity metric."""
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+
+@keras_nlp_export("keras_nlp.metrics.Perplexity")
 class Perplexity(keras.metrics.Metric):
     """Perplexity metric.
 
     This class implements the perplexity metric. In short, this class calculates
     the cross entropy loss and takes its exponent.
     Note: This implementation is not suitable for fixed-size windows.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/perplexity_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/perplexity_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for Perplexity."""
 
 import tensorflow as tf
 
-from keras_nlp.metrics import Perplexity
+from keras_nlp.metrics.perplexity import Perplexity
 
 
 class PerplexityTest(tf.test.TestCase):
     def test_vars_after_initializing_class(self):
         perplexity = Perplexity()
         self.assertEqual(perplexity.result().numpy(), 0.0)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_base.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_base.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_l.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ROUGE-L metric."""
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.metrics.rouge_base import RougeBase
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.metrics.RougeL")
 class RougeL(RougeBase):
     """ROUGE-L metric.
 
     This class implements the ROUGE-L variant of the ROUGE metric. The ROUGE-L
     metric is traditionally used for evaluating summarisation systems.
     Succinctly put, ROUGE-L is a score based on the length of the longest
     common subsequence present in the reference text and the hypothesis text.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_l_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_l_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for RougeL."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics import RougeL
+from keras_nlp.metrics.rouge_l import RougeL
 
 
 class RougeLTest(tf.test.TestCase):
     def setUp(self):
         super().setUp()
 
         def assertDictAlmostEqual(d1, d2, delta=1e-3, typecast_to_numpy=True):
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_n.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ROUGE-N metric."""
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.metrics.rouge_base import RougeBase
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.metrics.RogueN")
 class RougeN(RougeBase):
     """ROUGE-N metric.
 
     This class implements the ROUGE-N variant of the ROUGE metric. The ROUGE-N
     metric is traditionally used for evaluating summarisation systems.
     Succinctly put, ROUGE-N is a score based on the number of matching n-grams
     between the reference text and the hypothesis text.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/metrics/rouge_n_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/metrics/rouge_n_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for RougeN."""
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.metrics import RougeN
+from keras_nlp.metrics.rouge_n import RougeN
 
 
 class RougeNTest(tf.test.TestCase):
     def setUp(self):
         super().setUp()
 
         def assertDictAlmostEqual(d1, d2, delta=1e-3, typecast_to_numpy=True):
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,48 +18,87 @@
 from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
 from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
 from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
 from keras_nlp.models.bert.bert_backbone import BertBackbone
 from keras_nlp.models.bert.bert_classifier import BertClassifier
+from keras_nlp.models.bert.bert_masked_lm import BertMaskedLM
+from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+    BertMaskedLMPreprocessor,
+)
 from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
 from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.models.deberta_v3.deberta_v3_classifier import (
     DebertaV3Classifier,
 )
+from keras_nlp.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
+from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+    DebertaV3MaskedLMPreprocessor,
+)
 from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
 from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.models.distil_bert.distil_bert_classifier import (
     DistilBertClassifier,
 )
+from keras_nlp.models.distil_bert.distil_bert_masked_lm import (
+    DistilBertMaskedLM,
+)
+from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+    DistilBertMaskedLMPreprocessor,
+)
 from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
 from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.models.f_net.f_net_classifier import FNetClassifier
+from keras_nlp.models.f_net.f_net_masked_lm import FNetMaskedLM
+from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+    FNetMaskedLMPreprocessor,
+)
 from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
+from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.models.gpt2.gpt2_causal_lm import GPT2CausalLM
+from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
+    GPT2CausalLMPreprocessor,
+)
+from keras_nlp.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
+from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.models.opt.opt_backbone import OPTBackbone
+from keras_nlp.models.opt.opt_causal_lm import OPTCausalLM
+from keras_nlp.models.opt.opt_causal_lm_preprocessor import (
+    OPTCausalLMPreprocessor,
+)
+from keras_nlp.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
 from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.models.roberta.roberta_classifier import RobertaClassifier
+from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
 from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
 from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
 from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
     XLMRobertaClassifier,
 )
+from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm import (
+    XLMRobertaMaskedLM,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
+)
 from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
 from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
 )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 """ALBERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.position_embedding import PositionEmbedding
 from keras_nlp.layers.transformer_encoder import TransformerEncoder
 from keras_nlp.models.albert.albert_presets import backbone_presets
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.utils.python_utils import classproperty
 
 
 def albert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.AlbertBackbone")
 class AlbertBackbone(Backbone):
     """ALBERT encoder network.
 
     This class implements a bi-directional Transformer-based encoder as
     described in
     ["ALBERT: A Lite BERT for Self-supervised Learning of Language Representations"](https://arxiv.org/abs/1909.11942).
     ALBERT is a more efficient variant of BERT, and uses parameter reduction
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,114 +7,109 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for ALBERT backbone model."""
 
+"""Tests for FNet tokenizer."""
+
+import io
 import os
 
+import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
+from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
-class AlbertBackboneTest(tf.test.TestCase, parameterized.TestCase):
+class FNetTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = AlbertBackbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            num_groups=1,
-            num_inner_repetitions=1,
-            embedding_dim=16,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=3,
+            unk_id=0,
+            bos_id=4,
+            eos_id=5,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
         )
-        self.batch_size = 8
-        self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "segment_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-        }
-
-        self.input_dataset = tf.data.Dataset.from_tensor_slices(
-            self.input_batch
-        ).batch(2)
-
-    def test_valid_call_albert(self):
-        self.model(self.input_batch)
-
-        # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "albert_backbone")
-
-    def test_variable_sequence_length_call_albert(self):
-        for seq_length in (25, 50, 75):
-            input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "segment_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-            }
-            self.model(input_data)
+        self.proto = bytes_io.getvalue()
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+        self.tokenizer = FNetTokenizer(proto=self.proto)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
-
-    def test_error_for_invalid_num_groups(self):
+    def test_tokenize(self):
+        input_data = "the quick brown fox"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [2, 10, 6, 8])
+
+    def test_tokenize_batch(self):
+        input_data = tf.constant(["the quick brown fox", "the earth is round"])
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [[2, 10, 6, 8], [2, 7, 9, 11]])
+
+    def test_detokenize(self):
+        input_data = tf.constant([[2, 10, 6, 8]])
+        output = self.tokenizer.detokenize(input_data)
+        self.assertEqual(output, tf.constant(["the quick brown fox"]))
+
+    def test_vocabulary_size(self):
+        tokenizer = FNetTokenizer(proto=self.proto)
+        self.assertEqual(tokenizer.vocabulary_size(), 12)
+
+    def test_errors_missing_special_tokens(self):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=iter(["abc"]),
+            model_writer=bytes_io,
+            vocab_size=5,
+            pad_id=-1,
+            eos_id=-1,
+            bos_id=-1,
+        )
         with self.assertRaises(ValueError):
-            self.model = AlbertBackbone(
-                vocabulary_size=1000,
-                num_layers=3,
-                num_heads=2,
-                num_groups=2,
-                num_inner_repetitions=1,
-                embedding_dim=16,
-                hidden_dim=64,
-                intermediate_dim=128,
-            )
+            FNetTokenizer(proto=bytes_io.getvalue())
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, AlbertBackbone)
-
-        # Check that output matches.
-        restored_output = restored_model(self.input_batch)
-        self.assertAllClose(
-            model_output["pooled_output"], restored_output["pooled_output"]
+        input_data = tf.constant(["the quick brown fox"])
+
+        inputs = keras.Input(dtype="string", shape=())
+        outputs = self.tokenizer(inputs)
+        model = keras.Model(inputs, outputs)
+
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
+        restored_model = keras.models.load_model(path)
+        self.assertAllEqual(
+            model(input_data),
+            restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,206 +1,203 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ALBERT classification model."""
+"""BERT classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_backbone import albert_kernel_initializer
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_presets import backbone_presets
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.bert.bert_backbone import BertBackbone
+from keras_nlp.models.bert.bert_backbone import bert_kernel_initializer
+from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
+from keras_nlp.models.bert.bert_presets import backbone_presets
+from keras_nlp.models.bert.bert_presets import classifier_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class AlbertClassifier(Task):
-    """An end-to-end ALBERT model for classification tasks
-
-    This model attaches a classification head to a `keras_nlp.model.AlbertBackbone`
-    backbone, mapping from the backbone outputs to logit output suitable for
-    a classification task. For usage of this model with pre-trained weights, see
-    the `from_preset()` method.
+@keras_nlp_export("keras_nlp.models.BertClassifier")
+class BertClassifier(Task):
+    """An end-to-end BERT model for classification tasks.
+
+    This model attaches a classification head to a
+    `keras_nlp.model.BertBackbone` instance, mapping from the backbone outputs
+    to logits suitable for a classification task. For usage of this model with
+    pre-trained weights, use the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind.
 
     Args:
-        backbone: A `keras_nlp.models.AlertBackbone` instance.
+        backbone: A `keras_nlp.models.BertBackbone` instance.
         num_classes: int. Number of classes to predict.
-        dropout: float. The dropout probability value, applied after the dense
-            layer.
-        preprocessor: A `keras_nlp.models.AlbertPreprocessor` or `None`. If
+        preprocessor: A `keras_nlp.models.BertPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        dropout: float. The dropout probability value, applied after the dense
+            layer.
 
     Examples:
 
-    Example usage.
-    ```python
-    # Define the preprocessed inputs.
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "segment_ids": tf.constant(
-            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-    }
-    labels = [0, 3]
-
-    # Randomly initialize a ALBERT backbone.
-    backbone = AlbertBackbone(
-        vocabulary_size=1000,
-        num_layers=2,
-        num_heads=2,
-        embedding_dim=8,
-        hidden_dim=64,
-        intermediate_dim=128,
-        max_sequence_length=128,
-        name="encoder",
-    )
-
-    # Create a ALBERT classifier and fit your data.
-    classifier = keras_nlp.models.AlbertClassifier(
-        backbone,
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-
-    Raw string inputs with customized preprocessing.
+    Raw string data.
     ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
-    # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.AlbertPreprocessor.from_preset(
-        "albert_base_en_uncased",
-        sequence_length=128,
-    )
-
-    # Create a AlbertClassifier and fit your data.
-    classifier = keras_nlp.models.AlbertClassifier.from_preset(
-        "albert_base_en_uncased",
+    # Pretrained classifier.
+    classifier = keras_nlp.models.BertClassifier.from_preset(
+        "bert_base_en_uncased",
         num_classes=4,
-        preprocessor=preprocessor,
     )
+    classifier.fit(x=features, y=labels, batch_size=2)
+    classifier.predict(x=features, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate).
     classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
         "segment_ids": tf.constant(
             [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
     }
     labels = [0, 3]
 
-    # Create a ALBERT classifier and fit your data.
-    classifier = keras_nlp.models.AlbertClassifier.from_preset(
-        "albert_base_en_uncased",
+    # Pretrained classifier without preprocessing.
+    classifier = keras_nlp.models.BertClassifier.from_preset(
+        "bert_base_en_uncased",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.BertTokenizer(
+        vocabulary=vocab,
+    )
+    preprocessor = keras_nlp.models.BertPreprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
     )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    backbone = keras_nlp.models.BertBackbone(
+        vocabulary_size=30552,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
+    )
+    classifier = keras_nlp.models.BertClassifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
-        dropout=0.1,
+        num_classes,
         preprocessor=None,
+        activation=None,
+        dropout=0.1,
         **kwargs,
     ):
         inputs = backbone.input
         pooled = backbone(inputs)["pooled_output"]
         pooled = keras.layers.Dropout(dropout)(pooled)
         outputs = keras.layers.Dense(
             num_classes,
-            kernel_initializer=albert_kernel_initializer(),
+            kernel_initializer=bert_kernel_initializer(),
+            activation=activation,
             name="logits",
         )(pooled)
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
-        self._backbone = backbone
-        self._preprocessor = preprocessor
+        self.backbone = backbone
+        self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
         self.dropout = dropout
 
         # Default compilation
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(5e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
                 "dropout": self.dropout,
             }
         )
-
         return config
 
     @classproperty
     def backbone_cls(cls):
-        return AlbertBackbone
+        return BertBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return AlbertPreprocessor
+        return BertPreprocessor
 
     @classproperty
     def presets(cls):
-        return copy.deepcopy({**backbone_presets})
+        return copy.deepcopy({**backbone_presets, **classifier_presets})
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,150 +1,136 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for ALBERT classification model."""
+"""Tests for XLM-RoBERTa classification model."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_classifier import AlbertClassifier
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
+    XLMRobertaClassifier,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+    XLMRobertaPreprocessor,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
+)
 
 
-class AlbertClassifierTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = AlbertBackbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            embedding_dim=8,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-            name="encoder",
-        )
-
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
             vocab_size=10,
             model_type="WORD",
-            pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
-        )
-        self.proto = bytes_io.getvalue()
-
-        tokenizer = AlbertTokenizer(proto=self.proto)
-
-        self.preprocessor = AlbertPreprocessor(
-            tokenizer=tokenizer,
-            sequence_length=8,
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        self.preprocessor = XLMRobertaPreprocessor(
+            tokenizer=XLMRobertaTokenizer(proto=bytes_io.getvalue()),
+            sequence_length=5,
         )
-        self.classifier = AlbertClassifier(
-            self.backbone,
-            4,
-            preprocessor=self.preprocessor,
+        self.backbone = XLMRobertaBackbone(
+            vocabulary_size=10,
+            num_layers=2,
+            num_heads=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.classifier_no_preprocessing = AlbertClassifier(
+        self.classifier = XLMRobertaClassifier(
             self.backbone,
-            4,
-            preprocessor=None,
+            num_classes=4,
+            preprocessor=self.preprocessor,
+            # Check we handle serialization correctly.
+            activation=keras.activations.softmax,
+            hidden_dim=4,
         )
 
         self.raw_batch = tf.constant(
             [
                 "the quick brown fox.",
                 "the slow brown fox.",
-                "the smelly brown fox.",
-                "the old brown fox.",
             ]
         )
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            (self.raw_batch, tf.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
+    def test_classifier_predict(self):
+        preds1 = self.classifier.predict(self.raw_batch)
+        self.classifier.preprocessor = None
+        preds2 = self.classifier.predict(self.preprocessed_batch)
+        # Assert predictions match.
+        self.assertAllClose(preds1, preds2)
+        # Assert valid softmax output.
+        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
-
-    def test_albert_classifier_fit_default_compile(self):
+    def test_classifier_fit(self):
         self.classifier.fit(self.raw_dataset)
+        self.classifier.preprocessor = None
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_classifier_fit(self, jit_compile):
+    def test_classifier_fit_no_xla(self):
+        self.classifier.preprocessor = None
         self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+            loss="sparse_categorical_crossentropy",
+            jit_compile=False,
         )
-        self.classifier.fit(self.raw_dataset)
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.classifier)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.classifier.get_config(),
         )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
-    def test_saved_model(self, save_format, filename):
+    @pytest.mark.large  # Saving is slow, so mark these large.
+    def test_saving_model(self, save_format, filename):
         model_output = self.classifier.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.classifier.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, AlbertClassifier)
+        self.assertIsInstance(restored_model, XLMRobertaClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 
 """ALBERT masked LM model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.masked_lm_head import MaskedLMHead
 from keras_nlp.models.albert.albert_backbone import AlbertBackbone
 from keras_nlp.models.albert.albert_backbone import albert_kernel_initializer
 from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
 )
 from keras_nlp.models.albert.albert_presets import backbone_presets
 from keras_nlp.models.task import Task
+from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.AlbertMaskedLM")
 class AlbertMaskedLM(Task):
     """An end-to-end ALBERT model for the masked language modeling task.
 
     This model will train ALBERT on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` method.
@@ -51,68 +53,57 @@
         backbone: A `keras_nlp.models.AlbertBackbone` instance.
         preprocessor: A `keras_nlp.models.AlbertMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
     Example usage:
 
-    Raw string inputs and pretrained backbone.
+    Raw string data.
     ```python
-    # Create a dataset with raw string features. Labels are inferred.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
-    # Create a AlbertMaskedLM with a pretrained backbone and further train
-    # on an MLM task.
+    # Pretrained language model.
     masked_lm = keras_nlp.models.AlbertMaskedLM.from_preset(
         "albert_base_en_uncased",
     )
+    masked_lm.fit(x=features, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate).
     masked_lm.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    masked_lm.backbone.trainable = False
+    # Fit again.
     masked_lm.fit(x=features, batch_size=2)
     ```
 
-    Preprocessed inputs and custom backbone.
+    Preprocessed integer data.
     ```python
-    # Create a preprocessed dataset where 0 is the mask token.
-    preprocessed_features = {
-        "segment_ids": tf.constant(
-            [[1, 0, 0, 4, 0, 6, 7, 8]] * 2, shape=(2, 8)
-        ),
+    # Create preprocessed batch where 0 is the mask token.
+    features = {
         "token_ids": tf.constant(
             [[1, 2, 0, 4, 0, 6, 7, 8]] * 2, shape=(2, 8)
         ),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1]] * 2, shape=(2, 8)
         ),
-        "mask_positions": tf.constant([[2, 4]] * 2, shape=(2, 2))
+        "mask_positions": tf.constant([[2, 4]] * 2, shape=(2, 2)),
+        "segment_ids": tf.constant([[0, 0, 0, 0, 0, 0, 0, 0]] * 2, shape=(2, 8))
     }
     # Labels are the original masked values.
     labels = [[3, 5]] * 2
 
-    # Randomly initialize a ALBERT encoder
-    backbone = keras_nlp.models.AlbertBackbone(
-        vocabulary_size=1000,
-        num_layers=2,
-        num_heads=2,
-        embedding_dim=64,
-        hidden_dim=64,
-        intermediate_dim=128,
-        max_sequence_length=128)
-
-    # Create a ALBERT masked LM and fit the data.
-    masked_lm = keras_nlp.models.AlbertMaskedLM(
-        backbone,
+    masked_lm = keras_nlp.models.AlbertMaskedLM.from_preset(
+        "albert_base_en_uncased",
         preprocessor=None,
     )
-    masked_lm.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-        jit_compile=True
-    )
-    masked_lm.fit(x=preprocessed_features, y=labels, batch_size=2)
+    masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(self, backbone, preprocessor=None, **kwargs):
         inputs = {
             **backbone.input,
             "mask_positions": keras.Input(
@@ -137,14 +128,21 @@
             include_preprocessing=preprocessor is not None,
             **kwargs
         )
 
         self.backbone = backbone
         self.preprocessor = preprocessor
 
+        self.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            optimizer=keras.optimizers.Adam(5e-5),
+            weighted_metrics=keras.metrics.SparseCategoricalAccuracy(),
+            jit_compile=is_xla_compatible(self),
+        )
+
     @classproperty
     def backbone_cls(cls):
         return AlbertBackbone
 
     @classproperty
     def preprocessor_cls(cls):
         return AlbertMaskedLMPreprocessor
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ALBERT masked language model preprocessor layer."""
 
 from absl import logging
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
 from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.AlbertMaskedLMPreprocessor")
 class AlbertMaskedLMPreprocessor(AlbertPreprocessor):
     """ALBERT preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
     task. It is primarily intended for use with the
     `keras_nlp.models.AlbertMaskedLM` task model. Preprocessing will occur in
     multiple steps.
@@ -65,69 +65,55 @@
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
     preprocessor = keras_nlp.models.AlbertMaskedLMPreprocessor.from_preset(
         "albert_base_en_uncased"
     )
 
     # Tokenize and mask a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-
-    # Tokenize and mask a batch of sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
+    preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and mask a dataset of sentences.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((features))
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
-
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    vocab_data = tf.data.Dataset.from_tensor_slices(
-        ["the quick brown fox", "the earth is round"]
-    )
+    # Tokenize and mask a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
 
-    # Creating sentencepiece tokenizer for ALBERT LM preprocessor
-    bytes_io = io.BytesIO()
+    # Tokenize and mask sentence pairs.
+    # In this case, always convert input to tensors before calling the layer.
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+    ```
 
-    sentencepiece.SentencePieceTrainer.train(
-        sentence_iterator=vocab_data.as_numpy_iterator(),
-        model_writer=bytes_io,
-        vocab_size=12,
-        model_type="WORD",
-        pad_id=0,
-        unk_id=1,
-        bos_id=2,
-        eos_id=3,
-        pad_piece="<pad>",
-        unk_piece="<unk>",
-        bos_piece="[CLS]",
-        eos_piece="[SEP]",
-        user_defined_symbols="[MASK]"
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.AlbertMaskedLMPreprocessor.from_preset(
+        "albert_base_en_uncased"
     )
 
-    proto = bytes_io.getvalue()
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
 
-    tokenizer = AlbertTokenizer(proto=proto)
+    # Map single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    preprocessor = AlbertMaskedLMPreprocessor(
-        tokenizer=tokenizer
+    # Map sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
+    # Watch out for tf.data's default unpacking of tuples here!
+    # Best to invoke the `preprocessor` directly in this case.
+    ds = ds.map(
+        lambda first, second: preprocessor(x=(first, second)),
+        num_parallel_calls=tf.data.AUTOTUNE,
     )
-
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_masked_lm_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for ALBERT masked language model preprocessor layer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
     AlbertMaskedLMPreprocessor,
@@ -138,25 +139,36 @@
         self.assertAllEqual(
             x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0])
         self.assertAllEqual(y, [0, 0, 0, 0])
         self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0])
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_masked_lm_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,135 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for ALBERT masked language model."""
+"""Tests for RoBERTa masked language model."""
 
-import io
 import os
 
-import sentencepiece
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_backbone import AlbertBackbone
-from keras_nlp.models.albert.albert_masked_lm import AlbertMaskedLM
-from keras_nlp.models.albert.albert_masked_lm_preprocessor import (
-    AlbertMaskedLMPreprocessor,
+from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
+from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+    RobertaMaskedLMPreprocessor,
 )
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
-class AlbertMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
+class RobertaMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = AlbertBackbone(
-            vocabulary_size=1000,
+        self.vocab = {
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
+            "Ġkoh": 7,
+            "li": 8,
+            "Ġis": 9,
+            "Ġthe": 10,
+            "Ġbest": 11,
+            "<mask>": 12,
+        }
+
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+        self.merges = merges
+        self.preprocessor = RobertaMaskedLMPreprocessor(
+            RobertaTokenizer(vocabulary=self.vocab, merges=self.merges),
+            sequence_length=5,
+            mask_selection_length=2,
+        )
+        self.backbone = RobertaBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
-            embedding_dim=128,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-        )
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round", "an eagle flew"]
-        )
-
-        bytes_io = io.BytesIO()
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=15,
-            model_type="WORD",
-            pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
-        )
-
-        proto = bytes_io.getvalue()
-
-        tokenizer = AlbertTokenizer(proto=proto)
-
-        self.preprocessor = AlbertMaskedLMPreprocessor(
-            tokenizer=tokenizer,
-            # Simplify out testing by masking every available token.
-            mask_selection_rate=1.0,
-            mask_token_rate=1.0,
-            random_token_rate=0.0,
-            mask_selection_length=5,
-            sequence_length=12,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.masked_lm = AlbertMaskedLM(
+        self.masked_lm = RobertaMaskedLM(
             self.backbone,
             preprocessor=self.preprocessor,
         )
-        self.masked_lm_no_preprocessing = AlbertMaskedLM(
+        self.masked_lm_no_preprocessing = RobertaMaskedLM(
             self.backbone,
             preprocessor=None,
         )
 
         self.raw_batch = tf.constant(
             [
-                "quick brown fox",
-                "eagle flew over fox",
-                "the eagle flew quick",
-                "a brown eagle",
+                " airplane at airport",
+                " the airplane is the best",
             ]
         )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)[0]
+        self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
             self.raw_batch
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
-    def test_valid_call_masked_lm(self):
-        self.masked_lm(self.preprocessed_batch)
+    def test_valid_call_classifier(self):
+        self.masked_lm(self.preprocessed_batch[0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_masked_lm_predict(self, jit_compile):
-        self.masked_lm.compile(jit_compile=jit_compile)
+    def test_classifier_predict(self):
         self.masked_lm.predict(self.raw_batch)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.predict(self.preprocessed_batch[0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_masked_lm_predict_no_preprocessing(self, jit_compile):
-        self.masked_lm_no_preprocessing.compile(jit_compile=jit_compile)
-        self.masked_lm_no_preprocessing.predict(self.preprocessed_batch)
+    def test_classifier_fit(self):
+        self.masked_lm.fit(self.raw_dataset)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_masked_lm_fit(self, jit_compile):
-        self.masked_lm.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.masked_lm)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.masked_lm.get_config(),
         )
-        self.masked_lm.fit(self.raw_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_albert_masked_lm_fit_no_preprocessing(self, jit_compile):
-        self.masked_lm_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_classifier_fit_no_xla(self):
+        self.masked_lm.preprocessor = None
+        self.masked_lm.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
         )
-        self.masked_lm_no_preprocessing.fit(self.preprocessed_dataset)
+        self.masked_lm.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.masked_lm.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.masked_lm.predict(self.raw_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.masked_lm.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, AlbertMaskedLM)
-
-        model_output = self.masked_lm(self.preprocessed_batch)
-        restored_output = restored_model(self.preprocessed_batch)
+        self.assertIsInstance(restored_model, RobertaMaskedLM)
 
-        self.assertAllClose(model_output, restored_output)
+        # Check that output matches.
+        restored_output = restored_model.predict(self.raw_batch)
+        self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,43 +7,41 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ALBERT preprocessor layer."""
+"""DeBERTa preprocessor layer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.albert.albert_presets import backbone_presets
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class AlbertPreprocessor(Preprocessor):
-    """An ALBERT preprocessing layer which tokenizes and packs inputs.
+@keras_nlp_export("keras_nlp.models.DebertaV3Preprocessor")
+class DebertaV3Preprocessor(Preprocessor):
+    """A DeBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
      - Tokenize any number of input segments using the `tokenizer`.
      - Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
-       with the appropriate `"[CLS]"`, `"[SEP]"` and `"<pad>"` tokens.
-     - Construct a dictionary with keys `"token_ids"`, `"segment_ids"` and
-       `"padding_mask"`, that can be passed directly to
-       `keras_nlp.models.AlbertBackbone`.
+       with the appropriate `"[CLS]"`, `"[SEP]"` and `"[PAD]"` tokens.
+     - Construct a dictionary with keys `"token_ids"` and `"padding_mask"`, that
+       can be passed directly to a DeBERTa model.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
     The call method of this layer accepts three arguments, `x`, `y`, and
     `sample_weight`. `x` can be a python string or tensor representing a single
@@ -55,91 +53,98 @@
     Special care should be taken when using `tf.data` to map over an unlabeled
     tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
     directly into the call arguments of this layer, rather than forward all
     argument to `x`. To handle this case, it is recommended to  explicitly call
     the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
 
     Args:
-        tokenizer: A `keras_nlp.models.AlbertTokenizer` instance.
+        tokenizer: A `keras_nlp.models.DebertaV3Tokenizer` instance.
         sequence_length: The length of the packed inputs.
         truncate: string. The algorithm to truncate a list of batched segments
             to fit within `sequence_length`. The value can be either
             `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
     Examples:
+    Directly calling the layer on data.
     ```python
-    tokenizer = keras_nlp.models.AlbertTokenizer(proto="model.spm")
-    preprocessor = keras_nlp.models.AlbertPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=10,
+    preprocessor = keras_nlp.models.DebertaV3Preprocessor.from_preset(
+        "deberta_v3_base_en"
     )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
     preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
+
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+
+    # Custom vocabulary.
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(["The quick brown fox jumped."])
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=9,
+        model_type="WORD",
+        pad_id=0,
+        bos_id=1,
+        eos_id=2,
+        unk_id=3,
+        pad_piece="[PAD]",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        unk_piece="[UNK]",
     )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    tokenizer = keras_nlp.models.DebertaV3Tokenizer(
+        proto=bytes_io.getvalue(),
     )
+    preprocessor = keras_nlp.models.DebertaV3Preprocessor(tokenizer)
+    preprocessor("The quick brown fox jumped.")
+    ```
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.DebertaV3Preprocessor.from_preset(
+        "deberta_v3_base_en"
     )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
     def __init__(
         self,
@@ -167,22 +172,21 @@
             }
         )
         return config
 
     def call(self, x, y=None, sample_weight=None):
         x = convert_inputs_to_list_of_tensor_segments(x)
         x = [self.tokenizer(segment) for segment in x]
-        token_ids, segment_ids = self.packer(x)
+        token_ids, _ = self.packer(x)
         x = {
             "token_ids": token_ids,
-            "segment_ids": segment_ids,
             "padding_mask": token_ids != self.tokenizer.pad_token_id,
         }
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     @classproperty
     def tokenizer_cls(cls):
-        return AlbertTokenizer
+        return DebertaV3Tokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,169 +7,152 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Tests for BERT masked language model preprocessor layer."""
 
-"""Tests for ALBERT preprocessor layer."""
-
-import io
 import os
 
-import sentencepiece
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.models.bert.bert_masked_lm_preprocessor import (
+    BertMaskedLMPreprocessor,
+)
+from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
 
 
-class AlbertPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
+class BertMaskedLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=12,
-            model_type="WORD",
-            pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
-            pad_piece="<pad>",
-            unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            user_defined_symbols="[MASK]",
-        )
-        self.proto = bytes_io.getvalue()
-
-        self.preprocessor = AlbertPreprocessor(
-            tokenizer=AlbertTokenizer(proto=self.proto),
+        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
+        self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
+        self.vocab += ["the", "quick", "brown", "fox"]
+
+        tokenizer = BertTokenizer(vocabulary=self.vocab)
+
+        self.preprocessor = BertMaskedLMPreprocessor(
+            tokenizer=tokenizer,
+            # Simplify out testing by masking every available token.
+            mask_selection_rate=1.0,
+            mask_token_rate=1.0,
+            random_token_rate=0.0,
+            mask_selection_length=4,
             sequence_length=12,
         )
 
-    def test_tokenize_strings(self):
+    def test_preprocess_strings(self):
         input_data = "the quick brown fox"
-        output = self.preprocessor(input_data)
+
+        x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]
+            x["token_ids"], [2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(
-            output["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
+            x["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 3, 4])
+        self.assertAllEqual(y, [9, 10, 11, 12])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
 
-    def test_tokenize_list_of_strings(self):
-        # We should handle a list of strings as as batch.
+    def test_preprocess_list_of_strings(self):
         input_data = ["the quick brown fox"] * 4
-        output = self.preprocessor(input_data)
-        self.assertAllEqual(
-            output["token_ids"],
-            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
-        )
-        self.assertAllEqual(
-            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
-        )
-        self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
-        )
 
-    def test_tokenize_labeled_batch(self):
-        x = tf.constant(["the quick brown fox"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
+        x, y, sw = self.preprocessor(input_data)
         self.assertAllEqual(
-            x_out["token_ids"],
-            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
+            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4,
         )
-        self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
-        )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
+        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
 
-    def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["the quick brown fox"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
+    def test_preprocess_dataset(self):
+        sentences = tf.constant(["the quick brown fox"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(sentences)
         ds = ds.map(self.preprocessor)
-        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
-        self.assertAllEqual(
-            x_out["token_ids"],
-            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
-        )
+        x, y, sw = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
+            x["token_ids"], [[2, 4, 4, 4, 4, 3, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
+            x["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        self.assertAllEqual(x["mask_positions"], [[1, 2, 3, 4]] * 4)
+        self.assertAllEqual(y, [[9, 10, 11, 12]] * 4)
+        self.assertAllEqual(sw, [[1.0, 1.0, 1.0, 1.0]] * 4)
 
-    def test_tokenize_multiple_sentences(self):
-        sentence_one = tf.constant("the quick brown fox")
-        sentence_two = tf.constant("the earth")
-        output = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(
-            output["token_ids"],
-            [2, 5, 10, 6, 8, 3, 5, 7, 3, 0, 0, 0],
-        )
+    def test_mask_multiple_sentences(self):
+        sentence_one = tf.constant("the quick")
+        sentence_two = tf.constant("brown fox")
+
+        x, y, sw = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["segment_ids"], [0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]
+            x["token_ids"], [2, 4, 4, 3, 4, 4, 3, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+            x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         )
+        self.assertAllEqual(x["mask_positions"], [1, 2, 4, 5])
+        self.assertAllEqual(y, [9, 10, 11, 12])
+        self.assertAllEqual(sw, [1.0, 1.0, 1.0, 1.0])
 
-    def test_tokenize_multiple_batched_sentences(self):
-        sentence_one = tf.constant(["the quick brown fox"] * 4)
-        sentence_two = tf.constant(["the earth"] * 4)
-        # The first tuple or list is always interpreted as an enumeration of
-        # separate sequences to concatenate.
-        output = self.preprocessor((sentence_one, sentence_two))
-        self.assertAllEqual(
-            output["token_ids"],
-            [[2, 5, 10, 6, 8, 3, 5, 7, 3, 0, 0, 0]] * 4,
+    def test_no_masking_zero_rate(self):
+        no_mask_preprocessor = BertMaskedLMPreprocessor(
+            self.preprocessor.tokenizer,
+            mask_selection_rate=0.0,
+            mask_selection_length=4,
+            sequence_length=12,
         )
+        input_data = "the quick brown fox"
+
+        x, y, sw = no_mask_preprocessor(input_data)
         self.assertAllEqual(
-            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]] * 4
+            x["token_ids"], [2, 9, 10, 11, 12, 3, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4
+            x["padding_mask"],
+            [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0],
         )
+        self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0])
+        self.assertAllEqual(y, [0, 0, 0, 0])
+        self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0])
 
-    def test_errors_for_2d_list_input(self):
-        ambiguous_input = [["one", "two"], ["three", "four"]]
-        with self.assertRaises(ValueError):
-            self.preprocessor(ambiguous_input)
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
+
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
+
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
         restored_model = keras.models.load_model(path)
-        self.assertAllEqual(
-            model(input_data)["token_ids"],
-            restored_model(input_data)["token_ids"],
-        )
+        outputs = model(input_data)[0]["token_ids"]
+        restored_outputs = restored_model(input_data)[0]["token_ids"]
+        self.assertAllEqual(outputs, restored_outputs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             "description": (
                 "12-layer ALBERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 11683584,
             "official_name": "ALBERT",
             "path": "albert",
+            "model_card": "https://github.com/google-research/albert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30000,
             "num_layers": 12,
             "num_heads": 12,
             "num_groups": 1,
             "num_inner_repetitions": 1,
@@ -49,14 +50,15 @@
             "description": (
                 "24-layer ALBERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 17683968,
             "official_name": "ALBERT",
             "path": "albert",
+            "model_card": "https://github.com/google-research/albert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30000,
             "num_layers": 24,
             "num_heads": 16,
             "num_groups": 1,
             "num_inner_repetitions": 1,
@@ -78,14 +80,15 @@
             "description": (
                 "24-layer ALBERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 58724864,
             "official_name": "ALBERT",
             "path": "albert",
+            "model_card": "https://github.com/google-research/albert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30000,
             "num_layers": 24,
             "num_heads": 16,
             "num_groups": 1,
             "num_inner_repetitions": 1,
@@ -107,14 +110,15 @@
             "description": (
                 "12-layer ALBERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 222595584,
             "official_name": "ALBERT",
             "path": "albert",
+            "model_card": "https://github.com/google-research/albert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30000,
             "num_layers": 12,
             "num_heads": 64,
             "num_groups": 1,
             "num_inner_repetitions": 1,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_presets_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = AlbertClassifier.from_preset(
             "albert_base_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
         )
         # We don't assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
@@ -67,14 +68,15 @@
         input_data = {
             "token_ids": tf.constant([[101, 1996, 4248, 102]]),
             "segment_ids": tf.constant([[0, 0, 0, 0]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = AlbertClassifier.from_preset(
             "albert_base_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
@@ -103,23 +105,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("albert_tokenizer", AlbertTokenizer),
-        ("albert_preprocessor", AlbertPreprocessor),
-        ("albert", AlbertBackbone),
-        ("albert_classifier", AlbertClassifier),
+        ("albert_tokenizer", AlbertTokenizer, {}),
+        ("albert_preprocessor", AlbertPreprocessor, {}),
+        ("albert", AlbertBackbone, {}),
+        ("albert_classifier", AlbertClassifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("albert_base_en_uncased_clowntown")
+            cls.from_preset("albert_base_en_uncased_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
 class AlbertPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
     This tests every ALBERT preset and is only run manually.
@@ -149,26 +151,28 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_albert_classifier(self, load_weights):
         for preset in AlbertClassifier.presets:
             classifier = AlbertClassifier.from_preset(
                 preset,
+                num_classes=2,
                 load_weights=load_weights,
             )
             input_data = tf.constant(["This quick brown fox"])
             classifier.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_albert_classifier_without_preprocessing(self, load_weights):
         for preset in AlbertClassifier.presets:
             classifier = AlbertClassifier.from_preset(
                 preset,
+                num_classes=2,
                 preprocessor=None,
                 load_weights=load_weights,
             )
             input_data = {
                 "token_ids": tf.random.uniform(
                     shape=(1, 512),
                     dtype=tf.int64,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ALBERT tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.albert.albert_presets import backbone_presets
 from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.AlbertTokenizer")
 class AlbertTokenizer(SentencePieceTokenizer):
     """ALBERT tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
     underlying tokenizer, it will check for all special tokens needed by
     ALBERT models and provides a `from_preset()` method to automatically
@@ -48,24 +47,48 @@
             `bytes` object with a serialized SentencePiece proto. See the
             [SentencePiece repository](https://github.com/google/sentencepiece)
             for more details on the format.
 
     Examples:
 
     ```python
-    tokenizer = keras_nlp.models.AlbertTokenizer(proto="model.spm")
-
-    # Batched inputs.
-    tokenizer(["the quick brown fox", "the earth is round"])
+    # Unbatched input.
+    tokenizer = keras_nlp.models.AlbertTokenizer.from_preset(
+        "albert_base_en_uncased",
+    )
+    tokenizer("The quick brown fox jumped.")
 
-    # Unbatched inputs.
-    tokenizer("the quick brown fox")
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
-    tokenizer.detokenize(tf.constant([[2, 14, 2231, 886, 2385, 3]]))
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(["The quick brown fox jumped."])
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=10,
+        model_type="WORD",
+        pad_id=0,
+        unk_id=1,
+        bos_id=2,
+        eos_id=3,
+        pad_piece="<pad>",
+        unk_piece="<unk>",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        user_defined_symbols="[MASK]",
+    )
+    tokenizer = keras_nlp.models.AlbertTokenizer(
+        proto=bytes_io.getvalue(),
+    )
+    tokenizer("The quick brown fox jumped.")
     ```
     """
 
     def __init__(self, proto, **kwargs):
         super().__init__(proto=proto, **kwargs)
 
         # Check for necessary special tokens.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/albert/albert_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/t5_tokenizer_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,96 +8,107 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for ALBERT tokenizer."""
+"""Tests for T5 tokenizer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
+from keras_nlp.models.t5.t5_tokenizer import T5Tokenizer
 
 
-class AlbertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
+class T5TokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=12,
+            vocab_size=11,
             model_type="WORD",
+            bos_id=-1,
             pad_id=0,
-            unk_id=1,
-            bos_id=2,
-            eos_id=3,
+            eos_id=1,
+            unk_id=2,
             pad_piece="<pad>",
+            eos_piece="</s>",
             unk_piece="<unk>",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
             user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.tokenizer = AlbertTokenizer(proto=self.proto)
+        self.tokenizer = T5Tokenizer(proto=self.proto)
 
     def test_tokenize(self):
         input_data = "the quick brown fox"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [5, 10, 6, 8])
+        self.assertAllEqual(output, [4, 9, 5, 7])
 
     def test_tokenize_batch(self):
         input_data = tf.constant(["the quick brown fox", "the earth is round"])
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[5, 10, 6, 8], [5, 7, 9, 11]])
+        self.assertAllEqual(output, [[4, 9, 5, 7], [4, 6, 8, 10]])
 
     def test_detokenize(self):
-        input_data = tf.constant([[5, 10, 6, 8]])
+        input_data = tf.constant([[4, 9, 5, 7]])
         output = self.tokenizer.detokenize(input_data)
         self.assertEqual(output, tf.constant(["the quick brown fox"]))
 
     def test_vocabulary_size(self):
-        tokenizer = AlbertTokenizer(proto=self.proto)
-        self.assertEqual(tokenizer.vocabulary_size(), 12)
+        tokenizer = T5Tokenizer(proto=self.proto)
+        self.assertEqual(tokenizer.vocabulary_size(), 11)
 
     def test_errors_missing_special_tokens(self):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=iter(["abc"]),
             model_writer=bytes_io,
             vocab_size=5,
             pad_id=-1,
             eos_id=-1,
             bos_id=-1,
         )
         with self.assertRaises(ValueError):
-            AlbertTokenizer(proto=bytes_io.getvalue())
+            T5Tokenizer(proto=bytes_io.getvalue())
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/backbone.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 
         weights = keras.utils.get_file(
             "model.h5",
             metadata["weights_url"],
             cache_subdir=os.path.join("models", preset),
             file_hash=metadata["weights_hash"],
         )
-
         model.load_weights(weights)
         return model
 
     def __init_subclass__(cls, **kwargs):
         # Use __init_subclass__ to setup a correct docstring for from_preset.
         super().__init_subclass__(**kwargs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         ),
         "decoder_token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "decoder_padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0], shape=(1, 12)
         ),
     }
 
+    # Pretrained BART encoder.
+    model = keras_nlp.models.BartBackbone.from_preset("bart_base_en")
+    model(input_data)
+
     # Randomly initialized BART encoder-decoder model with a custom config
     model = keras_nlp.models.BartBackbone(
         vocabulary_size=50265,
         num_layers=6,
         num_heads=12,
         hidden_dim=768,
         intermediate_dim=3072,
@@ -232,25 +236,28 @@
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.intermediate_dim = intermediate_dim
         self.dropout = dropout
         self.max_sequence_length = max_sequence_length
 
     def get_config(self):
-        return {
-            "vocabulary_size": self.vocabulary_size,
-            "num_layers": self.num_layers,
-            "num_heads": self.num_heads,
-            "hidden_dim": self.hidden_dim,
-            "intermediate_dim": self.intermediate_dim,
-            "dropout": self.dropout,
-            "max_sequence_length": self.max_sequence_length,
-            "name": self.name,
-            "trainable": self.trainable,
-        }
+        config = super().get_config()
+        config.update(
+            {
+                "vocabulary_size": self.vocabulary_size,
+                "num_layers": self.num_layers,
+                "num_heads": self.num_heads,
+                "hidden_dim": self.hidden_dim,
+                "intermediate_dim": self.intermediate_dim,
+                "dropout": self.dropout,
+                "max_sequence_length": self.max_sequence_length,
+            }
+        )
+
+        return config
 
     @property
     def token_embedding(self):
         return self.get_layer("token_embedding")
 
     @classproperty
     def presets(cls):
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_backbone_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,17 +93,19 @@
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.model.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, BartBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,60 +11,62 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BART model preset configurations."""
 
 backbone_presets = {
     "bart_base_en": {
+        "metadata": {
+            "description": (
+                "6-layer BART model where case is maintained. "
+                "Trained on BookCorpus, English Wikipedia and CommonCrawl."
+            ),
+            "params": 139417344,
+            "official_name": "BART",
+            "path": "bart",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/bart/README.md",
+        },
         "config": {
             "vocabulary_size": 50265,
             "num_layers": 6,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "6-layer BART model where case is maintained. "
-                "Trained on BookCorpus, English Wikipedia and CommonCrawl."
-            ),
-            "params": 139417344,
-            "official_name": "BART",
-            "path": "bart",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/bart_base_en/v1/model.h5",
         "weights_hash": "5b59403f0cafafbd89680e0785791163",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/bart_base_en/v1/vocab.json",
         "vocabulary_hash": "be4d3c6f3f5495426b2c03b334334354",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/bart_base_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
     "bart_large_en": {
+        "metadata": {
+            "description": (
+                "12-layer BART model where case is maintained. "
+                "Trained on BookCorpus, English Wikipedia and CommonCrawl."
+            ),
+            "params": 406287360,
+            "official_name": "BART",
+            "path": "bart",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/bart/README.md",
+        },
         "config": {
             "vocabulary_size": 50265,
             "num_layers": 12,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "12-layer BART model where case is maintained. "
-                "Trained on BookCorpus, English Wikipedia and CommonCrawl."
-            ),
-            "params": 406287360,
-            "official_name": "BART",
-            "path": "bart",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/bart_large_en/v1/model.h5",
         "weights_hash": "6bfe7e591af8c5699ce6f9f18753af9a",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/bart_large_en/v1/vocab.json",
         "vocabulary_hash": "cf410ee085c5c69c957bb1f6d8456596",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/bart_large_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,105 +8,105 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""BART tokenizer."""
+"""OPT tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
-from keras_nlp.models.bart.bart_presets import backbone_presets
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.opt.opt_presets import backbone_presets
 from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class BartTokenizer(BytePairTokenizer):
-    """A BART tokenizer using Byte-Pair Encoding subword segmentation.
+@keras_nlp_export("keras_nlp.models.OPTTokenizer")
+class OPTTokenizer(BytePairTokenizer):
+    """An OPT tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by BART
+    underlying tokenizer, it will check for all special tokens needed by OPT
     models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a BART preset.
+    a matching vocabulary for a OPT preset.
 
-    This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.BartPreprocessor` layer for input
-    packing.
+    This tokenizer does not provide truncation or padding of inputs.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
-
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
         vocabulary: string or dict, maps token to integer ids. If it is a
             string, it should be the file path to a json file.
         merges: string or list, contains the merge rule. If it is a string,
             it should be the file path to merge rules. The merge rule file
             should have one merge rule per line. Every merge rule contains
             merge entities separated by a space.
 
     Examples:
 
     Batched inputs.
-    >>> vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    >>> vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    >>> vocab = {"<pad>": 1, "</s>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
     >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
     >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.RobertaTokenizer(
-    ...     vocabulary=vocab, merges=merges
+    >>> tokenizer = keras_nlp.models.OPTTokenizer(
+    ...     vocabulary=vocab,
+    ...     merges=merges,
     ... )
     >>> tokenizer(["a quick fox", "a fox quick"])
-    <tf.RaggedTensor [[4, 5, 6], [4, 6, 5]]>
+    <tf.RaggedTensor [[3, 4, 5], [3, 5, 4]]>
 
     Unbatched input.
-    >>> vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    >>> vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    >>> vocab = {"<pad>": 1, "</s>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
     >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
     >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.RobertaTokenizer(
-    ...     vocabulary=vocab, merges=merges
+    >>> tokenizer = keras_nlp.models.OPTTokenizer(
+    ...     vocabulary=vocab,
+    ...     merges=merges,
     ... )
     >>> tokenizer("a quick fox")
-    <tf.Tensor: shape=(3,), dtype=int32, numpy=array([4, 5, 6], dtype=int32)>
+    <tf.Tensor: shape=(4,), dtype=int32, numpy=array([3, 4, 5], dtype=int32)>
 
     Detokenization.
-    >>> vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    >>> vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    >>> vocab = {"<pad>": 1, "</s>": 2, "Ġquick": 4, "Ġfox": 5}
     >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
     >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.RobertaTokenizer(
-    ...     vocabulary=vocab, merges=merges
+    >>> tokenizer = keras_nlp.models.OPTTokenizer(
+    ...     vocabulary=vocab,
+    ...     merges=merges,
     ... )
-    >>> tokenizer.detokenize(tokenizer("a quick fox")).numpy().decode('utf-8')
-    'a quick fox'
+    >>> tokenizer.detokenize(tokenizer(" quick fox")).numpy().decode('utf-8')
+    ' quick fox'
     """
 
     def __init__(
         self,
         vocabulary,
         merges,
         **kwargs,
     ):
+        # Special tokens. We use `"</s>"` as both a start and end token, as OPT
+        # was only pre-trained with `"</s>"` marking document boundaries.
+        start_token = "</s>"
+        pad_token = "<pad>"
+        end_token = "</s>"
+
         super().__init__(
             vocabulary=vocabulary,
             merges=merges,
+            unsplittable_tokens=[start_token, pad_token, end_token],
             **kwargs,
         )
 
-        # Check for necessary special tokens.
-        start_token = "<s>"
-        pad_token = "<pad>"
-        end_token = "</s>"
+        # Check whether special tokens are present in the vocabulary.
         for token in [start_token, pad_token, end_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
@@ -114,7 +114,15 @@
         self.start_token_id = self.token_to_id(start_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.end_token_id = self.token_to_id(end_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bart/bart_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         self.tokenizer = BartTokenizer(vocabulary=vocab, merges=merges)
 
     def test_tokenize(self):
         input_data = " airplane at airport"
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [3, 4, 5, 3, 6])
 
+    def test_tokenize_special_tokens(self):
+        input_data = "<s> airplane at airport</s><pad>"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [0, 3, 4, 5, 3, 6, 0, 1])
+
     def test_tokenize_batch(self):
         input_data = tf.constant([" airplane at airport", " kohli is the best"])
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [[3, 4, 5, 3, 6], [7, 8, 9, 10, 11]])
 
     def test_detokenize(self):
         input_tokens = [[3, 4, 5, 3, 6]]
@@ -77,14 +82,16 @@
         input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 """BERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.position_embedding import PositionEmbedding
 from keras_nlp.layers.transformer_encoder import TransformerEncoder
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.bert.bert_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
 def bert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.BertBackbone")
 class BertBackbone(Backbone):
-    """BERT encoder network.
+    """A BERT encoder network.
 
     This class implements a bi-directional Transformer-based encoder as
     described in ["BERT: Pre-training of Deep Bidirectional Transformers for
     Language Understanding"](https://arxiv.org/abs/1810.04805). It includes the
     embedding lookups and transformer layers, but not the masked language model
     or next sentence prediction heads.
 
-    The default constructor gives a fully customizable, randomly initialized BERT
-    encoder with any number of layers, heads, and embedding dimensions. To load
-    preset architectures and weights, use the `from_preset` constructor.
+    The default constructor gives a fully customizable, randomly initialized
+    BERT encoder with any number of layers, heads, and embedding dimensions. To
+    load preset architectures and weights, use the `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind.
 
     Args:
         vocabulary_size: int. The size of the token vocabulary.
         num_layers: int. The number of transformer layers.
@@ -71,28 +72,28 @@
             [0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
     }
 
-    # Pretrained BERT encoder
+    # Pretrained BERT encoder.
     model = keras_nlp.models.BertBackbone.from_preset("bert_base_en_uncased")
-    output = model(input_data)
+    model(input_data)
 
-    # Randomly initialized BERT encoder with a custom config
+    # Randomly initialized BERT encoder with a custom config.
     model = keras_nlp.models.BertBackbone(
         vocabulary_size=30552,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_backbone_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,83 +21,73 @@
 from tensorflow import keras
 
 from keras_nlp.models.bert.bert_backbone import BertBackbone
 
 
 class BertBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = BertBackbone(
-            vocabulary_size=1000,
+        self.backbone = BertBackbone(
+            vocabulary_size=10,
             num_layers=2,
             num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=5,
         )
-        self.batch_size = 8
         self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "segment_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "segment_ids": tf.ones((2, 5), dtype="int32"),
+            "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
-
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_bert(self):
-        self.model(self.input_batch)
+        self.backbone(self.input_batch)
+
+    def test_token_embedding(self):
+        output = self.backbone.token_embedding(self.input_batch["token_ids"])
+        self.assertEqual(output.shape, (2, 5, 2))
 
+    def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "bert_backbone")
+        self.assertRegexpMatches(self.backbone.name, "bert_backbone")
 
     def test_variable_sequence_length_call_bert(self):
-        for seq_length in (25, 50, 75):
+        for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "segment_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "segment_ids": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
             }
-            self.model(input_data)
+            self.backbone(input_data)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+    def test_predict(self):
+        self.backbone.predict(self.input_batch)
+        self.backbone.predict(self.input_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+    def test_serialization(self):
+        new_backbone = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.backbone)
+        )
+        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.backbone(self.input_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.backbone.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, BertBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(
@@ -106,15 +96,15 @@
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
 class BertBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.model = BertBackbone(
+            self.backbone = BertBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
@@ -124,9 +114,9 @@
             "padding_mask": tf.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
-        self.model.compile()
-        self.model.predict(self.input_dataset)
+        self.backbone.compile()
+        self.backbone.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,216 +7,214 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""BERT classification model."""
+"""DistilBERT classification model."""
 
 import copy
 
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_backbone import bert_kernel_initializer
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_presets import backbone_presets
-from keras_nlp.models.bert.bert_presets import classifier_presets
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
+from keras_nlp.models.distil_bert.distil_bert_backbone import (
+    distilbert_kernel_initializer,
+)
+from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
+    DistilBertPreprocessor,
+)
+from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class BertClassifier(Task):
-    """An end-to-end BERT model for classification tasks
-
-    This model attaches a classification head to a `keras_nlp.model.BertBackbone`
-    backbone, mapping from the backbone outputs to logit output suitable for
-    a classification task. For usage of this model with pre-trained weights, see
-    the `from_preset()` method.
+@keras_nlp_export("keras_nlp.models.DistilBertClassifier")
+class DistilBertClassifier(Task):
+    """An end-to-end DistilBERT model for classification tasks.
+
+    This model attaches a classification head to a
+    `keras_nlp.model.DistilBertBackbone` instance, mapping from the backbone
+    outputs to logits suitable for a classification task. For usage of
+    this model with pre-trained weights, see the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
-    warranties or conditions of any kind.
+    warranties or conditions of any kind. The underlying model is provided by a
+    third party and subject to a separate license, available
+    [here](https://github.com/huggingface/transformers).
 
     Args:
-        backbone: A `keras_nlp.models.BertBackbone` instance.
+        backbone: A `keras_nlp.models.DistilBert` instance.
         num_classes: int. Number of classes to predict.
-        dropout: float. The dropout probability value, applied after the dense
-            layer.
-        preprocessor: A `keras_nlp.models.BertPreprocessor` or `None`. If
+        preprocessor: A `keras_nlp.models.DistilBertPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. The dropout probability value, applied after the first
+            dense layer.
 
     Examples:
 
-    Example usage.
+    Raw string data.
     ```python
-    # Define the preprocessed inputs.
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "segment_ids": tf.constant(
-            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-    }
-    labels = [0, 3]
-
-    # Randomly initialize a BERT backbone.
-    backbone = keras_nlp.models.BertBackbone(
-        vocabulary_size=30552,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
-    )
-
-    # Create a BERT classifier and fit your data.
-    classifier = keras_nlp.models.BertClassifier(
-        backbone,
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-    ```
-
-    Raw string inputs.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
-
-    # Create a BertClassifier and fit your data.
-    classifier = keras_nlp.models.BertClassifier.from_preset(
-        "bert_base_en_uncased",
-        num_classes=4,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Raw string inputs with customized preprocessing.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
     # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.BertPreprocessor.from_preset(
-        "bert_base_en_uncased",
+    preprocessor = keras_nlp.models.DistilBertPreprocessor.from_preset(
+        "distil_bert_base_en_uncased",
         sequence_length=128,
     )
-
-    # Create a BertClassifier and fit your data.
-    classifier = keras_nlp.models.BertClassifier.from_preset(
-        "bert_base_en_uncased",
+    # Pretrained classifier.
+    classifier = keras_nlp.models.DistilBertClassifier.from_preset(
+        "distil_bert_base_en_uncased",
         num_classes=4,
         preprocessor=preprocessor,
     )
+    classifier.fit(x=features, y=labels, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate)
     classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "segment_ids": tf.constant(
-            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
     }
     labels = [0, 3]
 
-    # Create a BERT classifier and fit your data.
-    classifier = keras_nlp.models.BertClassifier.from_preset(
-        "bert_base_en_uncased",
+    # Pretrained classifier without preprocessing.
+    classifier = keras_nlp.models.DistilBertClassifier.from_preset(
+        "distil_bert_base_en_uncased",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.DistilBertTokenizer(
+        vocabulary=vocab,
+    )
+    preprocessor = keras_nlp.models.DistilBertPreprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
+    )
+    backbone = keras_nlp.models.DistilBertBackbone(
+        vocabulary_size=30552,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
+    )
+    classifier = keras_nlp.models.DistilBertClassifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
-        dropout=0.1,
+        num_classes,
         preprocessor=None,
+        activation=None,
+        hidden_dim=None,
+        dropout=0.2,
         **kwargs,
     ):
         inputs = backbone.input
-        pooled = backbone(inputs)["pooled_output"]
-        pooled = keras.layers.Dropout(dropout)(pooled)
+        hidden_dim = hidden_dim or backbone.hidden_dim
+
+        x = backbone(inputs)[:, backbone.cls_token_index, :]
+        x = keras.layers.Dense(
+            hidden_dim,
+            activation="relu",
+            kernel_initializer=distilbert_kernel_initializer(),
+            name="pooled_dense",
+        )(x)
+        x = keras.layers.Dropout(dropout, name="classifier_dropout")(x)
         outputs = keras.layers.Dense(
             num_classes,
-            kernel_initializer=bert_kernel_initializer(),
+            kernel_initializer=distilbert_kernel_initializer(),
+            activation=activation,
             name="logits",
-        )(pooled)
+        )(x)
+
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
+        self.hidden_dim = hidden_dim
         self.dropout = dropout
 
-        # Default compilation
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(5e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
+                "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
     @classproperty
     def backbone_cls(cls):
-        return BertBackbone
+        return DistilBertBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return BertPreprocessor
+        return DistilBertPreprocessor
 
     @classproperty
     def presets(cls):
-        return copy.deepcopy({**backbone_presets, **classifier_presets})
+        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,134 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for BERT classification model."""
+"""Tests for XLM-RoBERTa masked language model."""
 
+import io
 import os
 
+import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_backbone import BertBackbone
-from keras_nlp.models.bert.bert_classifier import BertClassifier
-from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm import (
+    XLMRobertaMaskedLM,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
+)
 
 
-class BertClassifierTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = BertBackbone(
-            vocabulary_size=1000,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the slow brown fox"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=5,
+            model_type="WORD",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="<s>",
+            eos_piece="</s>",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+
+        self.preprocessor = XLMRobertaMaskedLMPreprocessor(
+            XLMRobertaTokenizer(proto=self.proto),
+            sequence_length=5,
+            mask_selection_length=2,
+        )
+
+        self.backbone = XLMRobertaBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-            name="encoder",
-        )
-        self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
-        self.vocab += ["the", "quick", "brown", "fox", "."]
-        self.preprocessor = BertPreprocessor(
-            BertTokenizer(vocabulary=self.vocab),
-            sequence_length=8,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.classifier = BertClassifier(
+
+        self.masked_lm = XLMRobertaMaskedLM(
             self.backbone,
-            4,
             preprocessor=self.preprocessor,
         )
-        self.classifier_no_preprocessing = BertClassifier(
-            self.backbone,
-            4,
-            preprocessor=None,
-        )
 
         self.raw_batch = tf.constant(
-            [
-                "the quick brown fox.",
-                "the slow brown fox.",
-                "the smelly brown fox.",
-                "the old brown fox.",
-            ]
+            ["the quick brown fox", "the slow brown fox"]
         )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)
+        self.preprocessed_batch = self.preprocessor(self.raw_batch)[0]
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            self.raw_batch
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
-    def test_valid_call_classifier(self):
-        self.classifier(self.preprocessed_batch)
+    def test_valid_call_masked_lm(self):
+        self.masked_lm(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_bert_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_bert_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
-
-    def test_bert_classifier_fit_default_compile(self):
-        self.classifier.fit(self.raw_dataset)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_bert_classifier_fit(self, jit_compile):
-        self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_classifier_predict(self):
+        self.masked_lm.predict(self.raw_batch)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.predict(self.preprocessed_batch)
+
+    def test_classifier_fit(self):
+        self.masked_lm.fit(self.raw_dataset)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.fit(self.preprocessed_dataset)
+
+    def test_classifier_fit_no_xla(self):
+        self.masked_lm.preprocessor = None
+        self.masked_lm.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
+        )
+        self.masked_lm.fit(self.preprocessed_dataset)
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.masked_lm)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.masked_lm.get_config(),
         )
-        self.classifier.fit(self.raw_dataset)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_bert_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
-        )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.classifier.predict(self.raw_batch)
         save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
+        self.masked_lm.save(save_path, save_format=save_format)
         restored_model = keras.models.load_model(save_path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, BertClassifier)
+        self.assertIsInstance(restored_model, XLMRobertaMaskedLM)
+
+        model_output = self.masked_lm(self.preprocessed_batch)
+        restored_output = restored_model(self.preprocessed_batch)
 
-        # Check that output matches.
-        restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,146 +11,125 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BERT preprocessor layer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
 from keras_nlp.models.bert.bert_presets import backbone_presets
 from keras_nlp.models.bert.bert_presets import classifier_presets
 from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.BertPreprocessor")
 class BertPreprocessor(Preprocessor):
     """A BERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
-     - Tokenize any number of input segments using the `tokenizer`.
-     - Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
+    1. Tokenize any number of input segments using the `tokenizer`.
+    2. Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
        with the appropriate `"[CLS]"`, `"[SEP]"` and `"[PAD]"` tokens.
-     - Construct a dictionary with keys `"token_ids"`, `"segment_ids"`,
+    3. Construct a dictionary with keys `"token_ids"`, `"segment_ids"`,
        `"padding_mask"`, that can be passed directly to a BERT model.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
-    The call method of this layer accepts three arguments, `x`, `y`, and
-    `sample_weight`. `x` can be a python string or tensor representing a single
-    segment, a list of python strings representing a batch of single segments,
-    or a list of tensors representing multiple segments to be packed together.
-    `y` and `sample_weight` are both optional, can have any format, and will be
-    passed through unaltered.
-
-    Special care should be taken when using `tf.data` to map over an unlabeled
-    tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
-    directly into the call arguments of this layer, rather than forward all
-    argument to `x`. To handle this case, it is recommended to  explicitly call
-    the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
-
     Args:
         tokenizer: A `keras_nlp.models.BertTokenizer` instance.
         sequence_length: The length of the packed inputs.
         truncate: string. The algorithm to truncate a list of batched segments
             to fit within `sequence_length`. The value can be either
             `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
+    Call arguments:
+        x: A tensor of single string sequences, or a tuple of multiple
+            tensor sequences to be packed together. Inputs may be batched or
+            unbatched. For single sequences, raw python inputs will be converted
+            to tensors. For multiple sequences, pass tensors directly.
+        y: Any label data. Will be passed through unaltered.
+        sample_weight: Any label weight data. Will be passed through unaltered.
+
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.BertPreprocessor.from_preset("bert_base_en_uncased")
+    preprocessor = keras_nlp.models.BertPreprocessor.from_preset(
+        "bert_base_en_uncased"
+    )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
     preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+
+    # Custom vocabulary.
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
+    preprocessor = keras_nlp.models.BertPreprocessor(tokenizer)
+    preprocessor("The quick brown fox jumped.")
+    ```
+
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.BertPreprocessor.from_preset(
+        "bert_base_en_uncased"
     )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
-
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as shown above.
-    vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]"]
-    vocab += ["The", "qu", "##ick", "br", "##own", "fox", "tripped"]
-    vocab += ["Call", "me", "Ish", "##mael", "."]
-    vocab += ["Oh", "look", "a", "whale"]
-    vocab += ["I", "forgot", "my", "home", "##work"]
-    tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
-    preprocessor = keras_nlp.models.BertPreprocessor(tokenizer)
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for BERT preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
 from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
 
@@ -107,23 +108,34 @@
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["THE QUICK BROWN FOX."])
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             "description": (
                 "2-layer BERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 4385920,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 2,
             "num_heads": 2,
             "hidden_dim": 128,
             "intermediate_dim": 512,
@@ -49,14 +50,15 @@
             "description": (
                 "4-layer BERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 28763648,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 4,
             "num_heads": 8,
             "hidden_dim": 512,
             "intermediate_dim": 2048,
@@ -77,14 +79,15 @@
             "description": (
                 "8-layer BERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 41373184,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 8,
             "num_heads": 8,
             "hidden_dim": 512,
             "intermediate_dim": 2048,
@@ -105,14 +108,15 @@
             "description": (
                 "12-layer BERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 109482240,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -133,14 +137,15 @@
             "description": (
                 "12-layer BERT model where case is maintained. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 108310272,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 28996,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -160,14 +165,15 @@
         "metadata": {
             "description": (
                 "12-layer BERT model. Trained on Chinese Wikipedia."
             ),
             "params": 102267648,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 21128,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -187,14 +193,15 @@
         "metadata": {
             "description": (
                 "12-layer BERT model where case is maintained. Trained on trained on Wikipedias of 104 languages"
             ),
             "params": 177853440,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 119547,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -215,14 +222,15 @@
             "description": (
                 "24-layer BERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 335141888,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
@@ -243,14 +251,15 @@
             "description": (
                 "24-layer BERT model where case is maintained. "
                 "Trained on English Wikipedia + BooksCorpus."
             ),
             "params": 333579264,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "vocabulary_size": 28996,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
@@ -273,14 +282,15 @@
         "metadata": {
             "description": (
                 "The bert_tiny_en_uncased backbone model fine-tuned on the SST-2 sentiment analysis dataset."
             ),
             "params": 4385920,
             "official_name": "BERT",
             "path": "bert",
+            "model_card": "https://github.com/google-research/bert/blob/master/README.md",
         },
         "config": {
             "backbone": {
                 "class_name": "keras_nlp>BertBackbone",
                 "config": {
                     "vocabulary_size": 30522,
                     "hidden_dim": 128,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_presets_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = BertClassifier.from_preset(
             "bert_tiny_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
         )
         # We don't assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
@@ -92,29 +93,30 @@
         input_data = {
             "token_ids": tf.constant([[101, 1996, 4248, 102]]),
             "segment_ids": tf.constant([[0, 0, 0, 0]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = BertClassifier.from_preset(
             "bert_tiny_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
-        ("bert_tokenizer", BertTokenizer),
-        ("bert_preprocessor", BertPreprocessor),
-        ("bert", BertBackbone),
-        ("bert_classifier", BertClassifier),
+        ("bert_tokenizer", BertTokenizer, {}),
+        ("bert_preprocessor", BertPreprocessor, {}),
+        ("bert", BertBackbone, {}),
+        ("bert_classifier", BertClassifier, {"num_classes": 2}),
     )
-    def test_preset_mutability(self, cls):
+    def test_preset_mutability(self, cls, kwargs):
         preset = "bert_tiny_en_uncased"
-        obj = cls.from_preset(preset)
+        obj = cls.from_preset(preset, **kwargs)
         # Cannot overwrite the presents attribute in an object
         with self.assertRaises(AttributeError):
             obj.presets = {"my_model": "clowntown"}
         # Cannot mutate presents in an object
         config = obj.presets[preset]["config"]
         config["num_layers"] = 1
         self.assertEqual(config["num_layers"], 1)
@@ -135,23 +137,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("bert_tokenizer", BertTokenizer),
-        ("bert_preprocessor", BertPreprocessor),
-        ("bert", BertBackbone),
-        ("bert_classifier", BertClassifier),
+        ("bert_tokenizer", BertTokenizer, {}),
+        ("bert_preprocessor", BertPreprocessor, {}),
+        ("bert", BertBackbone, {}),
+        ("bert_classifier", BertClassifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("bert_base_uncased_clowntown")
+            cls.from_preset("bert_base_uncased_clowntown", **kwargs)
 
     def test_override_preprocessor_sequence_length(self):
         """Override sequence length longer than model's maximum."""
         preprocessor = BertPreprocessor.from_preset(
             "bert_base_en_uncased",
             sequence_length=64,
         )
@@ -170,15 +172,15 @@
 @pytest.mark.extra_large
 class BertPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
 
     This every presets for BERT and is only run manually.
     Run with:
-    `pytest keras_nlp/models/bert_presets_test.py --run_extra_large`
+    `pytest keras_nlp/models/bert/bert_presets_test.py --run_extra_large`
     """
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_bert(self, load_weights):
         for preset in BertBackbone.presets:
@@ -197,26 +199,28 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_bert_classifier(self, load_weights):
         for preset in BertClassifier.presets:
             classifier = BertClassifier.from_preset(
                 preset,
+                num_classes=2,
                 load_weights=load_weights,
             )
             input_data = tf.constant(["This quick brown fox"])
             classifier.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_bert_classifier_without_preprocessing(self, load_weights):
         for preset in BertClassifier.presets:
             classifier = BertClassifier.from_preset(
                 preset,
+                num_classes=2,
                 preprocessor=None,
                 load_weights=load_weights,
             )
             input_data = {
                 "token_ids": tf.random.uniform(
                     shape=(1, 512),
                     dtype=tf.int64,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """BERT tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.bert.bert_presets import backbone_presets
 from keras_nlp.models.bert.bert_presets import classifier_presets
 from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 PRESET_NAMES = ", ".join(list(backbone_presets) + list(classifier_presets))
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.BertTokenizer")
 class BertTokenizer(WordPieceTokenizer):
     """A BERT tokenizer using WordPiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.WordPieceTokenizer`. Unlike the
     underlying tokenizer, it will check for all special tokens needed by BERT
     models and provides a `from_preset()` method to automatically download
@@ -49,38 +48,33 @@
             passing a list, each element of the list should be a single word
             piece token string. If passing a filename, the file should be a
             plain text file containing a single word piece token per line.
         lowercase: If true, the input text will be first lowered before
             tokenization.
 
     Examples:
-
-    Batched input.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = ["The quick brown fox.", "The fox."]
-    >>> tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
-    >>> tokenizer(inputs)
-    <tf.RaggedTensor [[4, 5, 6, 7, 8, 9], [4, 8, 9]]>
-
-    Unbatched input.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = "The fox."
-    >>> tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
-    >>> tokenizer(inputs)
-    <tf.Tensor: shape=(3,), dtype=int32, numpy=array([4, 8, 9], dtype=int32)>
-
-    Detokenization.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = "The quick brown fox."
-    >>> tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
-    >>> tokenizer.detokenize(tokenizer.tokenize(inputs)).numpy().decode('utf-8')
-    'The quick brown fox .'
+    ```python
+    # Unbatched input.
+    tokenizer = keras_nlp.models.BertTokenizer.from_preset(
+        "bert_base_en_uncased",
+    )
+    tokenizer("The quick brown fox jumped.")
+
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.BertTokenizer(vocabulary=vocab)
+    tokenizer("The quick brown fox jumped.")
+    ```
     """
 
     def __init__(
         self,
         vocabulary,
         lowercase=False,
         **kwargs,
@@ -91,22 +85,24 @@
             **kwargs,
         )
 
         # Check for necessary special tokens.
         cls_token = "[CLS]"
         sep_token = "[SEP]"
         pad_token = "[PAD]"
+        mask_token = "[MASK]"
         for token in [cls_token, pad_token, sep_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
         self.cls_token_id = self.token_to_id(cls_token)
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
+        self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy({**backbone_presets, **classifier_presets})
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/bert/bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,70 +7,84 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for BERT tokenizer."""
+"""Tests for DistilBERT tokenizer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
+from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
+    DistilBertTokenizer,
+)
 
 
-class BertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
+class DistilBertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
-        self.tokenizer = BertTokenizer(vocabulary=self.vocab)
+        self.tokenizer = DistilBertTokenizer(vocabulary=self.vocab)
 
     def test_tokenize(self):
         input_data = "THE QUICK BROWN FOX."
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [5, 6, 7, 8, 1])
 
     def test_tokenize_batch(self):
         input_data = tf.constant(["THE QUICK BROWN FOX.", "THE FOX."])
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [[5, 6, 7, 8, 1], [5, 8, 1]])
 
     def test_lowercase(self):
         input_data = "THE QUICK BROWN FOX."
-        tokenizer = BertTokenizer(vocabulary=self.vocab, lowercase=True)
+        tokenizer = DistilBertTokenizer(vocabulary=self.vocab, lowercase=True)
         output = tokenizer(input_data)
         self.assertAllEqual(output, [9, 10, 11, 12, 1])
 
     def test_detokenize(self):
         input_tokens = [[5, 6, 7, 8]]
         output = self.tokenizer.detokenize(input_tokens)
         self.assertAllEqual(output, ["THE QUICK BROWN FOX"])
 
     def test_vocabulary_size(self):
         self.assertEqual(self.tokenizer.vocabulary_size(), 13)
 
     def test_errors_missing_special_tokens(self):
         with self.assertRaises(ValueError):
-            BertTokenizer(vocabulary=["a", "b", "c"])
+            DistilBertTokenizer(vocabulary=["a", "b", "c"])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["THE QUICK BROWN FOX."])
-        tokenizer = BertTokenizer(vocabulary=self.vocab)
+        tokenizer = DistilBertTokenizer(vocabulary=self.vocab)
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 """DeBERTa backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.models.deberta_v3.disentangled_attention_encoder import (
     DisentangledAttentionEncoder,
 )
 from keras_nlp.models.deberta_v3.relative_embedding import RelativeEmbedding
 from keras_nlp.utils.python_utils import classproperty
 
 
 def deberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.DebertaV3Backbone")
 class DebertaV3Backbone(Backbone):
     """DeBERTa encoder network.
 
     This network implements a bi-directional Transformer-based encoder as
     described in
     ["DeBERTaV3: Improving DeBERTa using ELECTRA-Style Pre-Training with Gradient-Disentangled Embedding Sharing"](https://arxiv.org/abs/2111.09543).
     It includes the embedding lookups and transformer layers, but does not
@@ -74,32 +75,32 @@
     ```python
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
     }
 
-    # Pretrained DeBERTa encoder
+    # Pretrained DeBERTa encoder.
     model = keras_nlp.models.DebertaV3Backbone.from_preset(
-        "deberta_base_en",
+        "deberta_v3_base_en",
     )
-    output = model(input_data)
+    model(input_data)
 
     # Randomly initialized DeBERTa encoder with custom config
     model = keras_nlp.models.DebertaV3Backbone(
         vocabulary_size=128100,
         num_layers=12,
         num_heads=6,
         hidden_dim=384,
         intermediate_dim=1536,
         max_sequence_length=512,
         bucket_size=256,
     )
     # Call the model on the input data.
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_tokenizer_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,91 +7,109 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for DeBERTa backbone models."""
 
+"""Tests for ALBERT tokenizer."""
+
+import io
 import os
 
+import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
 
 
-class DebertaV3BackboneTest(tf.test.TestCase, parameterized.TestCase):
+class AlbertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = DebertaV3Backbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-            bucket_size=64,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=12,
+            model_type="WORD",
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
         )
-        self.batch_size = 8
-        self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-        }
-
-        self.input_dataset = tf.data.Dataset.from_tensor_slices(
-            self.input_batch
-        ).batch(2)
-
-    def test_valid_call_deberta(self):
-        self.model(self.input_batch)
-
-        # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "deberta_v3_backbone")
-
-    def test_variable_sequence_length_call_deberta(self):
-        for seq_length in (25, 50, 75):
-            input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-            }
-            self.model(input_data)
+        self.proto = bytes_io.getvalue()
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+        self.tokenizer = AlbertTokenizer(proto=self.proto)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+    def test_tokenize(self):
+        input_data = "the quick brown fox"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [5, 10, 6, 8])
+
+    def test_tokenize_batch(self):
+        input_data = tf.constant(["the quick brown fox", "the earth is round"])
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [[5, 10, 6, 8], [5, 7, 9, 11]])
+
+    def test_detokenize(self):
+        input_data = tf.constant([[5, 10, 6, 8]])
+        output = self.tokenizer.detokenize(input_data)
+        self.assertEqual(output, tf.constant(["the quick brown fox"]))
+
+    def test_vocabulary_size(self):
+        tokenizer = AlbertTokenizer(proto=self.proto)
+        self.assertEqual(tokenizer.vocabulary_size(), 12)
+
+    def test_errors_missing_special_tokens(self):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=iter(["abc"]),
+            model_writer=bytes_io,
+            vocab_size=5,
+            pad_id=-1,
+            eos_id=-1,
+            bos_id=-1,
+        )
+        with self.assertRaises(ValueError):
+            AlbertTokenizer(proto=bytes_io.getvalue())
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, DebertaV3Backbone)
-
-        # Check that output matches.
-        restored_output = restored_model(self.input_batch)
-        self.assertAllClose(model_output, restored_output)
+        input_data = tf.constant(["the quick brown fox"])
+
+        inputs = keras.Input(dtype="string", shape=())
+        outputs = self.tokenizer(inputs)
+        model = keras.Model(inputs, outputs)
+
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
+        restored_model = keras.models.load_model(path)
+        self.assertAllEqual(
+            model(input_data),
+            restored_model(input_data),
+        )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 # limitations under the License.
 """DeBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.models.deberta_v3.deberta_v3_backbone import (
     deberta_kernel_initializer,
 )
 from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
 from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.DebertaV3Classifier")
 class DebertaV3Classifier(Task):
     """An end-to-end DeBERTa model for classification tasks.
 
     This model attaches a classification head to a
     `keras_nlp.model.DebertaV3Backbone` model, mapping from the backbone
     outputs to logit output suitable for a classification task. For usage of
     this model with pre-trained weights, see the `from_preset()` method.
@@ -51,175 +52,174 @@
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/microsoft/DeBERTa).
 
     Args:
         backbone: A `keras_nlp.models.DebertaV3` instance.
         num_classes: int. Number of classes to predict.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. Dropout probability applied to the pooled output. For
-            the second dropout layer, `backbone.dropout` is used.
         preprocessor: A `keras_nlp.models.DebertaV3Preprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. Dropout probability applied to the pooled output. For
+            the second dropout layer, `backbone.dropout` is used.
 
     Examples:
 
-    Example usage.
-    ```python
-    # Define the preprocessed inputs.
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(1, 12)),
-    }
-    labels = [0, 3]
-
-    # Randomly initialized DeBERTa encoder
-    backbone = keras_nlp.models.DebertaV3Backbone(
-        vocabulary_size=128100,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
-        bucket_size=6,
-    )
-
-    # Create a DeBERTa classifier and fit your data.
-    classifier = keras_nlp.models.DebertaV3Classifier(
-        backbone,
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-    ```
-
-    Raw string inputs.
+    Raw string data.
     ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
-    # Create a DebertaV3Classifier and fit your data.
+    # Pretrained classifier.
     classifier = keras_nlp.models.DebertaV3Classifier.from_preset(
         "deberta_v3_base_en",
         num_classes=4,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
     classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Raw string inputs with customized preprocessing.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
+    classifier.predict(x=features, batch_size=2)
 
-    # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.DebertaV3Preprocessor.from_preset(
-        "deberta_v3_base_en",
-        sequence_length=128,
-    )
-
-    # Create a DebertaV3Classifier and fit your data.
-    classifier = keras_nlp.models.DebertaV3Classifier.from_preset(
-        "deberta_v3_base_en",
-        num_classes=4,
-        preprocessor=preprocessor,
-    )
+    # Re-compile (e.g., with a new learning rate).
     classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
     }
     labels = [0, 3]
 
-    # Create a DebertaV3Classifier and fit your data.
+    # Pretrained classifier without preprocessing.
     classifier = keras_nlp.models.DebertaV3Classifier.from_preset(
         "deberta_v3_base_en",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(features)
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=10,
+        model_type="WORD",
+        pad_id=0,
+        bos_id=1,
+        eos_id=2,
+        unk_id=3,
+        pad_piece="[PAD]",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        unk_piece="[UNK]",
+    )
+    tokenizer = keras_nlp.models.DebertaV3Tokenizer(
+        proto=bytes_io.getvalue(),
+    )
+    preprocessor = keras_nlp.models.DebertaV3Preprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
+    )
+    backbone = keras_nlp.models.DebertaV3Backbone(
+        vocabulary_size=30552,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    classifier = keras_nlp.models.DebertaV3Classifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
+        num_classes,
+        preprocessor=None,
+        activation=None,
         hidden_dim=None,
         dropout=0.0,
-        preprocessor=None,
         **kwargs,
     ):
         inputs = backbone.input
-        if hidden_dim is None:
-            hidden_dim = backbone.hidden_dim
+        hidden_dim = hidden_dim or backbone.hidden_dim
 
         x = backbone(inputs)[:, backbone.start_token_index, :]
         x = keras.layers.Dropout(dropout, name="pooled_dropout")(x)
         x = keras.layers.Dense(
             hidden_dim,
             activation=lambda x: keras.activations.gelu(x, approximate=False),
             name="pooled_dense",
         )(x)
         x = keras.layers.Dropout(backbone.dropout, name="classifier_dropout")(x)
         outputs = keras.layers.Dense(
             num_classes,
             kernel_initializer=deberta_kernel_initializer(),
+            activation=activation,
             name="logits",
         )(x)
 
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
         # Default compilation
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(5e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
     @classproperty
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,141 +7,131 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for DeBERTa classification model."""
+"""Tests for RoBERTa classification model."""
 
-import io
 import os
 
-import sentencepiece
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
-from keras_nlp.models.deberta_v3.deberta_v3_classifier import (
-    DebertaV3Classifier,
-)
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
-    DebertaV3Preprocessor,
-)
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.models.roberta.roberta_classifier import RobertaClassifier
+from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
-class DebertaV3ClassifierTest(tf.test.TestCase, parameterized.TestCase):
+class RobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        bytes_io = io.BytesIO()
-        vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
-        )
-        sentencepiece.SentencePieceTrainer.train(
-            sentence_iterator=vocab_data.as_numpy_iterator(),
-            model_writer=bytes_io,
-            vocab_size=10,
-            model_type="WORD",
-            pad_id=0,
-            bos_id=1,
-            eos_id=2,
-            unk_id=3,
-            pad_piece="[PAD]",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            unk_piece="[UNK]",
-        )
-        self.preprocessor = DebertaV3Preprocessor(
-            tokenizer=DebertaV3Tokenizer(proto=bytes_io.getvalue()),
-            sequence_length=12,
+        self.vocab = {
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
+            "Ġkoh": 7,
+            "li": 8,
+            "Ġis": 9,
+            "Ġthe": 10,
+            "Ġbest": 11,
+            "<mask>": 12,
+        }
+
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+        self.merges = merges
+        self.preprocessor = RobertaPreprocessor(
+            RobertaTokenizer(vocabulary=self.vocab, merges=self.merges),
+            sequence_length=5,
         )
-        self.backbone = DebertaV3Backbone(
-            vocabulary_size=1000,
+        self.backbone = RobertaBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-            bucket_size=64,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.classifier = DebertaV3Classifier(
+        self.classifier = RobertaClassifier(
             self.backbone,
-            4,
+            num_classes=4,
             preprocessor=self.preprocessor,
-        )
-        self.classifier_no_preprocessing = DebertaV3Classifier(
-            self.backbone,
-            4,
-            preprocessor=None,
+            # Check we handle serialization correctly.
+            activation=keras.activations.softmax,
+            hidden_dim=4,
         )
 
+        # Setup data.
         self.raw_batch = tf.constant(
             [
-                "the quick brown fox.",
-                "the slow brown fox.",
-                "the earth is round",
-                "the earth is spherical",
+                " airplane at airport",
+                " the airplane is the best",
             ]
         )
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            (self.raw_batch, tf.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
+    def test_classifier_predict(self):
+        preds1 = self.classifier.predict(self.raw_batch)
+        self.classifier.preprocessor = None
+        preds2 = self.classifier.predict(self.preprocessed_batch)
+        # Assert predictions match.
+        self.assertAllClose(preds1, preds2)
+        # Assert valid softmax output.
+        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
 
-    def test_debertav3_classifier_fit_default_compile(self):
+    def test_classifier_fit(self):
         self.classifier.fit(self.raw_dataset)
+        self.classifier.preprocessor = None
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit(self, jit_compile):
+    def test_classifier_fit_no_xla(self):
+        self.classifier.preprocessor = None
         self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
         )
-        self.classifier.fit(self.raw_dataset)
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.classifier)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.classifier.get_config(),
         )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
-    def test_saving_model(self, save_format, filename):
+    @pytest.mark.large  # Saving is slow, so mark these large.
+    def test_saved_model(self, save_format, filename):
         model_output = self.classifier.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.classifier.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, DebertaV3Classifier)
+        self.assertIsInstance(restored_model, RobertaClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""DeBERTa preprocessor layer."""
+"""ALBERT preprocessor layer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
+from keras_nlp.models.albert.albert_presets import backbone_presets
+from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class DebertaV3Preprocessor(Preprocessor):
-    """A DeBERTa preprocessing layer which tokenizes and packs inputs.
+@keras_nlp_export("keras_nlp.models.AlbertPreprocessor")
+class AlbertPreprocessor(Preprocessor):
+    """An ALBERT preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
      - Tokenize any number of input segments using the `tokenizer`.
      - Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
-       with the appropriate `"[CLS]"`, `"[SEP]"` and `"[PAD]"` tokens.
-     - Construct a dictionary with keys `"token_ids"` and `"padding_mask"`, that
-       can be passed directly to a DeBERTa model.
+       with the appropriate `"[CLS]"`, `"[SEP]"` and `"<pad>"` tokens.
+     - Construct a dictionary with keys `"token_ids"`, `"segment_ids"` and
+       `"padding_mask"`, that can be passed directly to
+       `keras_nlp.models.AlbertBackbone`.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
     The call method of this layer accepts three arguments, `x`, `y`, and
     `sample_weight`. `x` can be a python string or tensor representing a single
@@ -54,98 +54,101 @@
     Special care should be taken when using `tf.data` to map over an unlabeled
     tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
     directly into the call arguments of this layer, rather than forward all
     argument to `x`. To handle this case, it is recommended to  explicitly call
     the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
 
     Args:
-        tokenizer: A `keras_nlp.models.DebertaV3Tokenizer` instance.
+        tokenizer: A `keras_nlp.models.AlbertTokenizer` instance.
         sequence_length: The length of the packed inputs.
         truncate: string. The algorithm to truncate a list of batched segments
             to fit within `sequence_length`. The value can be either
             `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
     Examples:
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.DebertaV3Preprocessor.from_preset("deberta_v3_base_en")
+    preprocessor = keras_nlp.models.AlbertPreprocessor.from_preset(
+        "albert_base_en_uncased"
+    )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
     preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
+
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+
+    # Custom vocabulary.
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(["The quick brown fox jumped."])
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=10,
+        model_type="WORD",
+        pad_id=0,
+        unk_id=1,
+        bos_id=2,
+        eos_id=3,
+        pad_piece="<pad>",
+        unk_piece="<unk>",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        user_defined_symbols="[MASK]",
     )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    tokenizer = keras_nlp.models.AlbertTokenizer(
+        proto=bytes_io.getvalue(),
     )
+    preprocessor = keras_nlp.models.AlbertPreprocessor(tokenizer)
+    preprocessor("The quick brown fox jumped.")
+    ```
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.AlbertPreprocessor.from_preset(
+        "albert_base_en_uncased"
     )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
-
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is the exactly same as above.
-    tokenizer = keras_nlp.models.DebertaV3Tokenizer(proto="model.spm")
-    preprocessor = keras_nlp.models.DebertaV3Preprocessor(
-        tokenizer=tokenizer,
-        sequence_length=10,
-    )
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
@@ -171,21 +174,22 @@
             }
         )
         return config
 
     def call(self, x, y=None, sample_weight=None):
         x = convert_inputs_to_list_of_tensor_segments(x)
         x = [self.tokenizer(segment) for segment in x]
-        token_ids, _ = self.packer(x)
+        token_ids, segment_ids = self.packer(x)
         x = {
             "token_ids": token_ids,
+            "segment_ids": segment_ids,
             "padding_mask": token_ids != self.tokenizer.pad_token_id,
         }
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     @classproperty
     def tokenizer_cls(cls):
-        return DebertaV3Tokenizer
+        return AlbertTokenizer
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,85 +8,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for DeBERTa preprocessor layer."""
+"""Tests for XLM-RoBERTa preprocessor layer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
-    DebertaV3Preprocessor,
+from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
+    XLMRobertaPreprocessor,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
 )
-from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
-class DebertaV3PreprocessorTest(tf.test.TestCase, parameterized.TestCase):
+class XLMRobertaPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
             vocab_size=10,
             model_type="WORD",
-            pad_id=0,
+            unk_id=0,
             bos_id=1,
             eos_id=2,
-            unk_id=3,
-            pad_piece="[PAD]",
-            bos_piece="[CLS]",
-            eos_piece="[SEP]",
-            unk_piece="[UNK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.preprocessor = DebertaV3Preprocessor(
-            tokenizer=DebertaV3Tokenizer(proto=self.proto),
+        self.preprocessor = XLMRobertaPreprocessor(
+            tokenizer=XLMRobertaTokenizer(proto=self.proto),
             sequence_length=12,
         )
 
     def test_tokenize_strings(self):
         input_data = "the quick brown fox"
         output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [1, 4, 9, 5, 7, 2, 0, 0, 0, 0, 0, 0]
+            output["token_ids"], [0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]
         )
         self.assertAllEqual(
             output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         )
 
     def test_tokenize_list_of_strings(self):
         # We should handle a list of strings as as batch.
         input_data = ["the quick brown fox"] * 4
         output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [[1, 4, 9, 5, 7, 2, 0, 0, 0, 0, 0, 0]] * 4
+            output["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
             output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
 
     def test_tokenize_labeled_batch(self):
         x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         x_out, y_out, sw_out = self.preprocessor(x, y, sw)
         self.assertAllEqual(
-            x_out["token_ids"], [[1, 4, 9, 5, 7, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
@@ -94,60 +92,71 @@
         x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
         x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x_out["token_ids"], [[1, 4, 9, 5, 7, 2, 0, 0, 0, 0, 0, 0]] * 4
+            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
         )
         self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_multiple_sentences(self):
         sentence_one = tf.constant("the quick brown fox")
         sentence_two = tf.constant("the earth")
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"], [1, 4, 9, 5, 7, 2, 4, 6, 2, 0, 0, 0]
+            output["token_ids"], [0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]
         )
 
     def test_tokenize_multiple_batched_sentences(self):
         sentence_one = tf.constant(["the quick brown fox"] * 4)
         sentence_two = tf.constant(["the earth"] * 4)
         # The first tuple or list is always interpreted as an enumeration of
         # separate sequences to concatenate.
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"], [[1, 4, 9, 5, 7, 2, 4, 6, 2, 0, 0, 0]] * 4
+            output["token_ids"], [[0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]] * 4
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,137 +11,142 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DeBERTa model preset configurations."""
 
 backbone_presets = {
     "deberta_v3_extra_small_en": {
+        "metadata": {
+            "description": (
+                "12-layer DeBERTaV3 model where case is maintained. "
+                "Trained on English Wikipedia, BookCorpus and OpenWebText."
+            ),
+            "params": 70682112,
+            "official_name": "DeBERTaV3",
+            "path": "deberta_v3",
+            "model_card": "https://huggingface.co/microsoft/deberta-v3-xsmall",
+        },
         "config": {
             "vocabulary_size": 128100,
             "num_layers": 12,
             "num_heads": 6,
             "hidden_dim": 384,
             "intermediate_dim": 1536,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "bucket_size": 256,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "12-layer DeBERTaV3 model where case is maintained. "
-                "Trained on English Wikipedia, BookCorpus and OpenWebText."
-            ),
-            "params": 70682112,
-            "official_name": "DeBERTaV3",
-            "path": "deberta",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_extra_small_en/v1/model.h5",
         "weights_hash": "d8e10327107e5c5e20b45548a5028619",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_extra_small_en/v1/vocab.spm",
         "spm_proto_hash": "1613fcbf3b82999c187b09c9db79b568",
     },
     "deberta_v3_small_en": {
+        "metadata": {
+            "description": (
+                "6-layer DeBERTaV3 model where case is maintained. "
+                "Trained on English Wikipedia, BookCorpus and OpenWebText."
+            ),
+            "params": 141304320,
+            "official_name": "DeBERTaV3",
+            "path": "deberta_v3",
+            "model_card": "https://huggingface.co/microsoft/deberta-v3-small",
+        },
         "config": {
             "vocabulary_size": 128100,
             "num_layers": 6,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "bucket_size": 256,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "6-layer DeBERTaV3 model where case is maintained. "
-                "Trained on English Wikipedia, BookCorpus and OpenWebText."
-            ),
-            "params": 141304320,
-            "official_name": "DeBERTaV3",
-            "path": "deberta",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_small_en/v1/model.h5",
         "weights_hash": "84118eb7c5a735f2061ecccaf71bb888",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_small_en/v1/vocab.spm",
         "spm_proto_hash": "1613fcbf3b82999c187b09c9db79b568",
     },
     "deberta_v3_base_en": {
+        "metadata": {
+            "description": (
+                "12-layer DeBERTaV3 model where case is maintained. "
+                "Trained on English Wikipedia, BookCorpus and OpenWebText."
+            ),
+            "params": 183831552,
+            "official_name": "DeBERTaV3",
+            "path": "deberta_v3",
+            "model_card": "https://huggingface.co/microsoft/deberta-v3-base",
+        },
         "config": {
             "vocabulary_size": 128100,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "bucket_size": 256,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "12-layer DeBERTaV3 model where case is maintained. "
-                "Trained on English Wikipedia, BookCorpus and OpenWebText."
-            ),
-            "params": 183831552,
-            "official_name": "DeBERTaV3",
-            "path": "deberta",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_en/v1/model.h5",
         "weights_hash": "cebce044aeed36aec9b94e3b8a255430",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_en/v1/vocab.spm",
         "spm_proto_hash": "1613fcbf3b82999c187b09c9db79b568",
     },
     "deberta_v3_large_en": {
+        "metadata": {
+            "description": (
+                "24-layer DeBERTaV3 model where case is maintained. "
+                "Trained on English Wikipedia, BookCorpus and OpenWebText."
+            ),
+            "params": 434012160,
+            "official_name": "DeBERTaV3",
+            "path": "deberta_v3",
+            "model_card": "https://huggingface.co/microsoft/deberta-v3-large",
+        },
         "config": {
             "vocabulary_size": 128100,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "bucket_size": 256,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "24-layer DeBERTaV3 model where case is maintained. "
-                "Trained on English Wikipedia, BookCorpus and OpenWebText."
-            ),
-            "params": 434012160,
-            "official_name": "DeBERTaV3",
-            "path": "deberta",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_large_en/v1/model.h5",
         "weights_hash": "bce7690f358a9e39304f8c0ebc71a745",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_large_en/v1/vocab.spm",
         "spm_proto_hash": "1613fcbf3b82999c187b09c9db79b568",
     },
     "deberta_v3_base_multi": {
+        "metadata": {
+            "description": (
+                "12-layer DeBERTaV3 model where case is maintained. "
+                "Trained on the 2.5TB multilingual CC100 dataset."
+            ),
+            "params": 278218752,
+            "official_name": "DeBERTaV3",
+            "path": "deberta_v3",
+            "model_card": "https://huggingface.co/microsoft/mdeberta-v3-base",
+        },
         "config": {
             "vocabulary_size": 251000,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "bucket_size": 256,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "12-layer DeBERTaV3 model where case is maintained. "
-                "Trained on the 2.5TB multilingual CC100 dataset."
-            ),
-            "params": 278218752,
-            "official_name": "DeBERTaV3",
-            "path": "deberta",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_multi/v1/model.h5",
         "weights_hash": "26e5a824b26afd2ee336835bd337bbeb",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/deberta_v3_base_multi/v1/vocab.spm",
         "spm_proto_hash": "b4ca07289eac48600b29529119d565e2",
     },
 }
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_presets_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,22 @@
             "deberta_v3_extra_small_en",
             sequence_length=4,
         )
         outputs = preprocessor("The quick brown fox.")["token_ids"]
         expected_outputs = [1, 279, 1538, 2]
         self.assertAllEqual(outputs, expected_outputs)
 
+    def test_preprocessor_mask_token(self):
+        preprocessor = DebertaV3Preprocessor.from_preset(
+            "deberta_v3_extra_small_en",
+            sequence_length=4,
+        )
+        self.assertEqual(preprocessor.tokenizer.id_to_token(128000), "[MASK]")
+        self.assertEqual(preprocessor.tokenizer.token_to_id("[MASK]"), 128000)
+
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_backbone_output(self, load_weights):
         input_data = {
             "token_ids": tf.constant([[0, 581, 63773, 2]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
@@ -72,29 +80,32 @@
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = DebertaV3Classifier.from_preset(
-            "deberta_v3_extra_small_en", load_weights=load_weights
+            "deberta_v3_extra_small_en",
+            num_classes=2,
+            load_weights=load_weights,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output_without_preprocessing(self, load_weights):
         input_data = {
             "token_ids": tf.constant([[0, 581, 63773, 2]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = DebertaV3Classifier.from_preset(
             "deberta_v3_extra_small_en",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
@@ -105,23 +116,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("deberta_tokenizer", DebertaV3Tokenizer),
-        ("deberta_preprocessor", DebertaV3Preprocessor),
-        ("deberta", DebertaV3Backbone),
-        ("deberta_classifier", DebertaV3Classifier),
+        ("deberta_tokenizer", DebertaV3Tokenizer, {}),
+        ("deberta_preprocessor", DebertaV3Preprocessor, {}),
+        ("deberta", DebertaV3Backbone, {}),
+        ("deberta_classifier", DebertaV3Classifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("deberta_v3_extra_small_en_clowntown")
+            cls.from_preset("deberta_v3_extra_small_en_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
 class DebertaV3PresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_tokenizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""DeBERTa tokenizer."""
+"""FNet tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
-from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class DebertaV3Tokenizer(SentencePieceTokenizer):
-    """DeBERTa tokenizer layer based on SentencePiece.
+@keras_nlp_export("keras_nlp.models.FNetTokenizer")
+class FNetTokenizer(SentencePieceTokenizer):
+    """FNet tokenizer layer based on SentencePiece.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
     underlying tokenizer, it will check for all special tokens needed by
-    DeBERTa models and provides a `from_preset()` method to automatically
-    download a matching vocabulary for a DeBERTa preset.
+    FNet models and provides a `from_preset()` method to automatically
+    download a matching vocabulary for a FNet preset.
 
     This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.DebertaV3Preprocessor` layer for input
+    combined with a `keras_nlp.models.FNetPreprocessor` layer for input
     packing.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
@@ -46,44 +45,46 @@
     Args:
         proto: Either a `string` path to a SentencePiece proto file, or a
             `bytes` object with a serialized SentencePiece proto. See the
             [SentencePiece repository](https://github.com/google/sentencepiece)
             for more details on the format.
 
     Examples:
-
     ```python
-    tokenizer = keras_nlp.models.DebertaV3Tokenizer(proto="model.spm")
-
-    # Batched inputs.
-    tokenizer(["the quick brown fox", "the earth is round"])
+    # Unbatched input.
+    tokenizer = keras_nlp.models.FNetTokenizer.from_preset(
+        "f_net_base_en",
+    )
+    tokenizer("The quick brown fox jumped.")
 
-    # Unbatched inputs.
-    tokenizer("the quick brown fox")
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
-    tokenizer.detokenize(tf.constant([[1, 4, 9, 5, 7, 2]]))
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
     ```
     """
 
     def __init__(self, proto, **kwargs):
         super().__init__(proto=proto, **kwargs)
 
         # Check for necessary special tokens.
         cls_token = "[CLS]"
         sep_token = "[SEP]"
-        pad_token = "[PAD]"
-        for token in [cls_token, pad_token, sep_token]:
+        pad_token = "<pad>"
+        mask_token = "[MASK]"
+        for token in [cls_token, sep_token, pad_token, mask_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
         self.cls_token_id = self.token_to_id(cls_token)
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
+        self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Tests for DeBERTa tokenizer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
@@ -60,42 +61,67 @@
         self.assertAllEqual(output, [[4, 9, 5, 7], [4, 6, 8, 3]])
 
     def test_detokenize(self):
         input_data = tf.constant([[4, 9, 5, 7]])
         output = self.tokenizer.detokenize(input_data)
         self.assertEqual(output, tf.constant(["the quick brown fox"]))
 
+    def test_detokenize_mask_token(self):
+        input_data = tf.constant([[4, 9, 5, 7, self.tokenizer.mask_token_id]])
+        output = self.tokenizer.detokenize(input_data)
+        self.assertEqual(output, tf.constant(["the quick brown fox"]))
+
     def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 10)
+        self.assertEqual(self.tokenizer.vocabulary_size(), 11)
+
+    def test_get_vocabulary_mask_token(self):
+        self.assertEqual(self.tokenizer.get_vocabulary()[10], "[MASK]")
+
+    def test_id_to_token_mask_token(self):
+        self.assertEqual(self.tokenizer.id_to_token(10), "[MASK]")
+
+    def test_token_to_id_mask_token(self):
+        self.assertEqual(self.tokenizer.token_to_id("[MASK]"), 10)
 
     def test_errors_missing_special_tokens(self):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=iter(["abc"]),
             model_writer=bytes_io,
             vocab_size=5,
             pad_id=-1,
             eos_id=-1,
             bos_id=-1,
         )
         with self.assertRaises(ValueError):
             DebertaV3Tokenizer(proto=bytes_io.getvalue())
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_attention_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,31 +54,14 @@
             normalization components.
         kernel_initializer: string or `keras.initializers` initializer,
             defaults to "glorot_uniform". The kernel initializer for
             the dense and disentangled self-attention layers.
         bias_initializer: string or `keras.initializers` initializer,
             defaults to "zeros". The bias initializer for
             the dense and disentangled self-attention layers.
-
-    Examples:
-
-    ```python
-    # Create a single disentangled attention encoder layer.
-    encoder = keras_nlp.layers.DisentangledAttentionEncoder(
-        intermediate_dim=64, num_heads=8)
-
-    # Create a simple model containing the encoder.
-    input = keras.Input(shape=[10, 64])
-    output = encoder(input)
-    model = keras.Model(inputs=input, outputs=output)
-
-    # Call encoder on the inputs.
-    input_data = tf.random.uniform(shape=[2, 10, 64])
-    output = model(input_data)
-    ```
     """
 
     def __init__(
         self,
         intermediate_dim,
         num_heads,
         max_position_embeddings=512,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/disentangled_self_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/deberta_v3/relative_embedding.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/relative_embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,41 +15,42 @@
 """DistilBERT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 from keras_nlp.layers.transformer_encoder import TransformerEncoder
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
 def distilbert_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.DistilBertBackbone")
 class DistilBertBackbone(Backbone):
-    """DistilBERT encoder network.
+    """A DistilBERT encoder network.
 
     This network implements a bi-directional Transformer-based encoder as
     described in ["DistilBERT, a distilled version of BERT: smaller, faster,
     cheaper and lighter"](https://arxiv.org/abs/1910.01108). It includes the
     embedding lookups and transformer layers, but not the masked language model
     or classification task networks.
 
     The default constructor gives a fully customizable, randomly initialized
     DistilBERT encoder with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset`
-    constructor.
+    dimensions. To load preset architectures and weights, use the
+    `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/huggingface/transformers).
 
     Args:
@@ -71,30 +72,30 @@
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
     }
 
-    # Pretrained DistilBERT encoder
+    # Pretrained DistilBERT encoder.
     model = keras_nlp.models.DistilBertBackbone.from_preset(
         "distil_bert_base_en_uncased"
     )
-    output = model(input_data)
+    model(input_data)
 
-    # Randomly initialized DistilBERT encoder with custom config
+    # Randomly initialized DistilBERT encoder with custom config.
     model = keras_nlp.models.DistilBertBackbone(
         vocabulary_size=30552,
-        num_layers=6,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_backbone_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,90 +21,86 @@
 from tensorflow import keras
 
 from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 
 
 class DistilBertTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = DistilBertBackbone(
-            vocabulary_size=1000,
+        self.backbone = DistilBertBackbone(
+            vocabulary_size=10,
             num_layers=2,
             num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=5,
             name="encoder",
         )
-        self.batch_size = 8
+
         self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_distilbert(self):
-        self.model(self.input_batch)
+        self.backbone(self.input_batch)
+
+    def test_token_embedding(self):
+        output = self.backbone.token_embedding(self.input_batch["token_ids"])
+        self.assertEqual(output.shape, (2, 5, 2))
 
     def test_variable_sequence_length_call_distilbert(self):
-        for seq_length in (25, 50, 75):
+        for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "mask_positions": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
             }
-            self.model(input_data)
+            self.backbone(input_data)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_distilbert_base_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+    def test_predict(self):
+        self.backbone.predict(self.input_batch)
+        self.backbone.predict(self.input_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_distilbert_base_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+    def test_serialization(self):
+        new_backbone = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.backbone)
+        )
+        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.backbone(self.input_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.backbone.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DistilBertBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
 
 
 @pytest.mark.tpu
 @pytest.mark.usefixtures("tpu_test_class")
 class DistilBertTPUTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         with self.tpu_strategy.scope():
-            self.model = DistilBertBackbone(
+            self.backbone = DistilBertBackbone(
                 vocabulary_size=1000,
                 num_layers=2,
                 num_heads=2,
                 hidden_dim=64,
                 intermediate_dim=128,
                 max_sequence_length=128,
             )
@@ -113,9 +109,9 @@
             "padding_mask": tf.ones((8, 128), dtype="int32"),
         }
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_predict(self):
-        self.model.compile()
-        self.model.predict(self.input_dataset)
+        self.backbone.compile()
+        self.backbone.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_masked_lm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,157 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""DistilBERT classification model."""
+"""DistilBERT masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.masked_lm_head import MaskedLMHead
 from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.models.distil_bert.distil_bert_backbone import (
     distilbert_kernel_initializer,
 )
-from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
-    DistilBertPreprocessor,
+from keras_nlp.models.distil_bert.distil_bert_masked_lm_preprocessor import (
+    DistilBertMaskedLMPreprocessor,
 )
 from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class DistilBertClassifier(Task):
-    """An end-to-end DistilBERT model for classification tasks.
-
-    This model attaches a classification head to a
-    `keras_nlp.model.DistilBertBackbone` model, mapping from the backbone
-    outputs to logit output suitable for a classification task. For usage of
-    this model with pre-trained weights, see the `from_preset()` method.
+@keras_nlp_export("keras_nlp.models.DistilBertMaskedLM")
+class DistilBertMaskedLM(Task):
+    """An end-to-end DistilBERT model for the masked language modeling task.
+
+    This model will train DistilBERT on a masked language modeling task.
+    The model will predict labels for a number of masked tokens in the
+    input data. For usage of this model with pre-trained weights, see the
+    `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
-    which case it will automatically apply preprocessing to raw inputs during
-    `fit()`, `predict()`, and `evaluate()`. This is done by default when
-    creating the model with `from_preset()`.
+    which case inputs can be raw string features during `fit()`, `predict()`,
+    and `evaluate()`. Inputs will be tokenized and dynamically masked during
+    training and evaluation. This is done by default when creating the model
+    with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/huggingface/transformers).
 
     Args:
-        backbone: A `keras_nlp.models.DistilBert` instance.
-        num_classes: int. Number of classes to predict.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. The dropout probability value, applied after the first
-            dense layer.
-        preprocessor: A `keras_nlp.models.DistilBertPreprocessor` or `None`. If
-            `None`, this model will not apply preprocessing, and inputs should
-            be preprocessed before calling the model.
+        backbone: A `keras_nlp.models.DistilBertBackbone` instance.
+        preprocessor: A `keras_nlp.models.DistilBertMaskedLMPreprocessor` or
+            `None`. If `None`, this model will not apply preprocessing, and
+            inputs should be preprocessed before calling the model.
 
-    Examples:
+    Example usage:
 
-    Example usage.
+    Raw string data.
     ```python
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)),
-    }
-    labels = [0, 3]
-
-    # Randomly initialized DistilBertBackbone
-    backbone = keras_nlp.models.DistilBertBackbone(
-        vocabulary_size=30552,
-        num_layers=6,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=512
-    )
-
-    # Create a DistilBertClassifier and fit your data.
-    classifier = keras_nlp.models.DistilBertClassifier(
-        backbone,
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-    ```
-
-    Raw string inputs.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
 
-    # Create a DistilBertClassifier and fit your data.
-    classifier = keras_nlp.models.DistilBertClassifier.from_preset(
+    # Pretrained language model.
+    masked_lm = keras_nlp.models.DistilBertMaskedLM.from_preset(
         "distil_bert_base_en_uncased",
-        num_classes=4,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=features, y=labels, batch_size=2)
-    ```
+    masked_lm.fit(x=features, batch_size=2)
 
-    Raw string inputs with customized preprocessing.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
-
-    # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.DistilBertPreprocessor.from_preset(
-        "distil_bert_base_en_uncased",
-        sequence_length=128,
-    )
-    # Create a DistilBertClassifier and fit your data.
-    classifier = keras_nlp.models.DistilBertClassifier.from_preset(
-        "distil_bert_base_en_uncased",
-        num_classes=4,
-        preprocessor=preprocessor,
-    )
-    classifier.compile(
+    # Re-compile (e.g., with a new learning rate).
+    masked_lm.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
-    classifier.fit(x=features, y=labels, batch_size=2)
+    # Access backbone programatically (e.g., to change `trainable`).
+    masked_lm.backbone.trainable = False
+    # Fit again.
+    masked_lm.fit(x=features, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "segment_ids": tf.constant(
-            [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
+    # Create preprocessed batch where 0 is the mask token.
+    features = {
+        "token_ids": tf.constant(
+            [[1, 2, 0, 4, 0, 6, 7, 8]] * 2, shape=(2, 8)
         ),
         "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
+            [[1, 1, 1, 1, 1, 1, 1, 1]] * 2, shape=(2, 8)
         ),
+        "mask_positions": tf.constant([[2, 4]] * 2, shape=(2, 2))
     }
-    labels = [0, 3]
+    # Labels are the original masked values.
+    labels = [[3, 5]] * 2
 
-    # Create a DistilBERT classifier and fit your data.
-    classifier = keras_nlp.models.DistilBertClassifier.from_preset(
+    masked_lm = keras_nlp.models.DistilBertMaskedLM.from_preset(
         "distil_bert_base_en_uncased",
-        num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
-        hidden_dim=None,
-        dropout=0.2,
         preprocessor=None,
         **kwargs,
     ):
-        inputs = backbone.input
-        if hidden_dim is None:
-            hidden_dim = backbone.hidden_dim
-
-        x = backbone(inputs)[:, backbone.cls_token_index, :]
-        x = keras.layers.Dense(
-            hidden_dim,
-            activation="relu",
+        inputs = {
+            **backbone.input,
+            "mask_positions": keras.Input(
+                shape=(None,), dtype="int32", name="mask_positions"
+            ),
+        }
+        backbone_outputs = backbone(backbone.input)
+        outputs = MaskedLMHead(
+            vocabulary_size=backbone.vocabulary_size,
+            embedding_weights=backbone.token_embedding.embeddings,
+            intermediate_activation="gelu",
             kernel_initializer=distilbert_kernel_initializer(),
-            name="pooled_dense",
-        )(x)
-        x = keras.layers.Dropout(dropout, name="classifier_dropout")(x)
-        outputs = keras.layers.Dense(
-            num_classes,
-            kernel_initializer=distilbert_kernel_initializer(),
-            name="logits",
-        )(x)
+            name="mlm_head",
+        )(backbone_outputs, inputs["mask_positions"])
 
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
-        self.num_classes = num_classes
-        self.hidden_dim = hidden_dim
-        self.dropout = dropout
 
         self.compile(
             loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
             optimizer=keras.optimizers.Adam(5e-5),
-            metrics=keras.metrics.SparseCategoricalAccuracy(),
+            weighted_metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
-    def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "num_classes": self.num_classes,
-                "hidden_dim": self.hidden_dim,
-                "dropout": self.dropout,
-            }
-        )
-        return config
-
     @classproperty
     def backbone_cls(cls):
         return DistilBertBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return DistilBertPreprocessor
+        return DistilBertMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_classifier_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for DistilBERT classification model."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.distil_bert.distil_bert_backbone import DistilBertBackbone
 from keras_nlp.models.distil_bert.distil_bert_classifier import (
     DistilBertClassifier,
@@ -29,102 +30,96 @@
 from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
     DistilBertTokenizer,
 )
 
 
 class DistilBertClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = DistilBertBackbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-        )
+        # Setup model
+
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["the", "quick", "brown", "fox", "."]
         self.preprocessor = DistilBertPreprocessor(
             DistilBertTokenizer(vocabulary=self.vocab),
             sequence_length=8,
         )
+        self.backbone = DistilBertBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
+            num_layers=2,
+            num_heads=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
+        )
         self.classifier = DistilBertClassifier(
             self.backbone,
-            4,
+            num_classes=4,
             preprocessor=self.preprocessor,
-        )
-        self.classifier_no_preprocessing = DistilBertClassifier(
-            self.backbone,
-            4,
-            preprocessor=None,
+            # Check we handle serialization correctly.
+            activation=keras.activations.softmax,
+            hidden_dim=4,
         )
 
         self.raw_batch = tf.constant(
             [
                 "the quick brown fox.",
                 "the slow brown fox.",
-                "the smelly brown fox.",
-                "the old brown fox.",
             ]
         )
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            (self.raw_batch, tf.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
+    def test_classifier_predict(self):
+        preds1 = self.classifier.predict(self.raw_batch)
+        self.classifier.preprocessor = None
+        preds2 = self.classifier.predict(self.preprocessed_batch)
+        # Assert predictions match.
+        self.assertAllClose(preds1, preds2)
+        # Assert valid softmax output.
+        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
+    def test_classifier_fit(self):
+        self.classifier.fit(self.raw_dataset)
+        self.classifier.preprocessor = None
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit(self, jit_compile):
+    def test_classifier_fit_no_xla(self):
+        self.classifier.preprocessor = None
         self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+            loss="sparse_categorical_crossentropy",
+            jit_compile=False,
         )
-        self.classifier.fit(self.raw_dataset)
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.classifier)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.classifier.get_config(),
         )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
-
-    def test_distilbert_classifier_fit_default_compile(self):
-        self.classifier.fit(self.raw_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saving_model(self, save_format, filename):
         model_output = self.classifier.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.classifier.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DistilBertClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,192 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""DistilBERT preprocessor layers."""
 
-import copy
+"""GPT2 preprocessor layer."""
 
-from tensorflow import keras
+import copy
 
-from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
-from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
-    DistilBertTokenizer,
-)
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.start_end_packer import StartEndPacker
+from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
+from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class DistilBertPreprocessor(Preprocessor):
-    """A DistilBERT preprocessing layer which tokenizes and packs inputs.
-
-    This preprocessing layer will do three things:
-
-     - Tokenize any number of input segments using the `tokenizer`.
-     - Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
-       with the appropriate `"[CLS]"`, `"[SEP]"` and `"[PAD]"` tokens.
-     - Construct a dictionary of with keys `"token_ids"` and `"padding_mask"`,
-       that can be passed directly to a DistilBERT model.
+@keras_nlp_export("keras_nlp.models.GPT2Preprocessor")
+class GPT2Preprocessor(Preprocessor):
+    """GPT2 preprocessing layer which tokenizes and packs inputs.
+
+    This preprocessing layer will do 2 things:
+
+    - Tokenize the input using the `tokenizer`.
+    - Construct a dictionary with keys `"token_ids"`, `"padding_mask"`, that can
+        be passed directly to a `keras_nlp.models.GPT2Backbone`.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
     The call method of this layer accepts three arguments, `x`, `y`, and
     `sample_weight`. `x` can be a python string or tensor representing a single
     segment, a list of python strings representing a batch of single segments,
     or a list of tensors representing multiple segments to be packed together.
     `y` and `sample_weight` are both optional, can have any format, and will be
     passed through unaltered.
 
-    Special care should be taken when using `tf.data` to map over an unlabeled
-    tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
-    directly into the call arguments of this layer, rather than forward all
-    argument to `x`. To handle this case, it is recommended to  explicitly call
-    the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
+    `GPT2Preprocessor` forces the input to have only one segment, as GPT2 is
+    mainly used for generation tasks. For tasks having multi-segment inputs
+    like "glue/mnli", please use a model designed for classification purposes
+    such as BERT or RoBERTa.
 
     Args:
-        tokenizer: A `keras_nlp.models.DistilBertTokenizer` instance.
+        tokenizer: A `keras_nlp.models.GPT2Tokenizer` instance.
         sequence_length: The length of the packed inputs.
-        truncate: string. The algorithm to truncate a list of batched segments
-            to fit within `sequence_length`. The value can be either
-            `round_robin` or `waterfall`:
-                - `"round_robin"`: Available space is assigned one token at a
-                    time in a round-robin fashion to the inputs that still need
-                    some, until the limit is reached.
-                - `"waterfall"`: The allocation of the budget is done using a
-                    "waterfall" algorithm that allocates quota in a
-                    left-to-right manner and fills up the buckets until we run
-                    out of budget. It supports an arbitrary number of segments.
+        add_start_token: If true, the preprocessor will append the tokenizer
+            start token to each input sequence.
+        add_end_token: If true, the preprocessor will append the tokenizer
+            end token to each input sequence.
+
+    Call arguments:
+        x: A string `tf.Tensor` or list of python strings.
+        y: Any label data. Will be passed through unaltered.
+        sample_weight: Any label weight data. Will be passed through unaltered.
+        sequence_length: Pass to override the configured `sequence_length` of
+            the layer.
+        add_start_token: Pass to override the configure value of
+            `add_start_token` on the layer.
+        add_end_token: Pass to override the configure value of
+            `add_end_token` on the layer.
 
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.DistilBertPreprocessor.from_preset("distil_bert_base_en_uncased")
+    preprocessor = keras_nlp.models.GPT2Preprocessor.from_preset("gpt2_base_en")
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
     preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    # Custom vocabulary.
+    features = ["a quick fox.", "a fox quick."]
+    vocab = {"<|endoftext|>": 0, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.GPT2Tokenizer(
+        vocabulary=vocab,
+        merges=merges,
     )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+    preprocessor = keras_nlp.models.GPT2Preprocessor(tokenizer=tokenizer)
+    preprocessor("The quick brown fox jumped.")
+    ```
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.GPT2Preprocessor.from_preset("gpt2_base_en")
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
-    # Watch out for tf.data's default unpacking of tuples here!
-    # Best to invoke the `preprocessor` directly in this case.
-    ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
+    text = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((text, label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as above.
-    vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]"]
-    vocab += ["The", "qu", "##ick", "br", "##own", "fox", "tripped"]
-    vocab += ["Call", "me", "Ish", "##mael", "."]
-    vocab += ["Oh", "look", "a", "whale"]
-    vocab += ["I", "forgot", "my", "home", "##work"]
-    tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
-    preprocessor = keras_nlp.models.DistilBertPreprocessor(tokenizer)
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(text)
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
     ```
     """
 
     def __init__(
         self,
         tokenizer,
-        sequence_length=512,
-        truncate="round_robin",
+        sequence_length=1024,
+        add_start_token=True,
+        add_end_token=True,
         **kwargs,
     ):
         super().__init__(**kwargs)
+
         self.tokenizer = tokenizer
-        self.packer = MultiSegmentPacker(
-            start_value=self.tokenizer.cls_token_id,
-            end_value=self.tokenizer.sep_token_id,
-            pad_value=self.tokenizer.pad_token_id,
-            truncate=truncate,
+        self.sequence_length = sequence_length
+        self.add_start_token = add_start_token
+        self.add_end_token = add_end_token
+        self.packer = StartEndPacker(
+            start_value=tokenizer.start_token_id,
+            end_value=tokenizer.end_token_id,
+            pad_value=tokenizer.pad_token_id,
             sequence_length=sequence_length,
+            return_padding_mask=True,
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "sequence_length": self.packer.sequence_length,
-                "truncate": self.packer.truncate,
+                "sequence_length": self.sequence_length,
+                "add_start_token": self.add_start_token,
+                "add_end_token": self.add_end_token,
             }
         )
         return config
 
-    def call(self, x, y=None, sample_weight=None):
+    def call(
+        self,
+        x,
+        y=None,
+        sample_weight=None,
+        sequence_length=None,
+        add_start_token=None,
+        add_end_token=None,
+    ):
         x = convert_inputs_to_list_of_tensor_segments(x)
-        x = [self.tokenizer(segment) for segment in x]
-        token_ids, _ = self.packer(x)
+        if len(x) != 1:
+            raise ValueError(
+                "GPT2 requires each input feature to contain only "
+                f"one segment, but received {len(x)}. If you are using GPT2 "
+                "for a multi-segment classification task, please refer to "
+                "classification models like BERT or RoBERTa."
+            )
+        if sequence_length is None:
+            sequence_length = self.sequence_length
+        if add_start_token is None:
+            add_start_token = self.add_start_token
+        if add_end_token is None:
+            add_end_token = self.add_end_token
+        token_ids, padding_mask = self.packer(
+            self.tokenizer(x[0]),
+            sequence_length=sequence_length,
+            add_start_value=add_start_token,
+            add_end_value=add_end_token,
+        )
         x = {
             "token_ids": token_ids,
-            "padding_mask": token_ids != self.tokenizer.pad_token_id,
+            "padding_mask": padding_mask,
         }
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     @classproperty
-    def tokenizer_cls(cls):
-        return DistilBertTokenizer
-
-    @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
+    @classproperty
+    def tokenizer_cls(cls):
+        return GPT2Tokenizer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for DistilBERT preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.distil_bert.distil_bert_preprocessor import (
     DistilBertPreprocessor,
 )
@@ -97,23 +98,34 @@
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["THE QUICK BROWN FOX."])
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                 "6-layer DistilBERT model where all input is lowercased. "
                 "Trained on English Wikipedia + BooksCorpus using BERT as the "
                 "teacher model."
             ),
             "params": 66362880,
             "official_name": "DistilBERT",
             "path": "distil_bert",
+            "model_card": "https://huggingface.co/distilbert-base-uncased",
         },
         "config": {
             "vocabulary_size": 30522,
             "num_layers": 6,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -48,14 +49,15 @@
                 "6-layer DistilBERT model where case is maintained. "
                 "Trained on English Wikipedia + BooksCorpus using BERT as the "
                 "teacher model."
             ),
             "params": 65190912,
             "official_name": "DistilBERT",
             "path": "distil_bert",
+            "model_card": "https://huggingface.co/distilbert-base-cased",
         },
         "config": {
             "vocabulary_size": 28996,
             "num_layers": 6,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -74,14 +76,15 @@
         "metadata": {
             "description": (
                 "6-layer DistilBERT model where case is maintained. Trained on Wikipedias of 104 languages"
             ),
             "params": 134734080,
             "official_name": "DistilBERT",
             "path": "distil_bert",
+            "model_card": "https://huggingface.co/distilbert-base-multilingual-cased",
         },
         "config": {
             "vocabulary_size": 119547,
             "num_layers": 6,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,28 +74,30 @@
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = DistilBertClassifier.from_preset(
             "distil_bert_base_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
         )
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output_without_preprocessing(self, load_weights):
         input_data = {
             "token_ids": tf.constant([[101, 1996, 4248, 102]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = DistilBertClassifier.from_preset(
             "distil_bert_base_en_uncased",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("distilbert_tokenizer", DistilBertTokenizer),
@@ -105,23 +107,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("distilbert_tokenizer", DistilBertTokenizer),
-        ("distilbert_preprocessor", DistilBertPreprocessor),
-        ("distilbert", DistilBertBackbone),
-        ("distilbert_classifier", DistilBertClassifier),
+        ("distilbert_tokenizer", DistilBertTokenizer, {}),
+        ("distilbert_preprocessor", DistilBertPreprocessor, {}),
+        ("distilbert", DistilBertBackbone, {}),
+        ("distilbert_classifier", DistilBertClassifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("distilbert_base_uncased_clowntown")
+            cls.from_preset("distilbert_base_uncased", **kwargs)
 
 
 @pytest.mark.extra_large
 class DistilBertPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Tests the full enumeration of our preset.
 
@@ -149,28 +151,28 @@
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_load_distilbert_classifier(self, load_weights):
         for preset in DistilBertClassifier.presets:
             classifier = DistilBertClassifier.from_preset(
                 preset,
-                num_classes=4,
+                num_classes=2,
                 load_weights=load_weights,
             )
             input_data = tf.constant(["This quick brown fox"])
             classifier.predict(input_data)
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_load_distilbert_classifier_no_preprocessing(self, load_weights):
         for preset in DistilBertClassifier.presets:
             classifier = DistilBertClassifier.from_preset(
                 preset,
-                num_classes=4,
+                num_classes=2,
                 load_weights=load_weights,
                 preprocessor=None,
             )
             input_data = {
                 "token_ids": tf.random.uniform(
                     shape=(1, 512),
                     dtype=tf.int64,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """DistilBERT tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.distil_bert.distil_bert_presets import backbone_presets
 from keras_nlp.tokenizers.word_piece_tokenizer import WordPieceTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.DistilBertTokenizer")
 class DistilBertTokenizer(WordPieceTokenizer):
     """A DistilBERT tokenizer using WordPiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.WordPieceTokenizer`. Unlike the
     underlying tokenizer, it will check for all special tokens needed by DistilBERT
     models and provides a `from_preset()` method to automatically download
@@ -47,37 +46,33 @@
             piece token string. If passing a filename, the file should be a
             plain text file containing a single word piece token per line.
         lowercase: If true, the input text will be first lowered before
             tokenization.
 
     Examples:
 
-    Batched input.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = ["The quick brown fox.", "The fox."]
-    >>> tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
-    >>> tokenizer(inputs)
-    <tf.RaggedTensor [[4, 5, 6, 7, 8, 9], [4, 8, 9]]>
-
-    Unbatched input.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = "The fox."
-    >>> tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
-    >>> tokenizer(inputs)
-    <tf.Tensor: shape=(3,), dtype=int32, numpy=array([4, 8, 9], dtype=int32)>
-
-    Detokenization.
-    >>> vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]"]
-    >>> vocab += ["The", "qu", "##ick", "brown", "fox", "."]
-    >>> inputs = "The quick brown fox."
-    >>> tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
-    >>> tokenizer.detokenize(tokenizer.tokenize(inputs)).numpy().decode('utf-8')
-    'The quick brown fox .'
+    ```python
+    # Unbatched input.
+    tokenizer = keras_nlp.models.DistilBertTokenizer.from_preset(
+        "distil_bert_base_en_uncased",
+    )
+    tokenizer("The quick brown fox jumped.")
+
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    vocab = ["[UNK]", "[CLS]", "[SEP]", "[PAD]", "[MASK]"]
+    vocab += ["The", "quick", "brown", "fox", "jumped", "."]
+    tokenizer = keras_nlp.models.DistilBertTokenizer(vocabulary=vocab)
+    tokenizer("The quick brown fox jumped.")
+    ```
     """
 
     def __init__(
         self,
         vocabulary,
         lowercase=False,
         **kwargs,
@@ -88,22 +83,24 @@
             **kwargs,
         )
 
         # Check for necessary special tokens.
         cls_token = "[CLS]"
         sep_token = "[SEP]"
         pad_token = "[PAD]"
-        for token in [cls_token, pad_token, sep_token]:
+        mask_token = "[MASK]"
+        for token in [cls_token, pad_token, sep_token, mask_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
         self.cls_token_id = self.token_to_id(cls_token)
         self.sep_token_id = self.token_to_id(sep_token)
         self.pad_token_id = self.token_to_id(pad_token)
+        self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_tokenizer_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,72 +7,82 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for DistilBERT tokenizer."""
+"""Tests for BERT tokenizer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.distil_bert.distil_bert_tokenizer import (
-    DistilBertTokenizer,
-)
+from keras_nlp.models.bert.bert_tokenizer import BertTokenizer
 
 
-class DistilBertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
+class BertTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = ["[PAD]", "[UNK]", "[CLS]", "[SEP]", "[MASK]"]
         self.vocab += ["THE", "QUICK", "BROWN", "FOX"]
         self.vocab += ["the", "quick", "brown", "fox"]
-        self.tokenizer = DistilBertTokenizer(vocabulary=self.vocab)
+        self.tokenizer = BertTokenizer(vocabulary=self.vocab)
 
     def test_tokenize(self):
         input_data = "THE QUICK BROWN FOX."
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [5, 6, 7, 8, 1])
 
     def test_tokenize_batch(self):
         input_data = tf.constant(["THE QUICK BROWN FOX.", "THE FOX."])
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [[5, 6, 7, 8, 1], [5, 8, 1]])
 
     def test_lowercase(self):
         input_data = "THE QUICK BROWN FOX."
-        tokenizer = DistilBertTokenizer(vocabulary=self.vocab, lowercase=True)
+        tokenizer = BertTokenizer(vocabulary=self.vocab, lowercase=True)
         output = tokenizer(input_data)
         self.assertAllEqual(output, [9, 10, 11, 12, 1])
 
     def test_detokenize(self):
         input_tokens = [[5, 6, 7, 8]]
         output = self.tokenizer.detokenize(input_tokens)
         self.assertAllEqual(output, ["THE QUICK BROWN FOX"])
 
     def test_vocabulary_size(self):
         self.assertEqual(self.tokenizer.vocabulary_size(), 13)
 
     def test_errors_missing_special_tokens(self):
         with self.assertRaises(ValueError):
-            DistilBertTokenizer(vocabulary=["a", "b", "c"])
+            BertTokenizer(vocabulary=["a", "b", "c"])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["THE QUICK BROWN FOX."])
-        tokenizer = DistilBertTokenizer(vocabulary=self.vocab)
+        tokenizer = BertTokenizer(vocabulary=self.vocab)
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """FNet backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.f_net_encoder import FNetEncoder
 from keras_nlp.layers.position_embedding import PositionEmbedding
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
@@ -30,26 +31,26 @@
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
 def f_net_bias_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.FNetBackbone")
 class FNetBackbone(Backbone):
-    """FNet encoder network.
+    """A FNet encoder network.
 
     This class implements a bi-directional Fourier Transform-based encoder as
     described in ["FNet: Mixing Tokens with Fourier Transforms"](https://arxiv.org/abs/2105.03824).
     It includes the embedding lookups and `keras_nlp.layers.FNetEncoder` layers,
     but not the masked language model or next sentence prediction heads.
 
-    The default constructor gives a fully customizable, randomly initialized FNet
-    encoder with any number of layers and embedding dimensions. To load
-    preset architectures and weights, use the `from_preset` constructor.
+    The default constructor gives a fully customizable, randomly initialized
+    FNet encoder with any number of layers and embedding dimensions. To
+    load preset architectures and weights, use the `from_preset()` constructor.
 
     Note: unlike other models, FNet does not take in a `"padding_mask"` input,
     the `"<pad>"` token is handled equivalently to all other tokens in the input
     sequence.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind.
@@ -73,23 +74,27 @@
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "segment_ids": tf.constant(
             [0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
     }
 
-    # Randomly initialized FNet encoder with a custom config
+    # Pretrained BERT encoder.
+    model = keras_nlp.models.FNetBackbone.from_preset("f_net_base_en")
+    model(input_data)
+
+    # Randomly initialized FNet encoder with a custom config.
     model = keras_nlp.models.FNetBackbone(
         vocabulary_size=32000,
-        num_layers=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
+        num_layers=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,92 +7,112 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for FNet backbone model."""
+"""Test for GPT-2 backbone models."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
 
 
-class FNetBackboneTest(tf.test.TestCase, parameterized.TestCase):
+class GPT2Test(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = FNetBackbone(
-            vocabulary_size=1000,
+        self.backbone = GPT2Backbone(
+            vocabulary_size=10,
             num_layers=2,
-            hidden_dim=16,
-            intermediate_dim=32,
-            max_sequence_length=128,
-            num_segments=4,
+            num_heads=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=5,
         )
-        self.batch_size = 8
         self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "segment_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "segment_ids": tf.ones((2, 5), dtype="int32"),
+            "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
-
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_f_net(self):
-        self.model(self.input_batch)
+    def test_call(self):
+        self.backbone(self.input_batch)
+
+    def test_token_embedding(self):
+        output = self.backbone.token_embedding(self.input_batch["token_ids"])
+        self.assertEqual(output.shape, (2, 5, 2))
 
+    def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "f_net_backbone")
+        self.assertRegexpMatches(self.backbone.name, "gpt2_backbone")
 
-    def test_variable_sequence_length_call_f_net(self):
-        for seq_length in (25, 50, 75):
+    def test_variable_sequence_length(self):
+        for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "segment_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
             }
-            self.model(input_data)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+            self.backbone(input_data)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+    def test_predict(self):
+        self.backbone.predict(self.input_batch)
+        self.backbone.predict(self.input_dataset)
+
+    def test_serialization(self):
+        new_backbone = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.backbone)
+        )
+        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.backbone(self.input_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.backbone.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, FNetBackbone)
+        self.assertIsInstance(restored_model, GPT2Backbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
-        self.assertAllClose(
-            model_output["pooled_output"], restored_output["pooled_output"]
-        )
+        self.assertAllClose(model_output, restored_output)
+
+
+@pytest.mark.tpu
+@pytest.mark.usefixtures("tpu_test_class")
+class GPT2BackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+    def setUp(self):
+        with self.tpu_strategy.scope():
+            self.model = GPT2Backbone(
+                vocabulary_size=10,
+                num_layers=2,
+                num_heads=2,
+                hidden_dim=2,
+                intermediate_dim=4,
+                max_sequence_length=5,
+            )
+        self.input_batch = {
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "padding_mask": tf.ones((2, 5), dtype="int32"),
+        }
+        self.input_dataset = tf.data.Dataset.from_tensor_slices(
+            self.input_batch
+        ).batch(2)
+
+    def test_predict(self):
+        self.model.compile()
+        self.model.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,131 +14,149 @@
 
 """FNet classification model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.models.f_net.f_net_backbone import f_net_kernel_initializer
 from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.FNetClassifier")
 class FNetClassifier(Task):
     """An end-to-end f_net model for classification tasks.
 
     This model attaches a classification head to a
-    `keras_nlp.model.FNetBackbone` model, mapping from the backbone
-    outputs to logit output suitable for a classification task. For usage of
-    this model with pre-trained weights, see the `from_preset()` method.
+    `keras_nlp.model.FNetBackbone` instance, mapping from the backbone outputs
+    to logits suitable for a classification task. For usage of this model with
+    pre-trained weights, use the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind.
 
     Args:
         backbone: A `keras_nlp.models.FNetBackbone` instance.
         num_classes: int. Number of classes to predict.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. The dropout probability value, applied after the dense
-            layer.
         preprocessor: A `keras_nlp.models.FNetPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. The dropout probability value, applied after the dense
+            layer.
+
+    Examples:
+
+    Raw string data.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+    labels = [0, 3]
+
+    # Pretrained classifier.
+    classifier = keras_nlp.models.FNetClassifier.from_preset(
+        "f_net_base_en",
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
+    classifier.predict(x=features, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate).
+    classifier.compile(
+        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
+    )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
 
-    Example usage:
+    Preprocessed integer data.
     ```python
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
         "segment_ids": tf.constant(
             [[0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
     }
     labels = [0, 3]
 
-    # Randomly initialize a Fnet backbone
-    backbone = keras_nlp.models.FNetBackbone(
-        vocabulary_size=32000,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
-    )
-
-    # Create a Fnet classifier and fit your data.
-    classifier = keras_nlp.models.FnetClassifier(
-        backbone,
+    # Pretrained classifier without preprocessing.
+    classifier = keras_nlp.models.FNetClassifier.from_preset(
+        "f_net_base_en",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
-        dropout=0.1,
+        num_classes,
         preprocessor=None,
+        activation=None,
+        dropout=0.1,
         **kwargs,
     ):
         inputs = backbone.input
         pooled = backbone(inputs)["pooled_output"]
         pooled = keras.layers.Dropout(dropout)(pooled)
         outputs = keras.layers.Dense(
             num_classes,
             kernel_initializer=f_net_kernel_initializer(),
+            activation=activation,
             name="logits",
         )(pooled)
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
         self.dropout = dropout
 
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(5e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
                 "dropout": self.dropout,
+                "activation": keras.activations.serialize(self.activation),
             }
         )
         return config
 
     @classproperty
     def backbone_cls(cls):
         return FNetBackbone
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_classifier_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,137 +12,129 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for FNet classification model."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
 from keras_nlp.models.f_net.f_net_classifier import FNetClassifier
 from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
 class FNetClassifierTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = FNetBackbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-            name="encoder",
-        )
-
+        # Setup Model
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
 
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=12,
             model_type="WORD",
             pad_id=3,
             unk_id=0,
             bos_id=4,
             eos_id=5,
             pad_piece="<pad>",
             unk_piece="<unk>",
             bos_piece="[CLS]",
             eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
         )
 
         self.proto = bytes_io.getvalue()
 
         self.preprocessor = FNetPreprocessor(
             tokenizer=FNetTokenizer(proto=self.proto),
-            sequence_length=12,
+            sequence_length=8,
+        )
+        self.backbone = FNetBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
+            num_layers=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-
         self.classifier = FNetClassifier(
             self.backbone,
-            4,
+            num_classes=4,
             preprocessor=self.preprocessor,
-        )
-        self.classifier_no_preprocessing = FNetClassifier(
-            self.backbone,
-            4,
-            preprocessor=None,
+            # Check we handle serialization correctly.
+            activation=keras.activations.softmax,
         )
 
+        # Setup data.
         self.raw_batch = tf.constant(
             [
                 "the quick brown fox.",
                 "the slow brown fox.",
-                "the smelly brown fox.",
-                "the old brown fox.",
             ]
         )
         self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            (self.raw_batch, tf.ones((2,)))
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
         self.classifier(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_fnet_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_fnet_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
+    def test_classifier_predict(self):
+        preds1 = self.classifier.predict(self.raw_batch)
+        self.classifier.preprocessor = None
+        preds2 = self.classifier.predict(self.preprocessed_batch)
+        # Assert predictions match.
+        self.assertAllClose(preds1, preds2)
+        # Assert valid softmax output.
+        self.assertAllClose(tf.reduce_sum(preds2, axis=-1), [1.0, 1.0])
 
-    def test_fnet_classifier_fit_default_compile(self):
+    def test_fnet_classifier_fit(self):
         self.classifier.fit(self.raw_dataset)
+        self.classifier.preprocessor = None
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_fnet_classifier_fit(self, jit_compile):
+    def test_classifier_fit_no_xla(self):
+        self.classifier.preprocessor = None
         self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
         )
-        self.classifier.fit(self.raw_dataset)
+        self.classifier.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_fnet_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.classifier)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.classifier.get_config(),
         )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         model_output = self.classifier.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.classifier.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, FNetClassifier)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,134 +11,113 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """FNet preprocessor layer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.multi_segment_packer import MultiSegmentPacker
 from keras_nlp.models.f_net.f_net_presets import backbone_presets
 from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.FNetPreprocessor")
 class FNetPreprocessor(Preprocessor):
     """An FNet preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
-     - Tokenize any number of input segments using the `tokenizer`.
-     - Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
+     1. Tokenize any number of input segments using the `tokenizer`.
+     2. Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
        with the appropriate `"[CLS]"`, `"[SEP]"` and `"<pad>"` tokens.
-     - Construct a dictionary with keys `"token_ids"`, and `"segment_ids"`  that
+     3. Construct a dictionary with keys `"token_ids"`, and `"segment_ids"`  that
        can be passed directly to `keras_nlp.models.FNetBackbone`.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
-    The call method of this layer accepts three arguments, `x`, `y`, and
-    `sample_weight`. `x` can be a python string or tensor representing a single
-    segment, a list of python strings representing a batch of single segments,
-    or a list of tensors representing multiple segments to be packed together.
-    `y` and `sample_weight` are both optional, can have any format, and will be
-    passed through unaltered.
-
-    Special care should be taken when using `tf.data` to map over an unlabeled
-    tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
-    directly into the call arguments of this layer, rather than forward all
-    argument to `x`. To handle this case, it is recommended to  explicitly call
-    the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
-
     Args:
         tokenizer: A `keras_nlp.models.FNetTokenizer` instance.
         sequence_length: The length of the packed inputs.
         truncate: string. The algorithm to truncate a list of batched segments
             to fit within `sequence_length`. The value can be either
             `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
+    Call arguments:
+        x: A tensor of single string sequences, or a tuple of multiple
+            tensor sequences to be packed together. Inputs may be batched or
+            unbatched. For single sequences, raw python inputs will be converted
+            to tensors. For multiple sequences, pass tensors directly.
+        y: Any label data. Will be passed through unaltered.
+        sample_weight: Any label weight data. Will be passed through unaltered.
+
     Examples:
+
+    Directly calling the from_preset().
     ```python
-    tokenizer = keras_nlp.models.FNetTokenizer(proto="model.spm")
-    preprocessor = keras_nlp.models.FNetPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=10,
+    preprocessor = keras_nlp.models.FNetPreprocessor.from_preset(
+        "f_net_base_en"
     )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
     preprocessor("The quick brown fox jumped.")
 
     # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
+
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+    ```
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.FNetPreprocessor.from_preset(
+        "f_net_base_en"
     )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
+
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
     def __init__(
         self,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_preprocessor_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Tests for FNet preprocessor layer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
@@ -31,62 +32,63 @@
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=12,
             model_type="WORD",
             pad_id=3,
             unk_id=0,
             bos_id=4,
             eos_id=5,
             pad_piece="<pad>",
             unk_piece="<unk>",
             bos_piece="[CLS]",
             eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
         self.preprocessor = FNetPreprocessor(
             tokenizer=FNetTokenizer(proto=self.proto),
             sequence_length=12,
         )
 
     def test_tokenize_strings(self):
         input_data = "the quick brown fox"
         output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [4, 1, 9, 2, 7, 5, 3, 3, 3, 3, 3, 3]
+            output["token_ids"], [4, 2, 10, 6, 8, 5, 3, 3, 3, 3, 3, 3]
         )
         self.assertAllEqual(
             output["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         )
 
     def test_tokenize_list_of_strings(self):
-        # We should handle a list of strings as as batch.
+        # We should handle a list of strings as batch.
         input_data = ["the quick brown fox"] * 4
         output = self.preprocessor(input_data)
         self.assertAllEqual(
             output["token_ids"],
-            [[4, 1, 9, 2, 7, 5, 3, 3, 3, 3, 3, 3]] * 4,
+            [[4, 2, 10, 6, 8, 5, 3, 3, 3, 3, 3, 3]] * 4,
         )
         self.assertAllEqual(
             output["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
 
     def test_tokenize_labeled_batch(self):
         x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         x_out, y_out, sw_out = self.preprocessor(x, y, sw)
         self.assertAllEqual(
             x_out["token_ids"],
-            [[4, 1, 9, 2, 7, 5, 3, 3, 3, 3, 3, 3]] * 4,
+            [[4, 2, 10, 6, 8, 5, 3, 3, 3, 3, 3, 3]] * 4,
         )
         self.assertAllEqual(
             x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
@@ -95,62 +97,73 @@
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
         x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
             x_out["token_ids"],
-            [[4, 1, 9, 2, 7, 5, 3, 3, 3, 3, 3, 3]] * 4,
+            [[4, 2, 10, 6, 8, 5, 3, 3, 3, 3, 3, 3]] * 4,
         )
         self.assertAllEqual(
             x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_multiple_sentences(self):
         sentence_one = tf.constant("the quick brown fox")
         sentence_two = tf.constant("the earth")
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
             output["token_ids"],
-            [4, 1, 9, 2, 7, 5, 1, 6, 5, 3, 3, 3],
+            [4, 2, 10, 6, 8, 5, 2, 7, 5, 3, 3, 3],
         )
         self.assertAllEqual(
             output["segment_ids"], [0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]
         )
 
     def test_tokenize_multiple_batched_sentences(self):
         sentence_one = tf.constant(["the quick brown fox"] * 4)
         sentence_two = tf.constant(["the earth"] * 4)
         # The first tuple or list is always interpreted as an enumeration of
         # separate sequences to concatenate.
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
             output["token_ids"],
-            [[4, 1, 9, 2, 7, 5, 1, 6, 5, 3, 3, 3]] * 4,
+            [[4, 2, 10, 6, 8, 5, 2, 7, 5, 3, 3, 3]] * 4,
         )
         self.assertAllEqual(
             output["segment_ids"], [[0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]] * 4
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,57 +11,59 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """FNet model preset configurations."""
 
 backbone_presets = {
     "f_net_base_en": {
+        "metadata": {
+            "description": (
+                "12-layer FNet model where case is maintained. "
+                "Trained on the C4 dataset."
+            ),
+            "params": 82861056,
+            "official_name": "FNet",
+            "path": "f_net",
+            "model_card": "https://github.com/google-research/google-research/blob/master/f_net/README.md",
+        },
         "config": {
             "vocabulary_size": 32000,
             "num_layers": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "num_segments": 4,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "12-layer FNet model where case is maintained. "
-                "Trained on the C4 dataset."
-            ),
-            "params": 82861056,
-            "official_name": "FNet",
-            "path": "fnet",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/f_net_base_en/v1/model.h5",
         "weights_hash": "35db90842b85a985a0e54c86c00746fe",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/f_net_base_en/v1/vocab.spm",
         "spm_proto_hash": "71c5f4610bef1daf116998a113a01f3d",
     },
     "f_net_large_en": {
+        "metadata": {
+            "description": (
+                "24-layer FNet model where case is maintained. "
+                "Trained on the C4 dataset."
+            ),
+            "params": 236945408,
+            "official_name": "FNet",
+            "path": "f_net",
+            "model_card": "https://github.com/google-research/google-research/blob/master/f_net/README.md",
+        },
         "config": {
             "vocabulary_size": 32000,
             "num_layers": 24,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
             "dropout": 0.1,
             "max_sequence_length": 512,
             "num_segments": 4,
         },
         "preprocessor_config": {},
-        "metadata": {
-            "description": (
-                "24-layer FNet model where case is maintained. "
-                "Trained on the C4 dataset."
-            ),
-            "params": 236945408,
-            "official_name": "FNet",
-            "path": "fnet",
-        },
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/f_net_large_en/v1/model.h5",
         "weights_hash": "7ae4a3faa67ff054f8cecffb5619f779",
         "spm_proto_url": "https://storage.googleapis.com/keras-nlp/models/f_net_large_en/v1/vocab.spm",
         "spm_proto_hash": "71c5f4610bef1daf116998a113a01f3d",
     },
 }
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_presets_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = FNetClassifier.from_preset(
             "f_net_base_en",
+            num_classes=2,
             load_weights=load_weights,
         )
         # We don't assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("f_net_tokenizer", FNetTokenizer),
@@ -93,23 +94,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("f_net_tokenizer", FNetTokenizer),
-        ("f_net_preprocessor", FNetPreprocessor),
-        ("f_net", FNetBackbone),
-        ("f_net_classifier", FNetClassifier),
+        ("f_net_tokenizer", FNetTokenizer, {}),
+        ("f_net_preprocessor", FNetPreprocessor, {}),
+        ("f_net", FNetBackbone, {}),
+        ("f_net_classifier", FNetClassifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("f_net_base_en_clowntown")
+            cls.from_preset("f_net_base_en_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
 class FNetPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
 
@@ -137,26 +138,28 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_fnet_classifier(self, load_weights):
         for preset in FNetClassifier.presets:
             classifier = FNetClassifier.from_preset(
                 preset,
+                num_classes=2,
                 load_weights=load_weights,
             )
             input_data = tf.constant(["This quick brown fox"])
             classifier.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_fnet_classifier_without_preprocessing(self, load_weights):
         for preset in FNetClassifier.presets:
             classifier = FNetClassifier.from_preset(
                 preset,
+                num_classes=2,
                 preprocessor=None,
                 load_weights=load_weights,
             )
             input_data = {
                 "token_ids": tf.random.uniform(
                     shape=(1, 512),
                     dtype=tf.int64,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/f_net/f_net_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_tokenizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,133 +8,116 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""FNet tokenizer."""
+"""BART tokenizer."""
 
 import copy
-import os
 
 from tensorflow import keras
 
-from keras_nlp.models.f_net.f_net_presets import backbone_presets
-from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.models.bart.bart_presets import backbone_presets
+from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
-class FNetTokenizer(SentencePieceTokenizer):
-    """FNet tokenizer layer based on SentencePiece.
+class BartTokenizer(BytePairTokenizer):
+    """A BART tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
-    is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by
-    FNet models and provides a `from_preset()` method to automatically
-    download a matching vocabulary for a FNet preset.
+    is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by BART
+    models and provides a `from_preset()` method to automatically download
+    a matching vocabulary for a BART preset.
 
     This tokenizer does not provide truncation or padding of inputs. It can be
-    combined with a `keras_nlp.models.FNetPreprocessor` layer for input
+    combined with a `keras_nlp.models.BartPreprocessor` layer for input
     packing.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
-        proto: Either a `string` path to a SentencePiece proto file, or a
-            `bytes` object with a serialized SentencePiece proto. See the
-            [SentencePiece repository](https://github.com/google/sentencepiece)
-            for more details on the format.
+        vocabulary: string or dict, maps token to integer ids. If it is a
+            string, it should be the file path to a json file.
+        merges: string or list, contains the merge rule. If it is a string,
+            it should be the file path to merge rules. The merge rule file
+            should have one merge rule per line. Every merge rule contains
+            merge entities separated by a space.
 
     Examples:
 
     ```python
-    tokenizer = keras_nlp.models.FNetTokenizer(proto="model.spm")
+    # Unbatched input.
+    tokenizer = keras_nlp.models.BartTokenizer.from_preset(
+        "bart_base_en",
+    )
+    tokenizer("The quick brown fox jumped.")
 
-    # Batched inputs.
-    tokenizer(["the quick brown fox", "the earth is round"])
-
-    # Unbatched inputs.
-    tokenizer("the quick brown fox")
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
 
     # Detokenization.
-    tokenizer.detokenize(tf.constant([[2, 14, 2231, 886, 2385, 3]]))
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.BartTokenizer(
+        vocabulary=vocab,
+        merges=merges,
+    )
+    tokenizer("The quick brown fox jumped.")
     ```
     """
 
-    def __init__(self, proto, **kwargs):
-        super().__init__(proto=proto, **kwargs)
-
-        # Check for necessary special tokens.
-        cls_token = "[CLS]"
-        sep_token = "[SEP]"
+    def __init__(
+        self,
+        vocabulary,
+        merges,
+        **kwargs,
+    ):
+        # Special tokens.
+        start_token = "<s>"
         pad_token = "<pad>"
-        for token in [cls_token, sep_token, pad_token]:
+        end_token = "</s>"
+
+        super().__init__(
+            vocabulary=vocabulary,
+            merges=merges,
+            unsplittable_tokens=[start_token, pad_token, end_token],
+            **kwargs,
+        )
+
+        # Check whether special tokens are present in the vocabulary.
+        for token in [start_token, pad_token, end_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
-        self.cls_token_id = self.token_to_id(cls_token)
-        self.sep_token_id = self.token_to_id(sep_token)
+        self.start_token_id = self.token_to_id(start_token)
         self.pad_token_id = self.token_to_id(pad_token)
+        self.end_token_id = self.token_to_id(end_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
 
-    @classmethod
-    @format_docstring(names=", ".join(backbone_presets))
-    def from_preset(
-        cls,
-        preset,
-        **kwargs,
-    ):
-        """Instantiate an FNet tokenizer from preset vocabulary.
-
-        Args:
-            preset: string. Must be one of {{names}}.
-
-        Examples:
-        ```python
-        # Load a preset tokenizer.
-        tokenizer = keras_nlp.models.FNetTokenizer.from_preset(
-            "f_net_base_en",
-        )
-
-        # Tokenize some input.
-        tokenizer("The quick brown fox tripped.")
-
-        # Detokenize some input.
-        tokenizer.detokenize([5, 6, 7, 8, 9])
-        ```
-        """
-        if preset not in cls.presets:
-            raise ValueError(
-                "`preset` must be one of "
-                f"""{", ".join(cls.presets)}. Received: {preset}."""
-            )
-        metadata = cls.presets[preset]
-
-        spm_proto = keras.utils.get_file(
-            "vocab.spm",
-            metadata["spm_proto_url"],
-            cache_subdir=os.path.join("models", preset),
-            file_hash=metadata["spm_proto_hash"],
-        )
-
-        config = metadata["preprocessor_config"]
-        config.update(
-            {
-                "proto": spm_proto,
-            },
-        )
-
-        return cls.from_config({**config, **kwargs})
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_backbone.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 """GPT-2 backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers import PositionEmbedding
-from keras_nlp.layers import TransformerDecoder
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.position_embedding import PositionEmbedding
+from keras_nlp.layers.transformer_decoder import TransformerDecoder
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
 def _gpt_2_kernel_initializer(stddev=0.02):
     return keras.initializers.RandomNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.GPT2Backbone")
 class GPT2Backbone(Backbone):
     """GPT-2 core network with hyperparameters.
 
     This network implements a Transformer-based decoder network,
     Generative Pretrained Transformer-2 (GPT-2), as described in
     ["Language Models are Unsupervised Multitask Learners"](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf).
     It includes the embedding lookups and transformer layers.
@@ -68,30 +69,28 @@
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
     }
 
-    # Pretrained GPT-2 decoder
-    model = GPT2Backbone.from_preset("gpt2_base_en")
-    output = model(input_data)
+    # Pretrained GPT-2 decoder.
+    model = keras_nlp.models.GPT2Backbone.from_preset("gpt2_base_en")
+    model(input_data)
 
-    # Randomly initialized GPT-2 decoder with custom config
+    # Randomly initialized GPT-2 decoder with custom config.
     model = keras_nlp.models.GPT2Backbone(
         vocabulary_size=50257,
         num_layers=12,
         num_heads=12,
         hidden_dim=768,
         intermediate_dim=3072,
         max_sequence_length=1024,
     )
-
-    # Call the model on the input data.
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
@@ -121,15 +120,17 @@
         position_embedding = PositionEmbedding(
             initializer=_gpt_2_kernel_initializer(stddev=0.02),
             sequence_length=max_sequence_length,
             name="position_embedding",
         )(token_embedding)
 
         # Sum and apply dropout to embeddings.
-        x = keras.layers.Add()((token_embedding, position_embedding))
+        x = keras.layers.Add(name="embeddings_add")(
+            (token_embedding, position_embedding)
+        )
         x = keras.layers.Dropout(
             dropout,
             name="embeddings_dropout",
         )(x)
 
         # Apply successive transformer decoder blocks.
         for i in range(num_layers):
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,90 +7,102 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Test for GPT-2 backbone models."""
+
+"""Tests for RoBERTa tokenizer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
+from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 
 
-class GPT2Test(tf.test.TestCase, parameterized.TestCase):
+class RobertaTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = GPT2Backbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-        )
-        self.batch_size = 8
-        self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+        vocab = {
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
+            "Ġair": 3,
+            "plane": 4,
+            "Ġat": 5,
+            "port": 6,
+            "Ġkoh": 7,
+            "li": 8,
+            "Ġis": 9,
+            "Ġthe": 10,
+            "Ġbest": 11,
+            "<mask>": 12,
         }
 
-        self.input_dataset = tf.data.Dataset.from_tensor_slices(
-            self.input_batch
-        ).batch(2)
-
-    def test_valid_call_gpt2(self):
-        self.model(self.input_batch)
-
-        # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "gpt2_backbone")
-
-    def test_variable_sequence_length_call_gpt2(self):
-        for seq_length in (25, 50, 75):
-            input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-            }
-            self.model(input_data)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
+
+        self.tokenizer = RobertaTokenizer(vocabulary=vocab, merges=merges)
+
+    def test_tokenize(self):
+        input_data = " airplane at airport"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [3, 4, 5, 3, 6])
+
+    def test_tokenize_special_tokens(self):
+        input_data = "<s> airplane at airport</s><pad>"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [0, 3, 4, 5, 3, 6, 0, 1])
+
+    def test_tokenize_batch(self):
+        input_data = tf.constant([" airplane at airport", " kohli is the best"])
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [[3, 4, 5, 3, 6], [7, 8, 9, 10, 11]])
+
+    def test_detokenize(self):
+        input_tokens = [[3, 4, 5, 3, 6]]
+        output = self.tokenizer.detokenize(input_tokens)
+        self.assertAllEqual(output, [" airplane at airport"])
+
+    def test_vocabulary_size(self):
+        self.assertEqual(self.tokenizer.vocabulary_size(), 13)
+
+    def test_errors_missing_special_tokens(self):
+        with self.assertRaises(ValueError):
+            RobertaTokenizer(vocabulary=["a", "b", "c"], merges=[])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, GPT2Backbone)
-
-        # Check that output matches.
-        restored_output = restored_model(self.input_batch)
-        self.assertAllClose(model_output, restored_output)
+        input_data = tf.constant([" airplane at airport"])
+
+        inputs = keras.Input(dtype="string", shape=())
+        outputs = self.tokenizer(inputs)
+        model = keras.Model(inputs, outputs)
+
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
+        restored_model = keras.models.load_model(path)
+        self.assertAllEqual(
+            model(input_data),
+            restored_model(input_data),
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_preprocessor_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,138 +12,139 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for GPT2 causal LM preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
     GPT2CausalLMPreprocessor,
 )
 from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
 class GPT2CausalLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
-            "<|endoftext|>": 0,
-            "!": 1,
-            "air": 2,
-            "Ġair": 3,
-            "plane": 4,
-            "Ġat": 5,
-            "port": 6,
-            "Ġkoh": 7,
-            "li": 8,
-            "Ġis": 9,
-            "Ġthe": 10,
-            "Ġbest": 11,
+            "!": 0,
+            "air": 1,
+            "Ġair": 2,
+            "plane": 3,
+            "Ġat": 4,
+            "port": 5,
+            "<|endoftext|>": 6,
         }
 
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "a i", "p l", "n e"]
-        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "ai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["Ġai r", "Ġa i", "pla ne"]
-        self.merges = merges
+        self.merges = ["Ġ a", "Ġ t", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        self.merges += ["Ġa t", "p o", "r t", "Ġt h", "ai r", "pl a", "po rt"]
+        self.merges += ["Ġai r", "Ġa i", "pla ne"]
 
         self.preprocessor = GPT2CausalLMPreprocessor(
             tokenizer=GPT2Tokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
         )
 
-    def test_tokenize_strings(self):
+    def test_strings(self):
         input_data = "airplane at airport"
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(x["token_ids"], [2, 4, 5, 3, 6, 0, 0])
-        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 0, 0])
-        self.assertAllEqual(y, [4, 5, 3, 6, 0, 0, 0])
-        self.assertAllEqual(sw, [1, 1, 1, 1, 0, 0, 0])
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
+        self.assertAllEqual(y, [1, 3, 4, 2, 5, 6, 0, 0])
+        self.assertAllEqual(sw, [1, 1, 1, 1, 1, 1, 0, 0])
 
-    def test_tokenize_list_of_strings(self):
+    def test_list_of_strings(self):
         input_data = ["airplane at airport"] * 4
 
         x, y, sw = self.preprocessor(input_data)
-        self.assertAllEqual(
-            x["token_ids"],
-            [[2, 4, 5, 3, 6, 0, 0]] * 4,
-        )
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0]] * 4)
-        self.assertAllEqual(y, [[4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
-    def test_pad_start_end_token(self):
+    def test_no_start_end_token(self):
         input_data = ["airplane at airport"] * 4
 
         preprocessor = GPT2CausalLMPreprocessor(
             tokenizer=GPT2Tokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
-            add_start_token=True,
-            add_end_token=True,
+            add_start_token=False,
+            add_end_token=False,
         )
         x, y, sw = preprocessor(input_data)
-        self.assertAllEqual(
-            x["token_ids"],
-            [[0, 2, 4, 5, 3, 6, 0]] * 4,
-        )
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1]] * 4)
-        self.assertAllEqual(y, [[2, 4, 5, 3, 6, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 2, 5, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
+        self.assertAllEqual(y, [[3, 4, 2, 5, 0, 0, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0, 0]] * 4)
 
-    def test_tokenize_labeled_batch(self):
+    def test_labeled_batch(self):
         x = tf.constant(["airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
+        y = tf.constant([1] * 4)  # Ignored.
+        sw = tf.constant([1.0] * 4)  # Ignored.
         x, y, sw = self.preprocessor(x, y, sw)
-        self.assertAllEqual(
-            x["token_ids"],
-            [[2, 4, 5, 3, 6, 0, 0]] * 4,
-        )
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0]] * 4)
-        self.assertAllEqual(y, [[4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
-    def test_tokenize_labeled_dataset(self):
+    def test_dataset(self):
         x = tf.constant(["airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
+        ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
         x, y, sw = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[6, 1, 3, 4, 2, 5, 6, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, [[1, 3, 4, 2, 5, 6, 0, 0]] * 4)
+        self.assertAllEqual(sw, [[1, 1, 1, 1, 1, 1, 0, 0]] * 4)
 
-        self.assertAllEqual(
-            x["token_ids"],
-            [[2, 4, 5, 3, 6, 0, 0]] * 4,
+    def test_call_overrides(self):
+        input_data = "airplane at airport"
+        x, _, _ = self.preprocessor(input_data, add_start_token=False)
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 2, 5, 6, 0, 0])
+        x, _, _ = self.preprocessor(input_data, add_end_token=False)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 0, 0])
+        x, _, _ = self.preprocessor(input_data, sequence_length=4)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4])
+        x = self.preprocessor(input_data, return_labels=False)
+        self.assertAllEqual(x["token_ids"], [6, 1, 3, 4, 2, 5, 6, 0])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
-        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0]] * 4)
-        self.assertAllEqual(y, [[4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(sw, [[1, 1, 1, 1, 0, 0, 0]] * 4)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs, y, sw = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_causal_lm_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,154 +7,155 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for GPT2 causal LM model."""
+
+"""Tests for BART preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
-from keras_nlp.models.gpt2.gpt2_causal_lm import GPT2CausalLM
-from keras_nlp.models.gpt2.gpt2_causal_lm_preprocessor import (
-    GPT2CausalLMPreprocessor,
+from keras_nlp.models.bart.bart_seq_2_seq_lm_preprocessor import (
+    BartSeq2SeqLMPreprocessor,
 )
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.models.bart.bart_tokenizer import BartTokenizer
 
 
-class GPT2CausalLMTest(tf.test.TestCase, parameterized.TestCase):
+class BartSeq2SeqLMPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        backbone = GPT2Backbone(
-            vocabulary_size=1000,
-            num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-        )
         vocab = {
-            "<|endoftext|>": 0,
-            "!": 1,
-            "air": 2,
+            "<s>": 0,
+            "<pad>": 1,
+            "</s>": 2,
             "Ġair": 3,
             "plane": 4,
             "Ġat": 5,
             "port": 6,
             "Ġkoh": 7,
             "li": 8,
             "Ġis": 9,
             "Ġthe": 10,
             "Ġbest": 11,
+            "<mask>": 12,
         }
 
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "ai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["Ġai r", "Ġa i", "pla ne"]
-
-        self.preprocessor = GPT2CausalLMPreprocessor(
-            GPT2Tokenizer(vocabulary=vocab, merges=merges),
-            sequence_length=8,
-        )
-        self.causal_lm = GPT2CausalLM(
-            backbone,
-            preprocessor=self.preprocessor,
-        )
-        self.causal_lm_no_preprocessing = GPT2CausalLM(
-            backbone,
-            preprocessor=None,
-        )
-
-        self.raw_batch = tf.constant(
-            [
-                " airplane at airport",
-                " the airplane is the best",
-                " the best airport",
-                " kohli is the best",
-            ]
-        )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)[0]
-        self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            self.raw_batch
-        ).batch(2)
-        self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
-
-    def test_valid_call_causal_lm(self):
-        self.causal_lm(self.preprocessed_batch)
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_causal_lm_predict(self, jit_compile):
-        self.causal_lm.compile(jit_compile=jit_compile)
-        self.causal_lm.predict(self.raw_batch)
+        self.preprocessor = BartSeq2SeqLMPreprocessor(
+            tokenizer=BartTokenizer(
+                vocabulary=vocab,
+                merges=merges,
+            ),
+            encoder_sequence_length=10,
+            decoder_sequence_length=9,
+        )
+
+    def test_tokenize_strings(self):
+        input_data = {
+            "encoder_text": " airplane at airport",
+            "decoder_text": " kohli is the best",
+        }
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_causal_lm_predict_no_preprocessing(self, jit_compile):
-        self.causal_lm_no_preprocessing.compile(jit_compile=jit_compile)
-        self.causal_lm_no_preprocessing.predict(self.preprocessed_batch)
+        x_out, y_out, sw_out = self.preprocessor(input_data)
+        self.assertAllEqual(
+            x_out["encoder_token_ids"], [0, 3, 4, 5, 3, 6, 2, 1, 1, 1]
+        )
+        self.assertAllEqual(
+            x_out["encoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            x_out["decoder_token_ids"], [2, 0, 7, 8, 9, 10, 11, 2, 1]
+        )
+        self.assertAllEqual(
+            x_out["decoder_padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 0]
+        )
+        self.assertAllEqual(y_out, [0, 7, 8, 9, 10, 11, 2, 1, 1])
+        self.assertAllEqual(sw_out, [1, 1, 1, 1, 1, 1, 1, 0, 0])
+
+    def test_tokenize_list_of_strings(self):
+        input_data = {
+            "encoder_text": [" airplane at airport"] * 4,
+            "decoder_text": [" kohli is the best"] * 4,
+        }
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_causal_lm_fit(self, jit_compile):
-        self.causal_lm.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
-        )
-        self.causal_lm.fit(self.raw_dataset)
+        x_out, y_out, sw_out = self.preprocessor(input_data)
+        self.assertAllEqual(
+            x_out["encoder_token_ids"], [[0, 3, 4, 5, 3, 6, 2, 1, 1, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["encoder_padding_mask"],
+            [[1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4,
+        )
+        self.assertAllEqual(
+            x_out["decoder_token_ids"], [[2, 0, 7, 8, 9, 10, 11, 2, 1]] * 4
+        )
+        self.assertAllEqual(
+            x_out["decoder_padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 0]] * 4
+        )
+        self.assertAllEqual(y_out, [[0, 7, 8, 9, 10, 11, 2, 1, 1]] * 4)
+        self.assertAllEqual(sw_out, [[1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4)
+
+    def test_error_multi_segment_input(self):
+        input_data = {
+            "encoder_text": (
+                tf.constant([" airplane at airport"] * 2),
+                tf.constant([" airplane"] * 2),
+            ),
+            "decoder_text": (
+                tf.constant([" kohli is the best"] * 2),
+                tf.constant([" kohli"] * 2),
+            ),
+        }
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_causal_lm_fit_no_preprocessing(self, jit_compile):
-        self.causal_lm_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
-        )
-        self.causal_lm_no_preprocessing.fit(self.preprocessed_dataset)
+        with self.assertRaises(ValueError):
+            self.preprocessor(input_data)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_gpt2_causal_lm_generate(self, jit_compile):
-        self.causal_lm_no_preprocessing.compile(jit_compile=jit_compile)
-        self.causal_lm.generate(
-            self.raw_batch,
-            max_length=10,
+    def test_serialization(self):
+        new_preprocessor = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.preprocessor)
         )
-
-        # String input
-        prompt = " airplane"
-        generated = self.causal_lm.generate(
-            prompt,
-            max_length=10,
+        self.assertEqual(
+            new_preprocessor.get_config(), self.preprocessor.get_config()
         )
-        generated = generated.numpy().decode("utf-8")
-        self.assertTrue(prompt in generated)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        keras.utils.set_random_seed(42)
-        model_output = self.causal_lm.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.causal_lm.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
-
-        # Check we got the real object back.
-        self.assertIsInstance(restored_model, GPT2CausalLM)
-
-        # Check that output matches.
-        keras.utils.set_random_seed(42)
-        restored_output = restored_model.predict(self.raw_batch)
-        self.assertAllClose(model_output, restored_output)
+        input_data = {
+            "encoder_text": tf.constant(" airplane at airport"),
+            "decoder_text": tf.constant(" kohli is the best"),
+        }
+
+        inputs = {
+            "encoder_text": keras.Input(dtype="string", shape=()),
+            "decoder_text": keras.Input(dtype="string", shape=()),
+        }
+        outputs = self.preprocessor(inputs)
+        model = keras.Model(inputs=inputs, outputs=outputs)
+
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
+
+        restored_model = keras.models.load_model(path)
+
+        model_output = model(input_data)
+        restored_model_output = restored_model(input_data)
+
+        self.assertAllClose(
+            model_output,
+            restored_model_output,
+        )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,198 +1,196 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""GPT2 preprocessor layer."""
+"""XLM-RoBERTa preprocessor layer."""
 
 import copy
 
-import tensorflow as tf
-from tensorflow import keras
-
-from keras_nlp.models.gpt2.gpt2_presets import backbone_presets
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.preprocessor import Preprocessor
+from keras_nlp.models.roberta.roberta_preprocessor import (
+    RobertaMultiSegmentPacker,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
+    XLMRobertaTokenizer,
+)
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class GPT2Preprocessor(Preprocessor):
-    """GPT2 preprocessing layer which tokenizes and packs inputs.
-
-    This preprocessing layer will do 2 things:
-
-    - Tokenize the input using the `tokenizer`.
-    - Construct a dictionary with keys `"token_ids"`, `"padding_mask"`, that can
-        be passed directly to a `keras_nlp.models.GPT2Backbone`.
+@keras_nlp_export("keras_nlp.models.XLMRobertaPreprocessor")
+class XLMRobertaPreprocessor(Preprocessor):
+    """An XLM-RoBERTa preprocessing layer which tokenizes and packs inputs.
+
+    This preprocessing layer will do three things:
+
+    1. Tokenize any number of input segments using the `tokenizer`.
+    2. Pack the inputs together using a `keras_nlp.layers.MultiSegmentPacker`.
+      with the appropriate `"<s>"`, `"</s>"` and `"<pad>"` tokens, i.e., adding
+      a single `"<s>"` at the start of the entire sequence, `"</s></s>"` at the
+      end of each segment, save the last and a `"</s>"` at the end of the
+      entire sequence.
+    3. Construct a dictionary with keys `"token_ids"` and `"padding_mask"`,
+      that can be passed directly to an XLM-RoBERTa model.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
-    The call method of this layer accepts three arguments, `x`, `y`, and
-    `sample_weight`. `x` can be a python string or tensor representing a single
-    segment, a list of python strings representing a batch of single segments,
-    or a list of tensors representing multiple segments to be packed together.
-    `y` and `sample_weight` are both optional, can have any format, and will be
-    passed through unaltered.
-
-    `GPT2Preprocessor` forces the input to have only one segment, as GPT2 is
-    mainly used for generation tasks. For tasks having multi-segment inputs
-    like "glue/mnli", please use a model designed for classification purposes
-    such as BERT or RoBERTa.
-
     Args:
-        tokenizer: A `keras_nlp.models.GPT2Tokenizer` instance.
+        tokenizer: A `keras_nlp.tokenizers.XLMRobertaTokenizer` instance.
         sequence_length: The length of the packed inputs.
-        add_start_token: If true, the preprocessor will append the tokenizer
-            start token to each input sequence.
-        add_end_token: If true, the preprocessor will append the tokenizer
-            end token to each input sequence.
+        truncate: The algorithm to truncate a list of batched segments to fit
+            within `sequence_length`. The value can be either `round_robin` or
+            `waterfall`:
+                - `"round_robin"`: Available space is assigned one token at a
+                    time in a round-robin fashion to the inputs that still need
+                    some, until the limit is reached.
+                - `"waterfall"`: The allocation of the budget is done using a
+                    "waterfall" algorithm that allocates quota in a
+                    left-to-right manner and fills up the buckets until we run
+                    out of budget. It supports an arbitrary number of segments.
+
+    Call arguments:
+        x: A tensor of single string sequences, or a tuple of multiple
+            tensor sequences to be packed together. Inputs may be batched or
+            unbatched. For single sequences, raw python inputs will be converted
+            to tensors. For multiple sequences, pass tensors directly.
+        y: Any label data. Will be passed through unaltered.
+        sample_weight: Any label weight data. Will be passed through unaltered.
 
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.GPT2Preprocessor.from_preset("gpt2_base_en")
+    preprocessor = keras_nlp.models.XLMRobertaPreprocessor.from_preset(
+        "xlm_roberta_base_multi"
+    )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant("League of legends")
-    preprocessor(sentence)
-    # Same output.
-    preprocessor("League of legends")
-
-    # Tokenize a batch of sentences.
-    sentences = tf.constant(["Taco tuesday", "Fish taco!"])
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(["Taco tuesday", "Fish taco!"])
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        [
-            "Avatar 2 is amazing!",
-            "Well, I am not sure.",
-        ]
+    preprocessor("The quick brown fox jumped.")
+
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "اسمي اسماعيل"])
+
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "اسمي اسماعيل"])
+    second = tf.constant(["The fox tripped.", "الأسد ملك الغابة"])
+    preprocessor((first, second))
+
+    # Custom vocabulary.
+    def train_sentencepiece(ds, vocab_size):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=ds.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=vocab_size,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        return bytes_io.getvalue()
+    ds = tf.data.Dataset.from_tensor_slices(
+        ["the quick brown fox", "the earth is round"]
     )
-    labels = tf.constant([1, 0])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+    proto = train_sentencepiece(ds, vocab_size=10)
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer(proto=proto)
+    preprocessor = keras_nlp.models.XLMRobertaPreprocessor(tokenizer)
+    preprocessor("The quick brown fox jumped.")
+    ```
+
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.XLMRobertaPreprocessor.from_preset(
+        "xlm_roberta_base_multi"
+    )
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabled sentences.
-    ds = tf.data.Dataset.from_tensor_slices(features)
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as above.
-    vocab = {
-        "<s>": 0,
-        "<pad>": 1,
-        "</s>": 2,
-        "Ġafter": 5,
-        "noon": 6,
-        "Ġsun": 7,
-    }
-    merges = ["Ġ a", "Ġ s", "Ġ n", "e r", "n o", "o n", "Ġs u", "Ġa f", "no on"]
-    merges += ["Ġsu n", "Ġaf t", "Ġaft er"]
-
-    tokenizer = keras_nlp.models.GPT2Tokenizer(
-        vocabulary=vocab,
-        merges=merges,
-    )
-    preprocessor = keras_nlp.models.GPT2Preprocessor(
-        tokenizer=tokenizer,
-        sequence_length=20,
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
+    # Watch out for tf.data's default unpacking of tuples here!
+    # Best to invoke the `preprocessor` directly in this case.
+    ds = ds.map(
+        lambda first, second: preprocessor(x=(first, second)),
+        num_parallel_calls=tf.data.AUTOTUNE,
     )
     ```
     """
 
     def __init__(
         self,
         tokenizer,
-        sequence_length,
-        add_start_token=False,
-        add_end_token=False,
+        sequence_length=512,
+        truncate="round_robin",
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.tokenizer = tokenizer
-        self.sequence_length = sequence_length
-        self.add_start_token = add_start_token
-        self.add_end_token = add_end_token
+
+        self.packer = RobertaMultiSegmentPacker(
+            start_value=self.tokenizer.start_token_id,
+            end_value=self.tokenizer.end_token_id,
+            pad_value=self.tokenizer.pad_token_id,
+            truncate=truncate,
+            sequence_length=sequence_length,
+        )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "sequence_length": self.sequence_length,
+                "sequence_length": self.packer.sequence_length,
+                "truncate": self.packer.truncate,
             }
         )
         return config
 
     def call(self, x, y=None, sample_weight=None):
         x = convert_inputs_to_list_of_tensor_segments(x)
-        if len(x) > 1:
-            raise ValueError(
-                "GPT2 requires each input feature to contain only "
-                f"one segment, but received {len(x)}. If you are using GPT2 "
-                "for a multi-segment classification task, please refer to "
-                "classification models like BERT or RoBERTa."
-            )
-        token_ids = self.tokenizer(x[0])
-        input_is_1d = len(token_ids.shape) == 1
-        if input_is_1d:
-            token_ids = tf.RaggedTensor.from_tensor([token_ids])
-        if self.add_start_token:
-            start_tokens = tf.fill(
-                [tf.shape(token_ids)[0], 1],
-                self.tokenizer.start_token_id,
-            )
-            token_ids = tf.concat([start_tokens, token_ids], axis=1)
-        if self.add_end_token:
-            end_tokens = tf.fill(
-                [tf.shape(token_ids)[0], 1],
-                self.tokenizer.end_token_id,
-            )
-            token_ids = tf.concat([token_ids, end_tokens], axis=1)
-        mask = tf.ones_like(token_ids, dtype=tf.bool)
-        shape_after_padding = tf.stack(
-            [tf.constant(-1), self.sequence_length],
-            axis=0,
-        )
-        mask = mask.to_tensor(shape=shape_after_padding)
-        token_ids = token_ids.to_tensor(
-            shape=shape_after_padding,
-            default_value=self.tokenizer.pad_token_id,
-        )
-        if input_is_1d:
-            # If the input is a single string, we let the output be a 1D tensor.
-            token_ids = tf.squeeze(token_ids, axis=0)
-            mask = tf.squeeze(mask, axis=0)
+        x = [self.tokenizer(segment) for segment in x]
+        token_ids = self.packer(x)
         x = {
             "token_ids": token_ids,
-            "padding_mask": mask,
+            "padding_mask": token_ids != self.tokenizer.pad_token_id,
         }
-
         return pack_x_y_sample_weight(x, y, sample_weight)
 
     @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
+    def tokenizer_cls(cls):
+        return XLMRobertaTokenizer
 
     @classproperty
-    def tokenizer_cls(cls):
-        return GPT2Tokenizer
+    def presets(cls):
+        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_preprocessor_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,138 +8,133 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT2 preprocessor layer."""
+"""Tests for OPT preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_preprocessor import GPT2Preprocessor
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.models.opt.opt_preprocessor import OPTPreprocessor
+from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
 
 
-class GPT2PreprocessorTest(tf.test.TestCase, parameterized.TestCase):
+class OPTPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
-            "<|endoftext|>": 0,
-            "!": 1,
+            "<pad>": 0,
+            "</s>": 1,
             "air": 2,
             "Ġair": 3,
             "plane": 4,
             "Ġat": 5,
             "port": 6,
-            "Ġkoh": 7,
-            "li": 8,
-            "Ġis": 9,
-            "Ġthe": 10,
-            "Ġbest": 11,
         }
 
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "a i", "p l", "n e"]
+        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "ai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["Ġai r", "Ġa i", "pla ne"]
+        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
+        merges += ["pla ne"]
         self.merges = merges
 
-        self.preprocessor = GPT2Preprocessor(
-            tokenizer=GPT2Tokenizer(
+        self.preprocessor = OPTPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
         )
 
     def test_tokenize_strings(self):
-        input_data = "airplane at airport"
+        input_data = " airplane at airport"
 
-        output = self.preprocessor(input_data)
-        self.assertAllEqual(output["token_ids"], [2, 4, 5, 3, 6, 0, 0, 0])
-        self.assertAllEqual(output["padding_mask"], [1, 1, 1, 1, 1, 0, 0, 0])
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 1, 0])
+        self.assertAllEqual(x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0])
 
     def test_tokenize_list_of_strings(self):
-        input_data = ["airplane at airport"] * 4
+        input_data = [" airplane at airport"] * 4
 
-        output = self.preprocessor(input_data)
-        self.assertAllEqual(
-            output["token_ids"],
-            [[2, 4, 5, 3, 6, 0, 0, 0]] * 4,
-        )
+        x = self.preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
 
-        self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4
-        )
+    def test_no_start_end_token(self):
+        input_data = [" airplane at airport"] * 4
 
-    def test_pad_start_end_token(self):
-        input_data = ["airplane at airport"] * 4
-
-        preprocessor = GPT2Preprocessor(
-            tokenizer=GPT2Tokenizer(
+        preprocessor = OPTPreprocessor(
+            tokenizer=OPTTokenizer(
                 vocabulary=self.vocab,
                 merges=self.merges,
             ),
             sequence_length=8,
-            add_start_token=True,
-            add_end_token=True,
-        )
-        output = preprocessor(input_data)
-        self.assertAllEqual(
-            output["token_ids"],
-            [[0, 2, 4, 5, 3, 6, 0, 0]] * 4,
-        )
-
-        self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4
+            add_start_token=False,
+            add_end_token=False,
         )
+        x = preprocessor(input_data)
+        self.assertAllEqual(x["token_ids"], [[3, 4, 5, 3, 6, 0, 0, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4)
 
     def test_tokenize_labeled_batch(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        x_out, y_out, sw_out = self.preprocessor(x, y, sw)
-        self.assertAllEqual(x_out["token_ids"], [[2, 4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4
-        )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
+        x = tf.constant([" airplane at airport"] * 4)
+        y_in = tf.constant([1] * 4)
+        sw_in = tf.constant([1.0] * 4)
+        x, y, sw = self.preprocessor(x, y_in, sw_in)
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+        self.assertAllEqual(y, y_in)
+        self.assertAllEqual(sw, sw_in)
 
     def test_tokenize_labeled_dataset(self):
-        x = tf.constant(["airplane at airport"] * 4)
-        y = tf.constant([1] * 4)
-        sw = tf.constant([1.0] * 4)
-        ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
+        x = tf.constant([" airplane at airport"] * 4)
+        ds = tf.data.Dataset.from_tensor_slices(x)
         ds = ds.map(self.preprocessor)
-        x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
-
-        self.assertAllEqual(x_out["token_ids"], [[2, 4, 5, 3, 6, 0, 0, 0]] * 4)
-        self.assertAllEqual(
-            x_out["padding_mask"], [[1, 1, 1, 1, 1, 0, 0, 0]] * 4
+        x = ds.batch(4).take(1).get_single_element()
+        self.assertAllEqual(x["token_ids"], [[1, 3, 4, 5, 3, 6, 1, 0]] * 4)
+        self.assertAllEqual(x["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 0]] * 4)
+
+    def test_call_overrides(self):
+        input_data = " airplane at airport"
+        x = self.preprocessor(input_data, add_start_token=False)
+        self.assertAllEqual(x["token_ids"], [3, 4, 5, 3, 6, 1, 0, 0])
+        x = self.preprocessor(input_data, add_end_token=False)
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 5, 3, 6, 0, 0])
+        x = self.preprocessor(input_data, sequence_length=4)
+        self.assertAllEqual(x["token_ids"], [1, 3, 4, 1])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
         )
-        self.assertAllEqual(y_out, y)
-        self.assertAllEqual(sw_out, sw)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        input_data = tf.constant(["airplane at airport"])
+        input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,28 +20,26 @@
             "description": (
                 "12-layer GPT-2 model where case is maintained. "
                 "Trained on WebText."
             ),
             "params": 124439808,
             "official_name": "GPT-2",
             "path": "gpt2",
+            "model_card": "https://github.com/openai/gpt-2/blob/master/model_card.md",
         },
         "config": {
             "vocabulary_size": 50257,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "description": (
-            "Base size of GPT-2 with 124M parameters. Trained on WebText."
-        ),
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en/v1/model.h5",
         "weights_hash": "f4ea6e1b214516dd7de452461ee6e16e",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en/v1/vocab.json",
         "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
@@ -50,28 +48,26 @@
             "description": (
                 "24-layer GPT-2 model where case is maintained. "
                 "Trained on WebText."
             ),
             "params": 354823168,
             "official_name": "GPT-2",
             "path": "gpt2",
+            "model_card": "https://github.com/openai/gpt-2/blob/master/model_card.md",
         },
         "config": {
             "vocabulary_size": 50257,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "description": (
-            "Medium size of GPT-2 with 355M parameters. Trained on WebText."
-        ),
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_medium_en/v1/model.h5",
         "weights_hash": "580ff9b79c04fc90e6d6f47e975c5afe",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_medium_en/v1/vocab.json",
         "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_medium_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
@@ -80,28 +76,26 @@
             "description": (
                 "36-layer GPT-2 model where case is maintained. "
                 "Trained on WebText."
             ),
             "params": 774030080,
             "official_name": "GPT-2",
             "path": "gpt2",
+            "model_card": "https://github.com/openai/gpt-2/blob/master/model_card.md",
         },
         "config": {
             "vocabulary_size": 50257,
             "num_layers": 36,
             "num_heads": 20,
             "hidden_dim": 1280,
             "intermediate_dim": 5120,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "description": (
-            "Large size of GPT-2 with 774M parameters. Trained on WebText."
-        ),
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_large_en/v1/model.h5",
         "weights_hash": "67957cb3dfc9e965960dabe068811e1a",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_large_en/v1/vocab.json",
         "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_large_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
@@ -110,30 +104,54 @@
             "description": (
                 "48-layer GPT-2 model where case is maintained. "
                 "Trained on WebText."
             ),
             "params": 1557611200,
             "official_name": "GPT-2",
             "path": "gpt2",
+            "model_card": "https://github.com/openai/gpt-2/blob/master/model_card.md",
         },
         "config": {
             "vocabulary_size": 50257,
             "num_layers": 48,
             "num_heads": 25,
             "hidden_dim": 1600,
             "intermediate_dim": 6400,
             "dropout": 0.1,
             "max_sequence_length": 1024,
         },
         "preprocessor_config": {},
-        "description": (
-            "Extra large size of GPT-2 with 1558M parameters. "
-            "Trained on WebText."
-        ),
         "weights_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_extra_large_en/v1/model.h5",
         "weights_hash": "d093c1ee0d9705d845c0190909aa2917",
         "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_extra_large_en/v1/vocab.json",
         "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
         "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_extra_large_en/v1/merges.txt",
         "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
     },
+    "gpt2_base_en_cnn_dailymail": {
+        "metadata": {
+            "description": (
+                "12-layer GPT-2 model where case is maintained. "
+                "Finetuned on the CNN/DailyMail summarization dataset."
+            ),
+            "params": 124439808,
+            "official_name": "GPT-2",
+            "path": "gpt2",
+        },
+        "config": {
+            "vocabulary_size": 50257,
+            "num_layers": 12,
+            "num_heads": 12,
+            "hidden_dim": 768,
+            "intermediate_dim": 3072,
+            "dropout": 0.1,
+            "max_sequence_length": 1024,
+        },
+        "preprocessor_config": {},
+        "weights_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en_news/v1/model.h5",
+        "weights_hash": "09d86ca6e1b4213886b720a1392f2a70",
+        "vocabulary_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en_news/v1/vocab.json",
+        "vocabulary_hash": "dffec25a898b1f5e569bec4dffd7e5c0",
+        "merges_url": "https://storage.googleapis.com/keras-nlp/models/gpt2_base_en_news/v1/merges.txt",
+        "merges_hash": "75a37753dd7a28a2c5df80c28bf06e4e",
+    },
 }
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_tokenizer_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,84 +8,100 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for GPT-2 preprocessing layers."""
+"""Tests for OPT tokenizer layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
+from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
 
 
-class GPT2TokenizerTest(tf.test.TestCase, parameterized.TestCase):
+class OPTTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
-            "<|endoftext|>": 0,
-            "Ġair": 1,
-            "plane": 2,
-            "Ġat": 3,
-            "port": 4,
-            "Ġkoh": 5,
-            "li": 6,
-            "Ġis": 7,
-            "Ġthe": 8,
-            "Ġbest": 9,
+            "<pad>": 0,
+            "</s>": 1,
+            "Ġair": 2,
+            "plane": 3,
+            "Ġat": 4,
+            "port": 5,
+            "Ġkoh": 6,
+            "li": 7,
+            "Ġis": 8,
+            "Ġthe": 9,
+            "Ġbest": 10,
         }
 
         merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
         merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
         merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
         merges += ["pla ne"]
         self.merges = merges
 
-        self.tokenizer = GPT2Tokenizer(
-            vocabulary=self.vocab, merges=self.merges
-        )
+        self.tokenizer = OPTTokenizer(vocabulary=self.vocab, merges=self.merges)
 
     def test_tokenize(self):
         input_data = " airplane at airport"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [1, 2, 3, 1, 4])
+        self.assertAllEqual(output, [2, 3, 4, 2, 5])
+
+    def test_tokenize_special_tokens(self):
+        input_data = "</s> airplane at airport</s><pad>"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [1, 2, 3, 4, 2, 5, 1, 0])
 
     def test_tokenize_batch(self):
         input_data = tf.constant([" airplane at airport", " kohli is the best"])
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[1, 2, 3, 1, 4], [5, 6, 7, 8, 9]])
+        self.assertAllEqual(output, [[2, 3, 4, 2, 5], [6, 7, 8, 9, 10]])
 
     def test_detokenize(self):
-        input_tokens = [1, 2, 3, 1, 4]
+        input_tokens = [2, 3, 4, 2, 5]
         output = self.tokenizer.detokenize(input_tokens)
         self.assertEqual(output, " airplane at airport")
 
     def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 10)
+        self.assertEqual(self.tokenizer.vocabulary_size(), 11)
 
     def test_errors_missing_special_tokens(self):
         with self.assertRaises(ValueError):
-            GPT2Tokenizer(vocabulary=["a", "b", "c"], merges=[])
+            OPTTokenizer(vocabulary=["a", "b", "c"], merges=[])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,37 @@
 """OPT backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.token_and_position_embedding import (
     TokenAndPositionEmbedding,
 )
 from keras_nlp.layers.transformer_decoder import TransformerDecoder
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.opt.opt_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
 def opt_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.OPTBackbone")
 class OPTBackbone(Backbone):
-    """OPT decoder network.
+    """An OPT decoder network.
 
     This class implements a Transformer-based decoder model as described in
     ["OPT: Open Pre-trained Transformer Language Models"](https://arxiv.org/abs/2205.01068).
     The default constructor gives a fully customizable, randomly initialized OPT
     model with any number of layers, heads, and embedding dimensions. To load
-    preset architectures and weights, use the `from_preset` constructor.
+    preset architectures and weights, use the `from_preset()` constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq/).
 
     Args:
@@ -68,26 +69,26 @@
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)
         ),
     }
 
     # Pretrained OPT decoder
     model = keras_nlp.models.OPTBackbone.from_preset("opt_125m_en")
-    output = model(input_data)
+    model(input_data)
 
     # Randomly initialized OPT decoder model with a custom config
     model = keras_nlp.models.OPTBackbone(
         vocabulary_size=50265,
-        num_layers=6,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_backbone_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,86 +11,108 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Test for OPT backbone models."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.opt.opt_backbone import OPTBackbone
 
 
 class OPTTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = OPTBackbone(
-            vocabulary_size=1000,
+        self.backbone = OPTBackbone(
+            vocabulary_size=10,
             num_layers=2,
             num_heads=2,
-            hidden_dim=32,
-            intermediate_dim=128,
-            max_sequence_length=128,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=5,
         )
-        self.batch_size = 8
         self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "padding_mask": tf.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
     def test_valid_call_opt(self):
-        self.model(self.input_batch)
+        self.backbone(self.input_batch)
 
+    def test_token_embedding(self):
+        output = self.backbone.token_embedding(self.input_batch["token_ids"])
+        self.assertEqual(output.shape, (2, 5, 2))
+
+    def test_name(self):
         # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "opt_backbone")
+        self.assertRegexpMatches(self.backbone.name, "opt_backbone")
 
     def test_variable_sequence_length_call_opt(self):
-        for seq_length in (25, 50, 75):
+        for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "padding_mask": tf.ones((2, seq_length), dtype="int32"),
             }
-            self.model(input_data)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_opt_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+            self.backbone(input_data)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_opt_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
+    def test_predict(self):
+        self.backbone.predict(self.input_batch)
+        self.backbone.predict(self.input_dataset)
+
+    def test_serialization(self):
+        new_backbone = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.backbone)
+        )
+        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.backbone(self.input_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.backbone.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, OPTBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
         self.assertAllClose(model_output, restored_output)
+
+
+@pytest.mark.tpu
+@pytest.mark.usefixtures("tpu_test_class")
+class OPTBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+    def setUp(self):
+        with self.tpu_strategy.scope():
+            self.backbone = OPTBackbone(
+                vocabulary_size=1000,
+                num_layers=2,
+                num_heads=2,
+                hidden_dim=32,
+                intermediate_dim=128,
+                max_sequence_length=128,
+            )
+        self.input_batch = {
+            "token_ids": tf.ones((8, 128), dtype="int32"),
+            "padding_mask": tf.ones((8, 128), dtype="int32"),
+        }
+        self.input_dataset = tf.data.Dataset.from_tensor_slices(
+            self.input_batch
+        ).batch(2)
+
+    def test_predict(self):
+        self.backbone.compile()
+        self.backbone.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             "description": (
                 "12-layer OPT model where case in maintained. Trained on "
                 "BookCorpus, CommonCrawl, Pile, and PushShift.io corpora."
             ),
             "params": 125237760,
             "official_name": "OPT",
             "path": "opt",
+            "model_card": "https://github.com/facebookresearch/metaseq/blob/main/projects/OPT/model_card.md",
         },
         "config": {
             "vocabulary_size": 50272,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -49,14 +50,15 @@
             "description": (
                 "24-layer OPT model where case in maintained. Trained on "
                 "BookCorpus, CommonCrawl, Pile, and PushShift.io corpora."
             ),
             "params": 1315753984,
             "official_name": "OPT",
             "path": "opt",
+            "model_card": "https://github.com/facebookresearch/metaseq/blob/main/projects/OPT/model_card.md",
         },
         "config": {
             "vocabulary_size": 50272,
             "num_layers": 24,
             "num_heads": 32,
             "hidden_dim": 2048,
             "intermediate_dim": 8192,
@@ -76,14 +78,15 @@
             "description": (
                 "32-layer OPT model where case in maintained. Trained on "
                 "BookCorpus, CommonCrawl, Pile, and PushShift.io corpora."
             ),
             "params": 2700000000,
             "official_name": "OPT",
             "path": "opt",
+            "model_card": "https://github.com/facebookresearch/metaseq/blob/main/projects/OPT/model_card.md",
         },
         "config": {
             "vocabulary_size": 50272,
             "num_layers": 32,
             "num_heads": 32,
             "hidden_dim": 2560,
             "intermediate_dim": 10240,
@@ -103,14 +106,15 @@
             "description": (
                 "32-layer OPT model where case in maintained. Trained on "
                 "BookCorpus, CommonCrawl, Pile, and PushShift.io corpora."
             ),
             "params": 6700000000,
             "official_name": "OPT",
             "path": "opt",
+            "model_card": "https://github.com/facebookresearch/metaseq/blob/main/projects/OPT/model_card.md",
         },
         "config": {
             "vocabulary_size": 50272,
             "num_layers": 32,
             "num_heads": 32,
             "hidden_dim": 4096,
             "intermediate_dim": 16384,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/opt/opt_presets_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,111 +8,116 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""OPT tokenizer."""
+"""RoBERTa tokenizer."""
 
 import copy
 
-from tensorflow import keras
-
-from keras_nlp.models.opt.opt_presets import backbone_presets
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.tokenizers.byte_pair_tokenizer import BytePairTokenizer
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class OPTTokenizer(BytePairTokenizer):
-    """An OPT tokenizer using Byte-Pair Encoding subword segmentation.
+@keras_nlp_export("keras_nlp.models.RobertaTokenizer")
+class RobertaTokenizer(BytePairTokenizer):
+    """A RoBERTa tokenizer using Byte-Pair Encoding subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.BytePairTokenizer`. Unlike the
-    underlying tokenizer, it will check for all special tokens needed by OPT
+    underlying tokenizer, it will check for all special tokens needed by RoBERTa
     models and provides a `from_preset()` method to automatically download
-    a matching vocabulary for a OPT preset.
+    a matching vocabulary for a RoBERTa preset.
 
-    This tokenizer does not provide truncation or padding of inputs.
+    This tokenizer does not provide truncation or padding of inputs. It can be
+    combined with a `keras_nlp.models.RobertaPreprocessor` layer for input
+    packing.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
+
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
-        vocabulary: string or dict, maps token to integer ids. If it is a
-            string, it should be the file path to a json file.
-        merges: string or list, contains the merge rule. If it is a string,
-            it should be the file path to merge rules. The merge rule file
-            should have one merge rule per line. Every merge rule contains
-            merge entities separated by a space.
+        vocabulary: A dictionary mapping tokens to integer ids, or file path
+            to a json file containing the token to id mapping.
+        merges: A list of merge rules or a string file path, If passing a file
+            path. the file should have one merge rule per line. Every merge
+            rule contains merge entities separated by a space.
 
     Examples:
-
-    Batched inputs.
-    >>> vocab = {"<pad>": 1, "</s>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
-    >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.OPTTokenizer(
-    ...     vocabulary=vocab,
-    ...     merges=merges,
-    ... )
-    >>> tokenizer(["a quick fox", "a fox quick"])
-    <tf.RaggedTensor [[3, 4, 5], [3, 5, 4]]>
-
-    Unbatched input.
-    >>> vocab = {"<pad>": 1, "</s>": 2, "a": 3, "Ġquick": 4, "Ġfox": 5}
-    >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.OPTTokenizer(
-    ...     vocabulary=vocab,
-    ...     merges=merges,
-    ... )
-    >>> tokenizer("a quick fox")
-    <tf.Tensor: shape=(4,), dtype=int32, numpy=array([3, 4, 5], dtype=int32)>
-
-    Detokenization.
-    >>> vocab = {"<pad>": 1, "</s>": 2, "Ġquick": 4, "Ġfox": 5}
-    >>> merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
-    >>> merges += ["Ġ f", "o x", "Ġf ox"]
-    >>> tokenizer = keras_nlp.models.OPTTokenizer(
-    ...     vocabulary=vocab,
-    ...     merges=merges,
-    ... )
-    >>> tokenizer.detokenize(tokenizer(" quick fox")).numpy().decode('utf-8')
-    ' quick fox'
+    ```python
+    # Unbatched input.
+    tokenizer = keras_nlp.models.RobertaTokenizer.from_preset(
+        "roberta_base_en",
+    )
+    tokenizer("The quick brown fox jumped.")
+
+    # Batched input.
+    tokenizer(["The quick brown fox jumped.", "The fox slept."])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    # Note: 'Ġ' is space
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.RobertaTokenizer(
+        vocabulary=vocab,
+        merges=merges
+    )
+    tokenizer(["a quick fox", "a fox quick"])
+    ```
     """
 
     def __init__(
         self,
         vocabulary,
         merges,
         **kwargs,
     ):
+        # Special tokens.
+        start_token = "<s>"
+        pad_token = "<pad>"
+        end_token = "</s>"
+        mask_token = "<mask>"
+
         super().__init__(
             vocabulary=vocabulary,
             merges=merges,
+            unsplittable_tokens=[start_token, pad_token, end_token, mask_token],
             **kwargs,
         )
 
-        # We use `"</s>"` as both a start and end token, as OPT was only
-        # pre-trained with `"</s>"` marking document boundaries.
-        start_token = "</s>"
-        pad_token = "<pad>"
-        end_token = "</s>"
-        for token in [start_token, pad_token, end_token]:
+        # Check whether special tokens are present in the vocabulary.
+        for token in [start_token, pad_token, end_token, mask_token]:
             if token not in self.get_vocabulary():
                 raise ValueError(
                     f"Cannot find token `'{token}'` in the provided "
                     f"`vocabulary`. Please provide `'{token}'` in your "
                     "`vocabulary` or use a pretrained `vocabulary` name."
                 )
 
         self.start_token_id = self.token_to_id(start_token)
         self.pad_token_id = self.token_to_id(pad_token)
         self.end_token_id = self.token_to_id(end_token)
+        self.mask_token_id = self.token_to_id(mask_token)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
+
+    def get_config(self):
+        config = super().get_config()
+        # In the constructor, we pass the list of special tokens to the
+        # `unsplittable_tokens` arg of the superclass' constructor. Hence, we
+        # delete it from the config here.
+        del config["unsplittable_tokens"]
+        return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/opt/opt_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/gpt2/gpt2_tokenizer_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,84 +8,116 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for OPT tokenizer layer."""
+"""Tests for GPT-2 preprocessing layers."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.opt.opt_tokenizer import OPTTokenizer
+from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
 
 
-class OPTTokenizerTest(tf.test.TestCase, parameterized.TestCase):
+class GPT2TokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         self.vocab = {
-            "<s>": 0,
-            "<pad>": 1,
-            "</s>": 2,
-            "Ġair": 3,
-            "plane": 4,
-            "Ġat": 5,
-            "port": 6,
-            "Ġkoh": 7,
-            "li": 8,
-            "Ġis": 9,
-            "Ġthe": 10,
-            "Ġbest": 11,
+            "<|endoftext|>": 0,
+            "Ġair": 1,
+            "plane": 2,
+            "Ġat": 3,
+            "port": 4,
+            "Ġkoh": 5,
+            "li": 6,
+            "Ġis": 7,
+            "Ġthe": 8,
+            "Ġbest": 9,
         }
+        self.merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
+        self.merges += [
+            "Ġa t",
+            "p o",
+            "r t",
+            "o h",
+            "l i",
+            "Ġi s",
+            "Ġb e",
+            "s t",
+        ]
+        self.merges += [
+            "Ġt h",
+            "Ġai r",
+            "pl a",
+            "Ġk oh",
+            "Ġth e",
+            "Ġbe st",
+            "po rt",
+        ]
+        self.merges += ["pla ne"]
 
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["pla ne"]
-        self.merges = merges
-
-        self.tokenizer = OPTTokenizer(vocabulary=self.vocab, merges=self.merges)
+        self.tokenizer = GPT2Tokenizer(
+            vocabulary=self.vocab, merges=self.merges
+        )
 
     def test_tokenize(self):
         input_data = " airplane at airport"
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [3, 4, 5, 3, 6])
+        self.assertAllEqual(output, [1, 2, 3, 1, 4])
+
+    def test_tokenize_end_token(self):
+        input_data = " airplane at airport<|endoftext|>"
+        output = self.tokenizer(input_data)
+        self.assertAllEqual(output, [1, 2, 3, 1, 4, 0])
 
     def test_tokenize_batch(self):
         input_data = tf.constant([" airplane at airport", " kohli is the best"])
         output = self.tokenizer(input_data)
-        self.assertAllEqual(output, [[3, 4, 5, 3, 6], [7, 8, 9, 10, 11]])
+        self.assertAllEqual(output, [[1, 2, 3, 1, 4], [5, 6, 7, 8, 9]])
 
     def test_detokenize(self):
-        input_tokens = [3, 4, 5, 3, 6]
+        input_tokens = [1, 2, 3, 1, 4]
         output = self.tokenizer.detokenize(input_tokens)
         self.assertEqual(output, " airplane at airport")
 
     def test_vocabulary_size(self):
-        self.assertEqual(self.tokenizer.vocabulary_size(), 12)
+        self.assertEqual(self.tokenizer.vocabulary_size(), 10)
 
     def test_errors_missing_special_tokens(self):
         with self.assertRaises(ValueError):
-            OPTTokenizer(vocabulary=["a", "b", "c"], merges=[])
+            GPT2Tokenizer(vocabulary=["a", "b", "c"], merges=[])
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 from keras_nlp.utils.python_utils import format_docstring
 
 
 @keras.utils.register_keras_serializable(package="keras_nlp")
 class Preprocessor(keras.layers.Layer):
     """Base class for model preprocessors."""
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._tokenizer = None
+
     @property
     def tokenizer(self):
         """The tokenizer used to tokenize strings."""
         return self._tokenizer
 
     @tokenizer.setter
     def tokenizer(self, value):
@@ -59,26 +63,18 @@
         """Instantiate {{preprocessor_name}} from preset architecture.
 
         Args:
             preset: string. Must be one of "{{preset_names}}".
 
         Examples:
         ```python
-        # Load preprocessor from preset
-        preprocessor = keras_nlp.models.{{preprocessor_name}}.from_preset(
-            "{{example_preset_name}}",
-        )
-        preprocessor("The quick brown fox jumped.")
-
-        # Override sequence_length
+        # Load a preprocessor layer from a preset.
         preprocessor = keras_nlp.models.{{preprocessor_name}}.from_preset(
             "{{example_preset_name}}",
-            sequence_length=64
         )
-        preprocessor("The quick brown fox jumped.")
         ```
         """
         if not cls.presets:
             raise NotImplementedError(
                 "No presets have been created for this class."
             )
         if preset not in cls.presets:
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_backbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,37 +15,40 @@
 """RoBERTa backbone model."""
 
 import copy
 
 import tensorflow as tf
 from tensorflow import keras
 
-from keras_nlp.layers import TokenAndPositionEmbedding
-from keras_nlp.layers import TransformerEncoder
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.token_and_position_embedding import (
+    TokenAndPositionEmbedding,
+)
+from keras_nlp.layers.transformer_encoder import TransformerEncoder
 from keras_nlp.models.backbone import Backbone
 from keras_nlp.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
 def roberta_kernel_initializer(stddev=0.02):
     return keras.initializers.TruncatedNormal(stddev=stddev)
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.RobertBackbone")
 class RobertaBackbone(Backbone):
-    """RoBERTa encoder.
+    """A RoBERTa encoder network.
 
     This network implements a bi-directional Transformer-based encoder as
     described in ["RoBERTa: A Robustly Optimized BERT Pretraining Approach"](https://arxiv.org/abs/1907.11692).
     It includes the embedding lookups and transformer layers, but does not
-    include the masked language modeling head used during pretraining.
+    include the masked language model head used during pretraining.
 
     The default constructor gives a fully customizable, randomly initialized
     RoBERTa encoder with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset`
+    dimensions. To load preset architectures and weights, use the `from_preset()`
     constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
@@ -56,38 +59,39 @@
             The hidden size must be divisible by the number of attention heads.
         hidden_dim: int. The size of the transformer encoding layer.
         intermediate_dim: int. The output dimension of the first Dense layer in
             a two-layer feedforward network for each transformer.
         dropout: float. Dropout probability for the Transformer encoder.
         max_sequence_length: int. The maximum sequence length this encoder can
             consume. The sequence length of the input must be less than
-            `max_sequence_length`.
+            `max_sequence_length` default value. This determines the variable
+            shape for positional embeddings.
 
-    Example usage:
+    Examples:
     ```python
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
     }
 
     # Pretrained RoBERTa encoder
     model = keras_nlp.models.RobertaBackbone.from_preset("roberta_base_en")
-    output = model(input_data)
+    model(input_data)
 
     # Randomly initialized RoBERTa model with custom config
     model = keras_nlp.models.RobertaBackbone(
         vocabulary_size=50265,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
     )
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     def __init__(
         self,
         vocabulary_size,
         num_layers,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_backbone_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_backbone_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,95 +7,109 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""Test for RoBERTa backbone models."""
+"""Test for FNet backbone model."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
 
 
-class RobertaTest(tf.test.TestCase, parameterized.TestCase):
+class FNetBackboneTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.model = RobertaBackbone(
-            vocabulary_size=1000,
+        self.backbone = FNetBackbone(
+            vocabulary_size=10,
             num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=5,
+            num_segments=4,
         )
-        self.batch_size = 8
         self.input_batch = {
-            "token_ids": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
-            "padding_mask": tf.ones(
-                (self.batch_size, self.model.max_sequence_length), dtype="int32"
-            ),
+            "token_ids": tf.ones((2, 5), dtype="int32"),
+            "segment_ids": tf.ones((2, 5), dtype="int32"),
         }
 
         self.input_dataset = tf.data.Dataset.from_tensor_slices(
             self.input_batch
         ).batch(2)
 
-    def test_valid_call_roberta(self):
-        self.model(self.input_batch)
+    def test_valid_call_f_net(self):
+        self.backbone(self.input_batch)
 
         # Check default name passed through
-        self.assertRegexpMatches(self.model.name, "roberta_backbone")
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_compile(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_batch)
+        self.assertRegexpMatches(self.backbone.name, "f_net_backbone")
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_compile_batched_ds(self, jit_compile):
-        self.model.compile(jit_compile=jit_compile)
-        self.model.predict(self.input_dataset)
-
-    def test_variable_sequence_length_call_roberta(self):
-        for seq_length in (25, 50, 75):
+    def test_variable_sequence_length_call_f_net(self):
+        for seq_length in (2, 3, 4):
             input_data = {
-                "token_ids": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
-                "padding_mask": tf.ones(
-                    (self.batch_size, seq_length), dtype="int32"
-                ),
+                "token_ids": tf.ones((2, seq_length), dtype="int32"),
+                "segment_ids": tf.ones((2, seq_length), dtype="int32"),
             }
-            output = self.model(input_data)
-            self.assertAllEqual(
-                tf.shape(output),
-                [self.batch_size, seq_length, self.model.hidden_dim],
-            )
+            self.backbone(input_data)
+
+    def test_predict(self):
+        self.backbone.predict(self.input_batch)
+        self.backbone.predict(self.input_dataset)
+
+    def test_serialization(self):
+        new_backbone = keras.utils.deserialize_keras_object(
+            keras.utils.serialize_keras_object(self.backbone)
+        )
+        self.assertEqual(new_backbone.get_config(), self.backbone.get_config())
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        model_output = self.model(self.input_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.model.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.backbone(self.input_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.backbone.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, RobertaBackbone)
+        self.assertIsInstance(restored_model, FNetBackbone)
 
         # Check that output matches.
         restored_output = restored_model(self.input_batch)
-        self.assertAllClose(model_output, restored_output)
+        self.assertAllClose(
+            model_output["pooled_output"], restored_output["pooled_output"]
+        )
+
+
+@pytest.mark.tpu
+@pytest.mark.usefixtures("tpu_test_class")
+class FNetBackboneTPUTest(tf.test.TestCase, parameterized.TestCase):
+    def setUp(self):
+        with self.tpu_strategy.scope():
+            self.backbone = FNetBackbone(
+                vocabulary_size=100,
+                num_layers=2,
+                hidden_dim=16,
+                intermediate_dim=32,
+                max_sequence_length=128,
+                num_segments=4,
+            )
+        self.input_batch = {
+            "token_ids": tf.ones((8, 128), dtype="int32"),
+            "segment_ids": tf.ones((8, 128), dtype="int32"),
+        }
+        self.input_dataset = tf.data.Dataset.from_tensor_slices(
+            self.input_batch
+        ).batch(2)
+
+    def test_predict(self):
+        self.backbone.compile()
+        self.backbone.predict(self.input_dataset)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_classifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,205 +13,193 @@
 # limitations under the License.
 """RoBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
 from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.models.task import Task
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.RobertaClassifier")
 class RobertaClassifier(Task):
     """An end-to-end RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
-    `keras_nlp.model.RobertaBackbone`, mapping from the backbone outputs to
-    logit output suitable for a classification task. For usage of this model
-    with pre-trained weights, see the `from_preset()` method.
+    `keras_nlp.model.RobertaBackbone` instance, mapping from the backbone
+    outputs to logits suitable for a classification task. For usage of this
+    model with pre-trained weights, see the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
     Args:
         backbone: A `keras_nlp.models.RobertaBackbone` instance.
         num_classes: int. Number of classes to predict.
+        preprocessor: A `keras_nlp.models.RobertaPreprocessor` or `None`. If
+            `None`, this model will not apply preprocessing, and inputs should
+            be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
         hidden_dim: int. The size of the pooler layer.
         dropout: float. The dropout probability value, applied to the pooled
             output, and after the first dense layer.
-        preprocessor: A `keras_nlp.models.BertPreprocessor` or `None`. If
-            `None`, this model will not apply preprocessing, and inputs should
-            be preprocessed before calling the model.
 
     Examples:
 
-    Example usage.
+    Raw string data.
     ```python
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
-        ),
-    }
-    labels = [0, 3]
-
-    # Randomly initialize a RoBERTa encoder
-    backbone = keras_nlp.models.RobertaBackbone(
-        vocabulary_size=50265,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
-    )
-    # Create a RoBERTa classifier and fit the data.
-    classifier = keras_nlp.models.RobertaClassifier(
-        backbone,
-        4,
-        preprocessor=None,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-    ```
-
-    Raw string inputs.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
     labels = [0, 3]
 
-    # Create a RobertaClassifier and fit your data.
+    # Pretrained classifier.
     classifier = keras_nlp.models.RobertaClassifier.from_preset(
         "roberta_base_en",
         num_classes=4,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
     classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Raw string inputs with customized preprocessing.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
-
-    # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.RobertaPreprocessor.from_preset(
-        "roberta_base_en",
-        sequence_length=128,
-    )
+    classifier.predict(x=features, batch_size=2)
 
-    # Create a RobertaClassifier and fit your data.
-    classifier = keras_nlp.models.RobertaClassifier.from_preset(
-        "roberta_base_en",
-        num_classes=4,
-        preprocessor=preprocessor,
-    )
+    # Re-compile (e.g., with a new learning rate).
     classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
     }
     labels = [0, 3]
 
-    # Create a RoBERTa classifier and fit your data.
+    # Pretrained classifier without preprocessing.
     classifier = keras_nlp.models.RobertaClassifier.from_preset(
         "roberta_base_en",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["a quick fox", "a fox quick"]
+    labels = [0, 3]
+
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick"]
+    merges += ["Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.RobertaTokenizer(
+        vocabulary=vocab,
+        merges=merges
+    )
+    preprocessor = keras_nlp.models.RobertaPreprocessor(
+        tokenizer=tokenizer,
+        sequence_length=128,
+    )
+    backbone = keras_nlp.models.RobertaBackbone(
+        vocabulary_size=20,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128
     )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    classifier = keras_nlp.models.RobertaClassifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
+    )
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
+        num_classes,
+        preprocessor=None,
+        activation=None,
         hidden_dim=None,
         dropout=0.0,
-        preprocessor=None,
         **kwargs,
     ):
         inputs = backbone.input
-        if hidden_dim is None:
-            hidden_dim = backbone.hidden_dim
+        hidden_dim = hidden_dim or backbone.hidden_dim
 
         x = backbone(inputs)[:, backbone.start_token_index, :]
         x = keras.layers.Dropout(dropout, name="pooled_dropout")(x)
         x = keras.layers.Dense(
             hidden_dim, activation="tanh", name="pooled_dense"
         )(x)
         x = keras.layers.Dropout(dropout, name="classifier_dropout")(x)
         outputs = keras.layers.Dense(
             num_classes,
             kernel_initializer=roberta_kernel_initializer(),
+            activation=activation,
             name="logits",
         )(x)
 
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
         # Default compilation
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(2e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
     @classproperty
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""RoBERTa masked lm model."""
+"""XLM-RoBERTa masked lm model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.masked_lm_head import MaskedLMHead
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
 from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
-    RobertaMaskedLMPreprocessor,
-)
-from keras_nlp.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.models.task import Task
+from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
+from keras_nlp.models.xlm_roberta.xlm_roberta_masked_lm_preprocessor import (
+    XLMRobertaMaskedLMPreprocessor,
+)
+from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
+from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class RobertaMaskedLM(Task):
-    """An end-to-end RoBERTa model for the masked language modeling task.
+@keras_nlp_export("keras_nlp.models.XLMRobertaMaskedLM")
+class XLMRobertaMaskedLM(Task):
+    """An end-to-end XLM-RoBERTa model for the masked language modeling task.
 
-    This model will train RoBERTa on a masked language modeling task.
+    This model will train XLM-RoBERTa on a masked language modeling task.
     The model will predict labels for a number of masked tokens in the
     input data. For usage of this model with pre-trained weights, see the
     `from_preset()` method.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case inputs can be raw string features during `fit()`, `predict()`,
     and `evaluate()`. Inputs will be tokenized and dynamically masked during
@@ -45,70 +47,67 @@
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
     Args:
-        backbone: A `keras_nlp.models.RobertaBackbone` instance.
-        preprocessor: A `keras_nlp.models.RobertaMaskedLMPreprocessor` or
+        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
+        preprocessor: A `keras_nlp.models.XLMRobertaMaskedLMPreprocessor` or
             `None`. If `None`, this model will not apply preprocessing, and
             inputs should be preprocessed before calling the model.
 
     Example usage:
 
     Raw string inputs and pretrained backbone.
     ```python
     # Create a dataset with raw string features. Labels are inferred.
     features = ["The quick brown fox jumped.", "I forgot my homework."]
 
-    # Create a RobertaMaskedLM with a pretrained backbone and further train
+    # Pretrained language model
     # on an MLM task.
-    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
-        "roberta_base_en",
+    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
+        "xlm_roberta_base_multi",
     )
+    masked_lm.fit(x=features, batch_size=2)
+    ```
+
+    # Re-compile (e.g., with a new learning rate).
     masked_lm.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programatically (e.g., to change `trainable`).
+    masked_lm.backbone.trainable = False
+    # Fit again.
     masked_lm.fit(x=features, batch_size=2)
     ```
 
-    Preprocessed inputs and custom backbone.
+    Preprocessed integer data.
     ```python
     # Create a preprocessed dataset where 0 is the mask token.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.constant(
             [[1, 2, 0, 4, 0, 6, 7, 8]] * 2, shape=(2, 8)
         ),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1]] * 2, shape=(2, 8)
         ),
         "mask_positions": tf.constant([[2, 4]] * 2, shape=(2, 2))
     }
     # Labels are the original masked values.
     labels = [[3, 5]] * 2
 
-    # Randomly initialize a RoBERTa encoder
-    backbone = keras_nlp.models.RobertaBackbone(
-        vocabulary_size=50265,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
-    )
-    # Create a RoBERTa masked_lm and fit the data.
-    masked_lm = keras_nlp.models.RobertaMaskedLM(
-        backbone,
+    masked_lm = keras_nlp.models.XLMRobertaMaskedLM.from_preset(
+        "xlm_roberta_base_multi",
         preprocessor=None,
     )
-    masked_lm.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    masked_lm.fit(x=preprocessed_features, y=labels, batch_size=2)
+
+    masked_lm.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
         preprocessor=None,
@@ -125,29 +124,36 @@
             vocabulary_size=backbone.vocabulary_size,
             embedding_weights=backbone.token_embedding.embeddings,
             intermediate_activation="gelu",
             kernel_initializer=roberta_kernel_initializer(),
             name="mlm_head",
         )(backbone_outputs, inputs["mask_positions"])
 
-        # Instantiate using Functional API Model constructor
+        # Instantiate using Functional API Model constructor.
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
 
+        self.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            optimizer=keras.optimizers.Adam(5e-5),
+            weighted_metrics=keras.metrics.SparseCategoricalAccuracy(),
+            jit_compile=is_xla_compatible(self),
+        )
+
     @classproperty
     def backbone_cls(cls):
-        return RobertaBackbone
+        return XLMRobertaBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return RobertaMaskedLMPreprocessor
+        return XLMRobertaMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,49 @@
-# Copyright 2022 The KerasNLP Authors
+# Copyright 2023 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""RoBERTa masked language model preprocessor layer."""
-
 from absl import logging
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
-from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
+from keras_nlp.models.f_net.f_net_preprocessor import FNetPreprocessor
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class RobertaMaskedLMPreprocessor(RobertaPreprocessor):
-    """RoBERTa preprocessing for the masked language modeling task.
+@keras_nlp_export("keras_nlp.models.FNetMaskedLMPreprocessor")
+class FNetMaskedLMPreprocessor(FNetPreprocessor):
+    """FNet preprocessing for the masked language modeling task.
 
     This preprocessing layer will prepare inputs for a masked language modeling
     task. It is primarily intended for use with the
-    `keras_nlp.models.RobertaMaskedLM` task model. Preprocessing will occur in
+    `keras_nlp.models.FNetMaskedLM` task model. Preprocessing will occur in
     multiple steps.
 
-    - Tokenize any number of input segments using the `tokenizer`.
-    - Pack the inputs together with the appropriate `"<s>"`, `"</s>"` and
+    1. Tokenize any number of input segments using the `tokenizer`.
+    2. Pack the inputs together with the appropriate `"<s>"`, `"</s>"` and
       `"<pad>"` tokens, i.e., adding a single `"<s>"` at the start of the
       entire sequence, `"</s></s>"` between each segment,
       and a `"</s>"` at the end of the entire sequence.
-    - Randomly select non-special tokens to mask, controlled by
+    3. Randomly select non-special tokens to mask, controlled by
       `mask_selection_rate`.
-    - Construct a `(x, y, sample_weight)` tuple suitable for training with a
-      `keras_nlp.models.RobertaMaskedLM` task model.
+    4. Construct a `(x, y, sample_weight)` tuple suitable for training with a
+      `keras_nlp.models.FNetMaskedLM` task model.
 
     Args:
-        tokenizer: A `keras_nlp.models.RobertaTokenizer` instance.
+        tokenizer: A `keras_nlp.models.FNetTokenizer` instance.
         sequence_length: The length of the packed inputs.
         mask_selection_rate: The probability an input token will be dynamically
             masked.
         mask_selection_length: The maximum number of masked tokens supported
             by the layer.
         mask_token_rate: float, defaults to 0.8. `mask_token_rate` must be
             between 0 and 1 which indicates how often the mask_token is
@@ -65,51 +62,61 @@
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
     Examples:
+
+    Directly calling the layer on data.
     ```python
     # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.RobertaMaskedLMPreprocessor.from_preset(
-        "roberta_base_en"
+    preprocessor = keras_nlp.models.FNetMaskedLMPreprocessor.from_preset(
+        "f_net_base_en"
     )
 
     # Tokenize and mask a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
+    preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and mask a batch of sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
+    # Tokenize and mask a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
+
+    # Tokenize and mask sentence pairs.
+    # In this case, always convert input to tensors before calling the layer.
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+    ```
 
-    # Tokenize and mask a dataset of sentences.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.FNetMaskedLMPreprocessor.from_preset(
+        "f_net_base_en"
     )
-    ds = tf.data.Dataset.from_tensor_slices((features))
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+
+    # Map single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
     # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as above.
-    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick", "Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.RobertaTokenizer(
-        vocabulary=vocab,
-        merges=merges,
+    vocab_data = tf.data.Dataset.from_tensor_slices(
+        ["the quick brown fox", "the earth is round"]
     )
-    preprocessor = keras_nlp.models.RobertaMaskedLMPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=8,
+
+    # Map sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
+    # Watch out for tf.data's default unpacking of tuples here!
+    # Best to invoke the `preprocessor` directly in this case.
+    ds = ds.map(
+        lambda first, second: preprocessor(x=(first, second)),
+        num_parallel_calls=tf.data.AUTOTUNE,
     )
-    preprocessor("a quick fox")
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
@@ -131,16 +138,16 @@
             mask_selection_rate=mask_selection_rate,
             mask_selection_length=mask_selection_length,
             mask_token_rate=mask_token_rate,
             random_token_rate=random_token_rate,
             vocabulary_size=tokenizer.vocabulary_size(),
             mask_token_id=tokenizer.mask_token_id,
             unselectable_token_ids=[
-                tokenizer.start_token_id,
-                tokenizer.end_token_id,
+                tokenizer.cls_token_id,
+                tokenizer.sep_token_id,
                 tokenizer.pad_token_id,
             ],
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
@@ -157,19 +164,21 @@
         if y is not None or sample_weight is not None:
             logging.warning(
                 f"{self.__class__.__name__} generates `y` and `sample_weight` "
                 "based on your input data, but your data already contains `y` "
                 "or `sample_weight`. Your `y` and `sample_weight` will be "
                 "ignored."
             )
-
         x = super().call(x)
-        token_ids, padding_mask = x["token_ids"], x["padding_mask"]
+        token_ids, segment_ids = (
+            x["token_ids"],
+            x["segment_ids"],
+        )
         masker_outputs = self.masker(token_ids)
         x = {
             "token_ids": masker_outputs["token_ids"],
-            "padding_mask": padding_mask,
+            "segment_ids": segment_ids,
             "mask_positions": masker_outputs["mask_positions"],
         }
         y = masker_outputs["mask_ids"]
         sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm_preprocessor_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for RoBERTa masked language model preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
     RobertaMaskedLMPreprocessor,
 )
@@ -136,25 +137,36 @@
         self.assertAllEqual(
             x["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(x["mask_positions"], [0, 0, 0, 0, 0])
         self.assertAllEqual(y, [0, 0, 0, 0, 0])
         self.assertAllEqual(sw, [0.0, 0.0, 0.0, 0.0, 0.0])
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         outputs = model(input_data)[0]["token_ids"]
         restored_outputs = restored_model(input_data)[0]["token_ids"]
         self.assertAllEqual(outputs, restored_outputs)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_masked_lm_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,135 +7,126 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for RoBERTa masked language model."""
+"""Tests for DeBERTa masked language model."""
 
+import io
 import os
 
+import pytest
+import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
-from keras_nlp.models.roberta.roberta_masked_lm import RobertaMaskedLM
-from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
-    RobertaMaskedLMPreprocessor,
+from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
+from keras_nlp.models.deberta_v3.deberta_v3_masked_lm import DebertaV3MaskedLM
+from keras_nlp.models.deberta_v3.deberta_v3_masked_lm_preprocessor import (
+    DebertaV3MaskedLMPreprocessor,
 )
-from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
+from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
 
 
-class RobertaMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
+class DebertaV3MaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
-        self.backbone = RobertaBackbone(
-            vocabulary_size=1000,
+        bytes_io = io.BytesIO()
+        vocab_data = tf.data.Dataset.from_tensor_slices(
+            ["the quick brown fox", "the earth is round", "an eagle flew"]
+        )
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=vocab_data.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=15,
+            model_type="WORD",
+            pad_id=0,
+            bos_id=1,
+            eos_id=2,
+            unk_id=3,
+            pad_piece="[PAD]",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            unk_piece="[UNK]",
+            user_defined_symbols="[MASK]",
+        )
+        proto = bytes_io.getvalue()
+        self.preprocessor = DebertaV3MaskedLMPreprocessor(
+            DebertaV3Tokenizer(proto=proto),
+            mask_selection_length=2,
+            sequence_length=5,
+        )
+        self.backbone = DebertaV3Backbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
             num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
-        )
-        self.vocab = {
-            "<s>": 0,
-            "<pad>": 1,
-            "</s>": 2,
-            "Ġair": 3,
-            "plane": 4,
-            "Ġat": 5,
-            "port": 6,
-            "Ġkoh": 7,
-            "li": 8,
-            "Ġis": 9,
-            "Ġthe": 10,
-            "Ġbest": 11,
-            "<mask>": 12,
-        }
-
-        merges = ["Ġ a", "Ġ t", "Ġ k", "Ġ i", "Ġ b", "Ġa i", "p l", "n e"]
-        merges += ["Ġa t", "p o", "r t", "o h", "l i", "Ġi s", "Ġb e", "s t"]
-        merges += ["Ġt h", "Ġai r", "pl a", "Ġk oh", "Ġth e", "Ġbe st", "po rt"]
-        merges += ["pla ne"]
-        self.merges = merges
-        self.preprocessor = RobertaMaskedLMPreprocessor(
-            RobertaTokenizer(vocabulary=self.vocab, merges=self.merges),
-            sequence_length=8,
-            mask_selection_length=2,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.masked_lm = RobertaMaskedLM(
+        self.masked_lm = DebertaV3MaskedLM(
             self.backbone,
             preprocessor=self.preprocessor,
         )
-        self.masked_lm_no_preprocessing = RobertaMaskedLM(
-            self.backbone,
-            preprocessor=None,
-        )
 
         self.raw_batch = tf.constant(
             [
-                " airplane at airport",
-                " the airplane is the best",
-                " the best airport",
-                " kohli is the best",
+                "the quick brown fox.",
+                "the eagle flew over fox.",
             ]
         )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)[0]
+        self.preprocessed_batch = self.preprocessor(self.raw_batch)
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
             self.raw_batch
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
-    def test_valid_call_masked_lm(self):
-        self.masked_lm(self.preprocessed_batch)
+    def test_valid_call_classifier(self):
+        self.masked_lm(self.preprocessed_batch[0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_masked_lm_predict(self, jit_compile):
-        self.masked_lm.compile(jit_compile=jit_compile)
+    def test_classifier_predict(self):
         self.masked_lm.predict(self.raw_batch)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.predict(self.preprocessed_batch[0])
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_masked_lm_predict_no_preprocessing(self, jit_compile):
-        self.masked_lm_no_preprocessing.compile(jit_compile=jit_compile)
-        self.masked_lm_no_preprocessing.predict(self.preprocessed_batch)
+    def test_classifier_fit(self):
+        self.masked_lm.fit(self.raw_dataset)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_masked_lm_fit(self, jit_compile):
+    def test_classifier_fit_no_xla(self):
+        self.masked_lm.preprocessor = None
         self.masked_lm.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
         )
-        self.masked_lm.fit(self.raw_dataset)
+        self.masked_lm.fit(self.preprocessed_dataset)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_roberta_masked_lm_fit_no_preprocessing(self, jit_compile):
-        self.masked_lm_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.masked_lm)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.masked_lm.get_config(),
         )
-        self.masked_lm_no_preprocessing.fit(self.preprocessed_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.masked_lm.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+        model_output = self.masked_lm.predict(self.raw_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.masked_lm.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, RobertaMaskedLM)
-
-        model_output = self.masked_lm(self.preprocessed_batch)
-        restored_output = restored_model(self.preprocessed_batch)
+        self.assertIsInstance(restored_model, DebertaV3MaskedLM)
 
-        self.assertAllClose(model_output, restored_output)
+        # Check that output matches.
+        restored_output = restored_model.predict(self.raw_batch)
+        self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_multi_segment_packer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
 # TODO: This is a temporary, unexported layer until we find a way to make the
 # `MultiSegmentPacker` layer more generic.
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.RobertaMultiSegmentPacker")
 class RobertaMultiSegmentPacker(keras.layers.Layer):
     """Packs multiple sequences into a single fixed width model input.
 
     This layer packs multiple input sequences into a single fixed width sequence
     containing start and end delimiters, forming a dense input suitable for a
     classification task for RoBERTa.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,144 +12,130 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """RoBERTa preprocessor layer."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.preprocessor import Preprocessor
 from keras_nlp.models.roberta.roberta_multi_segment_packer import (
     RobertaMultiSegmentPacker,
 )
 from keras_nlp.models.roberta.roberta_presets import backbone_presets
 from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 from keras_nlp.utils.keras_utils import (
     convert_inputs_to_list_of_tensor_segments,
 )
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.RobertaPreprocessor")
 class RobertaPreprocessor(Preprocessor):
-    """RoBERTa preprocessing layer which tokenizes and packs inputs.
+    """A RoBERTa preprocessing layer which tokenizes and packs inputs.
 
     This preprocessing layer will do three things:
 
-    - Tokenize any number of input segments using the `tokenizer`.
-    - Pack the inputs together with the appropriate `"<s>"`, `"</s>"` and
-      `"<pad>"` tokens, i.e., adding a single `"<s>"` at the start of the
-      entire sequence, `"</s></s>"` at the end of each segment, save the last
-      and a `"</s>"` at the end of the entire sequence.
-    - Construct a dictionary with keys `"token_ids"`, `"segment_ids"`,
-       `"padding_mask"`, that can be passed directly to a RoBERTa model.
+    1. Tokenize any number of input segments using the `tokenizer`.
+    2. Pack the inputs together with the appropriate `"<s>"`, `"</s>"` and
+       `"<pad>"` tokens, i.e., adding a single `"<s>"` at the start of the
+       entire sequence, `"</s></s>"` at the end of each segment, save the last
+       and a `"</s>"` at the end of the entire sequence.
+    3. Construct a dictionary with keys `"token_ids"`, `"padding_mask"` that
+       can be passed directly to a RoBERTa model.
 
     This layer can be used directly with `tf.data.Dataset.map` to preprocess
     string data in the `(x, y, sample_weight)` format used by
     `keras.Model.fit`.
 
-    The call method of this layer accepts three arguments, `x`, `y`, and
-    `sample_weight`. `x` can be a python string or tensor representing a single
-    segment, a list of python strings representing a batch of single segments,
-    or a list of tensors representing multiple segments to be packed together.
-    `y` and `sample_weight` are both optional, can have any format, and will be
-    passed through unaltered.
-
-    Special care should be taken when using `tf.data` to map over an unlabeled
-    tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
-    directly into the call arguments of this layer, rather than forward all
-    argument to `x`. To handle this case, it is recommended to  explicitly call
-    the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
-
     Args:
         tokenizer: A `keras_nlp.models.RobertaTokenizer` instance.
         sequence_length: The length of the packed inputs.
         truncate: string. The algorithm to truncate a list of batched segments
             to fit within `sequence_length`. The value can be either
             `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
 
+    Call arguments:
+        x: A tensor of single string sequences, or a tuple of multiple
+            tensor sequences to be packed together. Inputs may be batched or
+            unbatched. For single sequences, raw python inputs will be converted
+            to tensors. For multiple sequences, pass tensors directly.
+        y: Any label data. Will be passed through unaltered.
+        sample_weight: Any label weight data. Will be passed through unaltered.
+
+
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
     preprocessor = keras_nlp.models.RobertaPreprocessor.from_preset(
-        "roberta_base_en",
+        "roberta_base_en"
     )
 
     # Tokenize and pack a single sentence.
-    sentence = tf.constant(" afternoon sun")
-    preprocessor(sentence)
-    # Same output.
-    preprocessor(" afternoon sun")
-
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        [" afternoon sun", " night moon"]
+    preprocessor("The quick brown fox jumped.")
+
+    # Tokenize a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
+
+    # Preprocess a batch of sentence pairs.
+    # When handling multiple sequences, always convert to tensors first!
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+
+    # Custom vocabulary.
+    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
+    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
+    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick", "Ġ f", "o x", "Ġf ox"]
+    tokenizer = keras_nlp.models.RobertaTokenizer(
+        vocabulary=vocab,
+        merges=merges
     )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        [" afternoon sun", " night moon"]
+    preprocessor = keras_nlp.models.RobertaPreprocessor(tokenizer)
+    preprocessor("a quick fox")
+    ```
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.RobertaPreprocessor.from_preset(
+        "roberta_base_en"
     )
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant(" afternoon sun")
-    second_sentence = tf.constant("refulgent sun")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        [" afternoon sun", " night moon"]
-    )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    label = tf.constant([1, 1])
+
+    # Map labeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices((first, label))
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant([" afternoon sun", " night moon"])
-    second_sentences = tf.constant(["refulgent sun", " bright moon"])
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
-    )
+    # Map unlabeled single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map labeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices(((first, second), label))
+    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+
+    # Map unlabeled sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
-
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as above.
-    vocab = {"<s>": 0, "<pad>": 1, "</s>": 2, "<mask>": 3}
-    vocab = {**vocab, "a": 4, "Ġquick": 5, "Ġfox": 6}
-    merges = ["Ġ q", "u i", "c k", "ui ck", "Ġq uick", "Ġ f", "o x", "Ġf ox"]
-    tokenizer = keras_nlp.models.RobertaTokenizer(
-        vocabulary=vocab,
-        merges=merges,
-    )
-    preprocessor = keras_nlp.models.RobertaPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=8,
-    )
-    preprocessor("a quick fox")
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_preprocessor_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for RoBERTa preprocessor layer."""
 
 import os
 
+import pytest
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.roberta.roberta_preprocessor import RobertaPreprocessor
 from keras_nlp.models.roberta.roberta_tokenizer import RobertaTokenizer
 
@@ -135,26 +136,37 @@
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant([" airplane at airport"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             "description": (
                 "12-layer RoBERTa model where case is maintained."
                 "Trained on English Wikipedia, BooksCorpus, CommonCraw, and OpenWebText."
             ),
             "params": 124052736,
             "official_name": "RoBERTa",
             "path": "roberta",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/roberta/README.md",
         },
         "config": {
             "vocabulary_size": 50265,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -46,14 +47,15 @@
             "description": (
                 "24-layer RoBERTa model where case is maintained."
                 "Trained on English Wikipedia, BooksCorpus, CommonCraw, and OpenWebText."
             ),
             "params": 354307072,
             "official_name": "RoBERTa",
             "path": "roberta",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/roberta/README.md",
         },
         "config": {
             "vocabulary_size": 50265,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/roberta/roberta_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_presets_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,29 +69,30 @@
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = ["Let's rock!"]
         model = RobertaClassifier.from_preset(
-            "roberta_base_en", load_weights=load_weights
+            "roberta_base_en", num_classes=2, load_weights=load_weights
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_classifier_output_without_preprocessing(self, load_weights):
         input_data = {
             "token_ids": tf.constant([[101, 1996, 4248, 102]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = RobertaClassifier.from_preset(
             "roberta_base_en",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
@@ -131,24 +132,24 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("roberta_tokenizer", RobertaTokenizer),
-        ("roberta_preprocessor", RobertaPreprocessor),
-        ("roberta", RobertaBackbone),
-        ("roberta_classifier", RobertaClassifier),
-        ("roberta_masked_lm", RobertaMaskedLM),
+        ("roberta_tokenizer", RobertaTokenizer, {}),
+        ("roberta_preprocessor", RobertaPreprocessor, {}),
+        ("roberta", RobertaBackbone, {}),
+        ("roberta_classifier", RobertaClassifier, {"num_classes": 2}),
+        ("roberta_masked_lm", RobertaMaskedLM, {}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("roberta_base_en_clowntown")
+            cls.from_preset("roberta_base_en_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
 class RobertaPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
 
@@ -187,14 +188,15 @@
     @parameterized.named_parameters(
         ("load_weights", True), ("no_load_weights", False)
     )
     def test_load_roberta_classifier_without_preprocessing(self, load_weights):
         for preset in RobertaClassifier.presets:
             classifier = RobertaClassifier.from_preset(
                 preset,
+                num_classes=2,
                 preprocessor=None,
                 load_weights=load_weights,
             )
             input_data = {
                 "token_ids": tf.random.uniform(
                     shape=(1, 512),
                     dtype=tf.int64,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/task.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/roberta/roberta_masked_lm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,156 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Base class for Task models."""
+"""RoBERTa masked lm model."""
 
-import os
+import copy
 
 from tensorflow import keras
 
-from keras_nlp.utils.pipeline_model import PipelineModel
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.masked_lm_head import MaskedLMHead
+from keras_nlp.models.roberta.roberta_backbone import RobertaBackbone
+from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
+from keras_nlp.models.roberta.roberta_masked_lm_preprocessor import (
+    RobertaMaskedLMPreprocessor,
+)
+from keras_nlp.models.roberta.roberta_presets import backbone_presets
+from keras_nlp.models.task import Task
+from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
-from keras_nlp.utils.python_utils import format_docstring
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class Task(PipelineModel):
-    """Base class for Task models."""
-
-    def preprocess_samples(self, x, y=None, sample_weight=None):
-        return self.preprocessor(x, y=y, sample_weight=sample_weight)
-
-    @property
-    def backbone(self):
-        """A `keras.Model` instance providing the backbone submodel."""
-        return self._backbone
-
-    @backbone.setter
-    def backbone(self, value):
-        self._backbone = value
-
-    @property
-    def preprocessor(self):
-        """A `keras.layers.Layer` instance used to preprocess inputs."""
-        return self._preprocessor
-
-    @preprocessor.setter
-    def preprocessor(self, value):
-        self.include_preprocessing = value is not None
-        self._preprocessor = value
-
-    def get_config(self):
-        # Don't chain to super here. The default `get_config()` for functional
-        # models is nested and cannot be passed to our Task constructors.
-        return {
-            "backbone": keras.layers.serialize(self.backbone),
-            "preprocessor": keras.layers.serialize(self.preprocessor),
-            "name": self.name,
-            "trainable": self.trainable,
+@keras_nlp_export("keras_nlp.models.RobertaMaskedLM")
+class RobertaMaskedLM(Task):
+    """An end-to-end RoBERTa model for the masked language modeling task.
+
+    This model will train RoBERTa on a masked language modeling task.
+    The model will predict labels for a number of masked tokens in the
+    input data. For usage of this model with pre-trained weights, see the
+    `from_preset()` method.
+
+    This model can optionally be configured with a `preprocessor` layer, in
+    which case inputs can be raw string features during `fit()`, `predict()`,
+    and `evaluate()`. Inputs will be tokenized and dynamically masked during
+    training and evaluation. This is done by default when creating the model
+    with `from_preset()`.
+
+    Disclaimer: Pre-trained models are provided on an "as is" basis, without
+    warranties or conditions of any kind. The underlying model is provided by a
+    third party and subject to a separate license, available
+    [here](https://github.com/facebookresearch/fairseq).
+
+    Args:
+        backbone: A `keras_nlp.models.RobertaBackbone` instance.
+        preprocessor: A `keras_nlp.models.RobertaMaskedLMPreprocessor` or
+            `None`. If `None`, this model will not apply preprocessing, and
+            inputs should be preprocessed before calling the model.
+
+    Examples:
+
+    Raw string data.
+    ```python
+    features = ["The quick brown fox jumped.", "I forgot my homework."]
+
+    # Pretrained language model.
+    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
+        "roberta_base_en",
+    )
+    masked_lm.fit(x=features, batch_size=2)
+
+    # Re-compile (e.g., with a new learning rate).
+    masked_lm.compile(
+        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
+    )
+    # Access backbone programatically (e.g., to change `trainable`).
+    masked_lm.backbone.trainable = False
+    # Fit again.
+    masked_lm.fit(x=features, batch_size=2)
+    ```
+
+    Preprocessed integer data.
+    ```python
+    # Create a preprocessed dataset where 0 is the mask token.
+    features = {
+        "token_ids": tf.constant(
+            [[1, 2, 0, 4, 0, 6, 7, 8]] * 2, shape=(2, 8)
+        ),
+        "padding_mask": tf.constant(
+            [[1, 1, 1, 1, 1, 1, 1, 1]] * 2, shape=(2, 8)
+        ),
+        "mask_positions": tf.constant([[2, 4]] * 2, shape=(2, 2))
+    }
+    # Labels are the original masked values.
+    labels = [[3, 5]] * 2
+
+    masked_lm = keras_nlp.models.RobertaMaskedLM.from_preset(
+        "roberta_base_en",
+        preprocessor=None,
+    )
+
+    masked_lm.fit(x=features, y=labels, batch_size=2)
+    ```
+    """
+
+    def __init__(
+        self,
+        backbone,
+        preprocessor=None,
+        **kwargs,
+    ):
+        inputs = {
+            **backbone.input,
+            "mask_positions": keras.Input(
+                shape=(None,), dtype="int32", name="mask_positions"
+            ),
         }
-
-    @classmethod
-    def from_config(cls, config):
-        # The default `from_config()` for functional models will return a
-        # vanilla `keras.Model`. We override it to get a subclass instance back.
-        if "backbone" in config and isinstance(config["backbone"], dict):
-            config["backbone"] = keras.layers.deserialize(config["backbone"])
-        if "preprocessor" in config and isinstance(
-            config["preprocessor"], dict
-        ):
-            config["preprocessor"] = keras.layers.deserialize(
-                config["preprocessor"]
-            )
-        return cls(**config)
+        backbone_outputs = backbone(backbone.input)
+        outputs = MaskedLMHead(
+            vocabulary_size=backbone.vocabulary_size,
+            embedding_weights=backbone.token_embedding.embeddings,
+            intermediate_activation="gelu",
+            kernel_initializer=roberta_kernel_initializer(),
+            name="mlm_head",
+        )(backbone_outputs, inputs["mask_positions"])
+
+        # Instantiate using Functional API Model constructor
+        super().__init__(
+            inputs=inputs,
+            outputs=outputs,
+            include_preprocessing=preprocessor is not None,
+            **kwargs,
+        )
+        # All references to `self` below this line
+        self.backbone = backbone
+        self.preprocessor = preprocessor
+
+        self.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            optimizer=keras.optimizers.Adam(5e-5),
+            weighted_metrics=keras.metrics.SparseCategoricalAccuracy(),
+            jit_compile=is_xla_compatible(self),
+        )
 
     @classproperty
     def backbone_cls(cls):
-        return None
+        return RobertaBackbone
 
     @classproperty
     def preprocessor_cls(cls):
-        return None
+        return RobertaMaskedLMPreprocessor
 
     @classproperty
     def presets(cls):
-        return {}
-
-    @classmethod
-    def from_preset(
-        cls,
-        preset,
-        load_weights=True,
-        **kwargs,
-    ):
-        """Instantiate {{model_task_name}} model from preset architecture and weights.
-
-        Args:
-            preset: string. Must be one of "{{preset_names}}".
-            load_weights: Whether to load pre-trained weights into model.
-                Defaults to `True`.
-
-        Examples:
-        ```python
-        # Load architecture and weights from preset
-        model = {{model_task_name}}.from_preset("{{example_preset_name}}")
-
-        # Load randomly initialized model from preset architecture
-        model = {{model_task_name}}.from_preset(
-            "{{example_preset_name}}",
-            load_weights=False
-        )
-        ```
-        """
-        if not cls.presets:
-            raise NotImplementedError(
-                "No presets have been created for this class."
-            )
-
-        if preset not in cls.presets:
-            raise ValueError(
-                "`preset` must be one of "
-                f"""{", ".join(cls.presets)}. Received: {preset}."""
-            )
-
-        if "preprocessor" not in kwargs:
-            kwargs["preprocessor"] = cls.preprocessor_cls.from_preset(preset)
-
-        # Check if preset is backbone-only model
-        if preset in cls.backbone_cls.presets:
-            backbone = cls.backbone_cls.from_preset(preset, load_weights)
-            return cls(backbone, **kwargs)
-
-        # Otherwise must be one of class presets
-        metadata = cls.presets[preset]
-        config = metadata["config"]
-        model = cls.from_config({**config, **kwargs})
-
-        if not load_weights:
-            return model
-
-        weights = keras.utils.get_file(
-            "model.h5",
-            metadata["weights_url"],
-            cache_subdir=os.path.join("models", preset),
-            file_hash=metadata["weights_hash"],
-        )
-
-        model.load_weights(weights)
-        return model
-
-    def __init_subclass__(cls, **kwargs):
-        # Use __init_subclass__ to setup a correct docstring for from_preset.
-        super().__init_subclass__(**kwargs)
-
-        # If the subclass does not define `from_preset`, assign a wrapper so that
-        # each class can have a distinct docstring.
-        if "from_preset" not in cls.__dict__:
-
-            def from_preset(calling_cls, *args, **kwargs):
-                return super(cls, calling_cls).from_preset(*args, **kwargs)
-
-            cls.from_preset = classmethod(from_preset)
-
-        # Format and assign the docstring unless the subclass has overridden it.
-        if cls.from_preset.__doc__ is None:
-            cls.from_preset.__func__.__doc__ = Task.from_preset.__doc__
-            format_docstring(
-                model_task_name=cls.__name__,
-                example_preset_name=next(iter(cls.presets), ""),
-                preset_names='", "'.join(cls.presets),
-            )(cls.from_preset.__func__)
+        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """XLM-RoBERTa backbone model."""
 
 import copy
 
-from tensorflow import keras
-
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.roberta import roberta_backbone
 from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.XLMRobertaBackbone")
 class XLMRobertaBackbone(roberta_backbone.RobertaBackbone):
-    """XLM-RoBERTa encoder.
+    """An XLM-RoBERTa encoder network.
 
-    This network implements a bi-directional Transformer-based encoder as
-    described in
-    ["Unsupervised Cross-lingual Representation Learning at Scale"](https://arxiv.org/abs/1911.02116).
-    It includes the embedding lookups and transformer layers, but does not
+    This class implements a bi-directional Transformer-based encoder as
+    described in ["Unsupervised Cross-lingual Representation Learning at Scale"](https://arxiv.org/abs/1911.02116).
+    It includes the embedding lookups and transformer layers, but it does not
     include the masked language modeling head used during pretraining.
 
     The default constructor gives a fully customizable, randomly initialized
-    RoBERTa encoder with any number of layers, heads, and embedding
-    dimensions. To load preset architectures and weights, use the `from_preset`
+    RoBERTa encoder with any number of layers, heads, and embedding dimensions.
+    To load preset architectures and weights, use the `from_preset()`
     constructor.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
@@ -50,41 +48,40 @@
             The hidden size must be divisible by the number of attention heads.
         hidden_dim: int. The size of the transformer encoding layer.
         intermediate_dim: int. The output dimension of the first Dense layer in
             a two-layer feedforward network for each transformer.
         dropout: float. Dropout probability for the Transformer encoder.
         max_sequence_length: int. The maximum sequence length this encoder can
             consume. The sequence length of the input must be less than
-            `max_sequence_length`.
+            `max_sequence_length` default value. This determines the variable
+            shape for positional embeddings.
 
-    Example usage:
+    Examples:
     ```python
     input_data = {
         "token_ids": tf.ones(shape=(1, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0], shape=(1, 12)),
     }
 
-    # Pretrained XLM-R encoder
+    # Pretrained XLM-R encoder.
     model = keras_nlp.models.XLMRobertaBackbone.from_preset(
         "xlm_roberta_base_multi",
     )
-    output = model(input_data)
+    model(input_data)
 
-    # Randomly initialized XLM-R model with custom config
+    # Randomly initialized XLM-R model with custom config.
     model = keras_nlp.models.XLMRobertaBackbone(
         vocabulary_size=250002,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128
     )
-
-    # Call the model on the input data.
-    output = model(input_data)
+    model(input_data)
     ```
     """
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,209 +13,208 @@
 # limitations under the License.
 """XLM-RoBERTa classification model."""
 
 import copy
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.roberta.roberta_backbone import roberta_kernel_initializer
 from keras_nlp.models.task import Task
 from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
 from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
     XLMRobertaPreprocessor,
 )
 from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
 from keras_nlp.utils.keras_utils import is_xla_compatible
 from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.XLMRobertaClassifier")
 class XLMRobertaClassifier(Task):
     """An end-to-end XLM-RoBERTa model for classification tasks.
 
     This model attaches a classification head to a
-    `keras_nlp.model.XLMRobertaBackbone` model, mapping from the backbone
-    outputs to logit output suitable for a classification task. For usage of
-    this model with pre-trained weights, see the `from_preset()` method.
+    `keras_nlp.model.XLMRobertaBackbone` instance, mapping from the backbone
+    outputs to logits suitable for a classification task. For usage of
+    this model with pre-trained weights, see the `from_preset()` constructor.
 
     This model can optionally be configured with a `preprocessor` layer, in
     which case it will automatically apply preprocessing to raw inputs during
     `fit()`, `predict()`, and `evaluate()`. This is done by default when
     creating the model with `from_preset()`.
 
     Disclaimer: Pre-trained models are provided on an "as is" basis, without
     warranties or conditions of any kind. The underlying model is provided by a
     third party and subject to a separate license, available
     [here](https://github.com/facebookresearch/fairseq).
 
     Args:
-        backbone: A `keras_nlp.models.XLMRoberta` instance.
+        backbone: A `keras_nlp.models.XLMRobertaBackbone` instance.
         num_classes: int. Number of classes to predict.
-        hidden_dim: int. The size of the pooler layer.
-        dropout: float. The dropout probability value, applied to the pooled
-            output, and after the first dense layer.
         preprocessor: A `keras_nlp.models.XLMRobertaPreprocessor` or `None`. If
             `None`, this model will not apply preprocessing, and inputs should
             be preprocessed before calling the model.
+        activation: Optional `str` or callable, defaults to `None`. The
+            activation function to use on the model outputs. Set
+            `activation="softmax"` to return output probabilities.
+        hidden_dim: int. The size of the pooler layer.
+        dropout: float. The dropout probability value, applied to the pooled
+            output, and after the first dense layer.
 
     Examples:
 
-    Example usage.
+    Raw string data.
     ```python
-    preprocessed_features = {
-        "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
-        "padding_mask": tf.constant(
-            [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)),
-    }
+    features = ["The quick brown fox jumped.", "نسيت الواجب"]
     labels = [0, 3]
 
-    # Randomly initialized XLM-RoBERTa encoder
-    backbone = keras_nlp.models.XLMRobertaBackbone(
-        vocabulary_size=250002,
-        num_layers=12,
-        num_heads=12,
-        hidden_dim=768,
-        intermediate_dim=3072,
-        max_sequence_length=12
-    )
-
-    # Create a XLM-RoBERTa classifier and fit your data.
-    classifier = keras_nlp.models.XLMRobertaClassifier(
-        backbone,
-        num_classes=4,
-        preprocessor=None,
-    )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
-
-    # Access backbone programatically (e.g., to change `trainable`)
-    classifier.backbone.trainable = False
-    ```
-
-    Raw string inputs.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
-
-    # Create a XLMRobertaClassifier and fit your data.
+    # Pretrained classifier.
     classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
         "xlm_roberta_base_multi",
         num_classes=4,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    )
     classifier.fit(x=features, y=labels, batch_size=2)
-    ```
-
-    Raw string inputs with customized preprocessing.
-    ```python
-    # Create a dataset with raw string features in an `(x, y)` format.
-    features = ["The quick brown fox jumped.", "I forgot my homework."]
-    labels = [0, 3]
+    classifier.predict(x=features, batch_size=2)
 
-    # Use a shorter sequence length.
-    preprocessor = keras_nlp.models.XLMRobertaPreprocessor.from_preset(
-        "xlm_roberta_base_multi",
-        sequence_length=128,
-    )
-
-    # Create a XLMRobertaClassifier and fit your data.
-    classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
-        "xlm_roberta_base_multi",
-        num_classes=4,
-        preprocessor=preprocessor,
-    )
+    # Re-compile (e.g., with a new learning rate).
     classifier.compile(
         loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+        optimizer=keras.optimizers.Adam(5e-5),
+        jit_compile=True,
     )
+    # Access backbone programmatically (e.g., to change `trainable`).
+    classifier.backbone.trainable = False
+    # Fit again.
     classifier.fit(x=features, y=labels, batch_size=2)
     ```
 
-    Preprocessed inputs.
+    Preprocessed integer data.
     ```python
-    # Create a dataset with preprocessed features in an `(x, y)` format.
-    preprocessed_features = {
+    features = {
         "token_ids": tf.ones(shape=(2, 12), dtype=tf.int64),
         "padding_mask": tf.constant(
             [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 2, shape=(2, 12)
         ),
     }
     labels = [0, 3]
 
-    # Create a XLMRobertaClassifier and fit your data.
+    # Pretrained classifier without preprocessing.
     classifier = keras_nlp.models.XLMRobertaClassifier.from_preset(
         "xlm_roberta_base_multi",
         num_classes=4,
         preprocessor=None,
     )
-    classifier.compile(
-        loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+    classifier.fit(x=features, y=labels, batch_size=2)
+    ```
+
+    Custom backbone and vocabulary.
+    ```python
+    features = ["The quick brown fox jumped.", "نسيت الواجب"]
+    labels = [0, 3]
+
+    def train_sentencepiece(ds, vocab_size):
+        bytes_io = io.BytesIO()
+        sentencepiece.SentencePieceTrainer.train(
+            sentence_iterator=ds.as_numpy_iterator(),
+            model_writer=bytes_io,
+            vocab_size=vocab_size,
+            model_type="WORD",
+            unk_id=0,
+            bos_id=1,
+            eos_id=2,
+        )
+        return bytes_io.getvalue()
+    ds = tf.data.Dataset.from_tensor_slices(
+        ["the quick brown fox", "the earth is round"]
+    )
+    proto = train_sentencepiece(ds, vocab_size=10)
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer(
+        proto=proto
+    )
+    preprocessor = keras_nlp.models.XLMRobertaPreprocessor(
+        tokenizer,
+        sequence_length=128,
+    )
+    backbone = keras_nlp.models.XLMRobertaBackbone(
+        vocabulary_size=250002,
+        num_layers=4,
+        num_heads=4,
+        hidden_dim=256,
+        intermediate_dim=512,
+        max_sequence_length=128,
+    )
+    classifier = keras_nlp.models.XLMRobertaClassifier(
+        backbone=backbone,
+        preprocessor=preprocessor,
+        num_classes=4,
     )
-    classifier.fit(x=preprocessed_features, y=labels, batch_size=2)
+    classifier.fit(x=features, y=labels, batch_size=2)
     ```
     """
 
     def __init__(
         self,
         backbone,
-        num_classes=2,
+        num_classes,
+        preprocessor=None,
+        activation=None,
         hidden_dim=None,
         dropout=0.0,
-        preprocessor=None,
         **kwargs,
     ):
         inputs = backbone.input
-        if hidden_dim is None:
-            hidden_dim = backbone.hidden_dim
+        hidden_dim = hidden_dim or backbone.hidden_dim
 
         x = backbone(inputs)[:, backbone.start_token_index, :]
         x = keras.layers.Dropout(dropout, name="pooled_dropout")(x)
         x = keras.layers.Dense(
             hidden_dim, activation="tanh", name="pooled_dense"
         )(x)
         x = keras.layers.Dropout(dropout, name="classifier_dropout")(x)
         outputs = keras.layers.Dense(
             num_classes,
             kernel_initializer=roberta_kernel_initializer(),
+            activation=activation,
             name="logits",
         )(x)
 
         # Instantiate using Functional API Model constructor
         super().__init__(
             inputs=inputs,
             outputs=outputs,
             include_preprocessing=preprocessor is not None,
             **kwargs,
         )
         # All references to `self` below this line
         self.backbone = backbone
         self.preprocessor = preprocessor
         self.num_classes = num_classes
+        self.activation = keras.activations.get(activation)
         self.hidden_dim = hidden_dim
         self.dropout = dropout
 
         self.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+            loss=keras.losses.SparseCategoricalCrossentropy(
+                from_logits=activation is None
+            ),
             optimizer=keras.optimizers.Adam(5e-5),
             metrics=keras.metrics.SparseCategoricalAccuracy(),
             jit_compile=is_xla_compatible(self),
         )
 
     def preprocess_samples(self, x, y=None, sample_weight=None):
         return self.preprocessor(x, y=y, sample_weight=sample_weight)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "num_classes": self.num_classes,
+                "activation": keras.activations.serialize(self.activation),
                 "hidden_dim": self.hidden_dim,
                 "dropout": self.dropout,
             }
         )
         return config
 
     @classproperty
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/f_net/f_net_masked_lm_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,137 +7,124 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for XLM-RoBERTa classification model."""
-
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_backbone import XLMRobertaBackbone
-from keras_nlp.models.xlm_roberta.xlm_roberta_classifier import (
-    XLMRobertaClassifier,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
-    XLMRobertaPreprocessor,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
-    XLMRobertaTokenizer,
+from keras_nlp.models.f_net.f_net_backbone import FNetBackbone
+from keras_nlp.models.f_net.f_net_masked_lm import FNetMaskedLM
+from keras_nlp.models.f_net.f_net_masked_lm_preprocessor import (
+    FNetMaskedLMPreprocessor,
 )
+from keras_nlp.models.f_net.f_net_tokenizer import FNetTokenizer
 
 
-class XLMRobertaClassifierTest(tf.test.TestCase, parameterized.TestCase):
+class FNetMaskedLMTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
+        # Setup Model.
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
-            ["the quick brown fox", "the earth is round"]
+            ["the quick brown fox", "the slow brown fox"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=5,
             model_type="WORD",
-            unk_id=0,
+            pad_id=0,
             bos_id=1,
             eos_id=2,
+            unk_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
+        )
+        self.proto = bytes_io.getvalue()
+        self.preprocessor = FNetMaskedLMPreprocessor(
+            FNetTokenizer(proto=self.proto),
+            sequence_length=5,
+            mask_selection_length=2,
         )
-        self.preprocessor = XLMRobertaPreprocessor(
-            tokenizer=XLMRobertaTokenizer(proto=bytes_io.getvalue()),
-            sequence_length=12,
-        )
-        self.backbone = XLMRobertaBackbone(
-            vocabulary_size=1000,
+        self.backbone = FNetBackbone(
+            vocabulary_size=self.preprocessor.tokenizer.vocabulary_size(),
             num_layers=2,
-            num_heads=2,
-            hidden_dim=64,
-            intermediate_dim=128,
-            max_sequence_length=128,
+            hidden_dim=2,
+            intermediate_dim=4,
+            max_sequence_length=self.preprocessor.packer.sequence_length,
         )
-        self.classifier = XLMRobertaClassifier(
+        self.masked_lm = FNetMaskedLM(
             self.backbone,
-            4,
             preprocessor=self.preprocessor,
         )
-        self.classifier_no_preprocessing = XLMRobertaClassifier(
-            self.backbone,
-            4,
-            preprocessor=None,
-        )
 
         self.raw_batch = tf.constant(
             [
-                "the quick brown fox.",
-                "the slow brown fox.",
-                "the earth is round",
-                "the earth is spherical",
+                "the quick brown fox",
+                "the slow brown fox",
             ]
         )
-        self.preprocessed_batch = self.preprocessor(self.raw_batch)
+        self.preprocessed_batch = self.preprocessor(self.raw_batch)[0]
         self.raw_dataset = tf.data.Dataset.from_tensor_slices(
-            (self.raw_batch, tf.ones((4,)))
+            self.raw_batch
         ).batch(2)
         self.preprocessed_dataset = self.raw_dataset.map(self.preprocessor)
 
     def test_valid_call_classifier(self):
-        self.classifier(self.preprocessed_batch)
+        self.masked_lm(self.preprocessed_batch)
 
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict(self, jit_compile):
-        self.classifier.compile(jit_compile=jit_compile)
-        self.classifier.predict(self.raw_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_predict_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(jit_compile=jit_compile)
-        self.classifier_no_preprocessing.predict(self.preprocessed_batch)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit(self, jit_compile):
-        self.classifier.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
+    def test_classifier_predict(self):
+        # self.masked_lm.predict(self.raw_batch)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.predict(self.preprocessed_batch)
+
+    def test_classifier_fit(self):
+        self.masked_lm.fit(self.raw_dataset)
+        self.masked_lm.preprocessor = None
+        self.masked_lm.fit(self.preprocessed_dataset)
+
+    def test_classifier_fit_no_xla(self):
+        self.masked_lm.preprocessor = None
+        self.masked_lm.compile(
+            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=False),
+            jit_compile=False,
+        )
+        self.masked_lm.fit(self.preprocessed_dataset)
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.masked_lm)
+        new_classifier = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_classifier.get_config(),
+            self.masked_lm.get_config(),
         )
-        self.classifier.fit(self.raw_dataset)
-
-    @parameterized.named_parameters(
-        ("jit_compile_false", False), ("jit_compile_true", True)
-    )
-    def test_classifier_fit_no_preprocessing(self, jit_compile):
-        self.classifier_no_preprocessing.compile(
-            loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-            jit_compile=jit_compile,
-        )
-        self.classifier_no_preprocessing.fit(self.preprocessed_dataset)
-
-    def test_xlmroberta_classifier_fit_default_compile(self):
-        self.classifier.fit(self.raw_dataset)
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
-    def test_saving_model(self, save_format, filename):
-        model_output = self.classifier.predict(self.raw_batch)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        self.classifier.save(save_path, save_format=save_format)
-        restored_model = keras.models.load_model(save_path)
+    @pytest.mark.large
+    def test_saved_model(self, save_format, filename):
+        model_output = self.masked_lm.predict(self.raw_batch)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        self.masked_lm.save(path, save_format=save_format, **kwargs)
+        restored_model = keras.models.load_model(path)
 
         # Check we got the real object back.
-        self.assertIsInstance(restored_model, XLMRobertaClassifier)
+        self.assertIsInstance(restored_model, FNetMaskedLM)
 
         # Check that output matches.
         restored_output = restored_model.predict(self.raw_batch)
-        self.assertAllClose(model_output, restored_output)
+        self.assertAllClose(model_output, restored_output, atol=0.01, rtol=0.01)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/bert/bert_masked_lm_preprocessor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,189 @@
-# Copyright 2023 The KerasNLP Authors
+# Copyright 2022 The KerasNLP Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""XLM-RoBERTa preprocessor layer."""
+"""BERT masked language model preprocessor layer."""
 
-import copy
+from absl import logging
 
-from tensorflow import keras
-
-from keras_nlp.models.preprocessor import Preprocessor
-from keras_nlp.models.roberta.roberta_preprocessor import (
-    RobertaMultiSegmentPacker,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
-    XLMRobertaTokenizer,
-)
-from keras_nlp.utils.keras_utils import (
-    convert_inputs_to_list_of_tensor_segments,
-)
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.layers.masked_lm_mask_generator import MaskedLMMaskGenerator
+from keras_nlp.models.bert.bert_preprocessor import BertPreprocessor
 from keras_nlp.utils.keras_utils import pack_x_y_sample_weight
-from keras_nlp.utils.python_utils import classproperty
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class XLMRobertaPreprocessor(Preprocessor):
-    """XLM-RoBERTa preprocessing layer.
-
-    This preprocessing layer will do three things:
-
-    - Tokenize any number of input segments using the `tokenizer`.
-    - Pack the inputs together with the appropriate `"<s>"`, `"</s>"` and
-      `"<pad>"` tokens, i.e., adding a single `"<s>"` at the start of the
-      entire sequence, `"</s></s>"` at the end of each segment, save the last
-      and a `"</s>"` at the end of the entire sequence.
-    - Construct a dictionary with keys `"token_ids"` and `"padding_mask"`,
-      that can be passed directly to a XLM-RoBERTa model.
-
-    This layer can be used directly with `tf.data.Dataset.map` to preprocess
-    string data in the `(x, y, sample_weight)` format used by
-    `keras.Model.fit`.
-
-    The call method of this layer accepts three arguments, `x`, `y`, and
-    `sample_weight`. `x` can be a python string or tensor representing a single
-    segment, a list of python strings representing a batch of single segments,
-    or a list of tensors representing multiple segments to be packed together.
-    `y` and `sample_weight` are both optional, can have any format, and will be
-    passed through unaltered.
-
-    Special care should be taken when using `tf.data` to map over an unlabeled
-    tuple of string segments. `tf.data.Dataset.map` will unpack this tuple
-    directly into the call arguments of this layer, rather than forward all
-    argument to `x`. To handle this case, it is recommended to  explicitly call
-    the layer, e.g. `ds.map(lambda seg1, seg2: preprocessor(x=(seg1, seg2)))`.
+@keras_nlp_export("keras_nlp.models.BertMaskedLMPreprocessor")
+class BertMaskedLMPreprocessor(BertPreprocessor):
+    """BERT preprocessing for the masked language modeling task.
+
+    This preprocessing layer will prepare inputs for a masked language modeling
+    task. It is primarily intended for use with the
+    `keras_nlp.models.BertMaskedLM` task model. Preprocessing will occur in
+    multiple steps.
+
+    1. Tokenize any number of input segments using the `tokenizer`.
+    2. Pack the inputs together with the appropriate `"[CLS]"`, `"[SEP]"` and
+      `"[PAD]"` tokens.
+    3. Randomly select non-special tokens to mask, controlled by
+      `mask_selection_rate`.
+    4. Construct a `(x, y, sample_weight)` tuple suitable for training with a
+      `keras_nlp.models.BertMaskedLM` task model.
 
     Args:
-        tokenizer: A `keras_nlp.tokenizers.XLMRobertaTokenizer` instance.
-        sequence_length: The length of the packed inputs.
-        truncate: The algorithm to truncate a list of batched segments to fit
-            within `sequence_length`. The value can be either `round_robin` or
-            `waterfall`:
+        tokenizer: A `keras_nlp.models.BertTokenizer` instance.
+        sequence_length: int. The length of the packed inputs.
+        truncate: string. The algorithm to truncate a list of batched segments
+            to fit within `sequence_length`. The value can be either
+            `round_robin` or `waterfall`:
                 - `"round_robin"`: Available space is assigned one token at a
                     time in a round-robin fashion to the inputs that still need
                     some, until the limit is reached.
                 - `"waterfall"`: The allocation of the budget is done using a
                     "waterfall" algorithm that allocates quota in a
                     left-to-right manner and fills up the buckets until we run
                     out of budget. It supports an arbitrary number of segments.
+        mask_selection_rate: float. The probability an input token will be
+            dynamically masked.
+        mask_selection_length: int. The maximum number of masked tokens
+            in a given sample.
+        mask_token_rate: float. The probability the a selected token will be
+            replaced with the mask token.
+        random_token_rate: float. The probability the a selected token will be
+            replaced with a random token from the vocabulary. A selected token
+            will be left as is with probability
+            `1 - mask_token_rate - random_token_rate`.
+
+    Call arguments:
+        x: A tensor of single string sequences, or a tuple of multiple
+            tensor sequences to be packed together. Inputs may be batched or
+            unbatched. For single sequences, raw python inputs will be converted
+            to tensors. For multiple sequences, pass tensors directly.
+        y: Label data. Should always be `None` as the layer generates labels.
+        sample_weight: Label weights. Should always be `None` as the layer
+            generates label weights.
 
     Examples:
+
+    Directly calling the layer on data.
     ```python
-    # Load the preprocessor from a preset.
-    preprocessor = keras_nlp.models.XLMRobertaPreprocessor.from_preset("xlm_roberta_base_multi")
+    preprocessor = keras_nlp.models.BertMaskedLMPreprocessor.from_preset(
+        "bert_base_en_uncased"
+    )
 
-    # Tokenize and pack a single sentence.
-    sentence = tf.constant("The quick brown fox jumped.")
-    preprocessor(sentence)
-    # Same output.
+    # Tokenize and mask a single sentence.
     preprocessor("The quick brown fox jumped.")
 
-    # Tokenize and a batch of single sentences.
-    sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    preprocessor(sentences)
-    # Same output.
-    preprocessor(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
+    # Tokenize and mask a batch of single sentences.
+    preprocessor(["The quick brown fox jumped.", "Call me Ishmael."])
 
-    # Tokenize and pack a sentence pair.
-    first_sentence = tf.constant("The quick brown fox jumped.")
-    second_sentence = tf.constant("The fox tripped.")
-    preprocessor((first_sentence, second_sentence))
-
-    # Map a dataset to preprocess a single sentence.
-    features = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    labels = tf.constant([0, 1])
-    ds = tf.data.Dataset.from_tensor_slices((features, labels))
-    ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
+    # Tokenize and mask sentence pairs.
+    # In this case, always convert input to tensors before calling the layer.
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+    preprocessor((first, second))
+    ```
 
-    # Map a dataset to preprocess sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    labels = tf.constant([1, 1])
-    ds = tf.data.Dataset.from_tensor_slices(
-        (
-            (first_sentences, second_sentences), labels
-        )
+    Mapping with `tf.data.Dataset`.
+    ```python
+    preprocessor = keras_nlp.models.BertMaskedLMPreprocessor.from_preset(
+        "bert_base_en_uncased"
     )
+
+    first = tf.constant(["The quick brown fox jumped.", "Call me Ishmael."])
+    second = tf.constant(["The fox tripped.", "Oh look, a whale."])
+
+    # Map single sentences.
+    ds = tf.data.Dataset.from_tensor_slices(first)
     ds = ds.map(preprocessor, num_parallel_calls=tf.data.AUTOTUNE)
 
-    # Map a dataset to preprocess unlabeled sentence pairs.
-    first_sentences = tf.constant(
-        ["The quick brown fox jumped.", "Call me Ishmael."]
-    )
-    second_sentences = tf.constant(
-        ["The fox tripped.", "Oh look, a whale."]
-    )
-    ds = tf.data.Dataset.from_tensor_slices((first_sentences, second_sentences))
+    # Map sentence pairs.
+    ds = tf.data.Dataset.from_tensor_slices((first, second))
     # Watch out for tf.data's default unpacking of tuples here!
     # Best to invoke the `preprocessor` directly in this case.
     ds = ds.map(
-        lambda s1, s2: preprocessor(x=(s1, s2)),
+        lambda first, second: preprocessor(x=(first, second)),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
-
-    # Alternatively, you can create a preprocessor from your own vocabulary.
-    # The usage is exactly the same as above.
-    tokenizer = keras_nlp.models.XLMRobertaTokenizer(proto="model.spm")
-    preprocessor = keras_nlp.models.XLMRobertaPreprocessor(
-        tokenizer=tokenizer,
-        sequence_length=10,
-    )
     ```
     """
 
     def __init__(
         self,
         tokenizer,
         sequence_length=512,
         truncate="round_robin",
+        mask_selection_rate=0.15,
+        mask_selection_length=96,
+        mask_token_rate=0.8,
+        random_token_rate=0.1,
         **kwargs,
     ):
-        super().__init__(**kwargs)
-
-        self.tokenizer = tokenizer
-
-        self.packer = RobertaMultiSegmentPacker(
-            start_value=self.tokenizer.start_token_id,
-            end_value=self.tokenizer.end_token_id,
-            pad_value=self.tokenizer.pad_token_id,
-            truncate=truncate,
+        super().__init__(
+            tokenizer,
             sequence_length=sequence_length,
+            truncate=truncate,
+            **kwargs,
+        )
+
+        self.masker = MaskedLMMaskGenerator(
+            mask_selection_rate=mask_selection_rate,
+            mask_selection_length=mask_selection_length,
+            mask_token_rate=mask_token_rate,
+            random_token_rate=random_token_rate,
+            vocabulary_size=tokenizer.vocabulary_size(),
+            mask_token_id=tokenizer.mask_token_id,
+            unselectable_token_ids=[
+                tokenizer.cls_token_id,
+                tokenizer.sep_token_id,
+                tokenizer.pad_token_id,
+            ],
         )
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "sequence_length": self.packer.sequence_length,
-                "truncate": self.packer.truncate,
+                "mask_selection_rate": self.masker.mask_selection_rate,
+                "mask_selection_length": self.masker.mask_selection_length,
+                "mask_token_rate": self.masker.mask_token_rate,
+                "random_token_rate": self.masker.random_token_rate,
             }
         )
         return config
 
     def call(self, x, y=None, sample_weight=None):
-        x = convert_inputs_to_list_of_tensor_segments(x)
-        x = [self.tokenizer(segment) for segment in x]
-        token_ids = self.packer(x)
+        if y is not None or sample_weight is not None:
+            logging.warning(
+                f"{self.__class__.__name__} generates `y` and `sample_weight` "
+                "based on your input data, but your data already contains `y` "
+                "or `sample_weight`. Your `y` and `sample_weight` will be "
+                "ignored."
+            )
+
+        x = super().call(x)
+
+        token_ids, padding_mask, segment_ids = (
+            x["token_ids"],
+            x["padding_mask"],
+            x["segment_ids"],
+        )
+        masker_outputs = self.masker(token_ids)
         x = {
-            "token_ids": token_ids,
-            "padding_mask": token_ids != self.tokenizer.pad_token_id,
+            "token_ids": masker_outputs["token_ids"],
+            "padding_mask": padding_mask,
+            "segment_ids": segment_ids,
+            "mask_positions": masker_outputs["mask_positions"],
         }
+        y = masker_outputs["mask_ids"]
+        sample_weight = masker_outputs["mask_weights"]
         return pack_x_y_sample_weight(x, y, sample_weight)
-
-    @classproperty
-    def tokenizer_cls(cls):
-        return XLMRobertaTokenizer
-
-    @classproperty
-    def presets(cls):
-        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/albert/albert_preprocessor_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,82 +8,96 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for XLM-RoBERTa preprocessor layer."""
+"""Tests for ALBERT preprocessor layer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
-from keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor import (
-    XLMRobertaPreprocessor,
-)
-from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
-    XLMRobertaTokenizer,
-)
+from keras_nlp.models.albert.albert_preprocessor import AlbertPreprocessor
+from keras_nlp.models.albert.albert_tokenizer import AlbertTokenizer
 
 
-class XLMRobertaPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
+class AlbertPreprocessorTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         bytes_io = io.BytesIO()
         vocab_data = tf.data.Dataset.from_tensor_slices(
             ["the quick brown fox", "the earth is round"]
         )
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=vocab_data.as_numpy_iterator(),
             model_writer=bytes_io,
-            vocab_size=10,
+            vocab_size=12,
             model_type="WORD",
-            unk_id=0,
-            bos_id=1,
-            eos_id=2,
+            pad_id=0,
+            unk_id=1,
+            bos_id=2,
+            eos_id=3,
+            pad_piece="<pad>",
+            unk_piece="<unk>",
+            bos_piece="[CLS]",
+            eos_piece="[SEP]",
+            user_defined_symbols="[MASK]",
         )
         self.proto = bytes_io.getvalue()
 
-        self.preprocessor = XLMRobertaPreprocessor(
-            tokenizer=XLMRobertaTokenizer(proto=self.proto),
+        self.preprocessor = AlbertPreprocessor(
+            tokenizer=AlbertTokenizer(proto=self.proto),
             sequence_length=12,
         )
 
     def test_tokenize_strings(self):
         input_data = "the quick brown fox"
         output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]
+            output["token_ids"], [2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]
+        )
+        self.assertAllEqual(
+            output["segment_ids"], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         )
         self.assertAllEqual(
             output["padding_mask"], [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]
         )
 
     def test_tokenize_list_of_strings(self):
         # We should handle a list of strings as as batch.
         input_data = ["the quick brown fox"] * 4
         output = self.preprocessor(input_data)
         self.assertAllEqual(
-            output["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+            output["token_ids"],
+            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
+        )
+        self.assertAllEqual(
+            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
             output["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
 
     def test_tokenize_labeled_batch(self):
         x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         x_out, y_out, sw_out = self.preprocessor(x, y, sw)
         self.assertAllEqual(
-            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+            x_out["token_ids"],
+            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
+        )
+        self.assertAllEqual(
+            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
@@ -91,60 +105,83 @@
         x = tf.constant(["the quick brown fox"] * 4)
         y = tf.constant([1] * 4)
         sw = tf.constant([1.0] * 4)
         ds = tf.data.Dataset.from_tensor_slices((x, y, sw))
         ds = ds.map(self.preprocessor)
         x_out, y_out, sw_out = ds.batch(4).take(1).get_single_element()
         self.assertAllEqual(
-            x_out["token_ids"], [[0, 4, 9, 5, 7, 2, 1, 1, 1, 1, 1, 1]] * 4
+            x_out["token_ids"],
+            [[2, 5, 10, 6, 8, 3, 0, 0, 0, 0, 0, 0]] * 4,
+        )
+        self.assertAllEqual(
+            x_out["segment_ids"], [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(
             x_out["padding_mask"], [[1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 0, 0]] * 4
         )
         self.assertAllEqual(y_out, y)
         self.assertAllEqual(sw_out, sw)
 
     def test_tokenize_multiple_sentences(self):
         sentence_one = tf.constant("the quick brown fox")
         sentence_two = tf.constant("the earth")
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"], [0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]
+            output["token_ids"],
+            [2, 5, 10, 6, 8, 3, 5, 7, 3, 0, 0, 0],
+        )
+        self.assertAllEqual(
+            output["segment_ids"], [0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]
         )
         self.assertAllEqual(
-            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]
+            output["padding_mask"], [1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]
         )
 
     def test_tokenize_multiple_batched_sentences(self):
         sentence_one = tf.constant(["the quick brown fox"] * 4)
         sentence_two = tf.constant(["the earth"] * 4)
         # The first tuple or list is always interpreted as an enumeration of
         # separate sequences to concatenate.
         output = self.preprocessor((sentence_one, sentence_two))
         self.assertAllEqual(
-            output["token_ids"], [[0, 4, 9, 5, 7, 2, 2, 4, 6, 2, 1, 1]] * 4
+            output["token_ids"],
+            [[2, 5, 10, 6, 8, 3, 5, 7, 3, 0, 0, 0]] * 4,
         )
         self.assertAllEqual(
-            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0]] * 4
+            output["segment_ids"], [[0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0]] * 4
+        )
+        self.assertAllEqual(
+            output["padding_mask"], [[1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 0, 0]] * 4
         )
 
     def test_errors_for_2d_list_input(self):
         ambiguous_input = [["one", "two"], ["three", "four"]]
         with self.assertRaises(ValueError):
             self.preprocessor(ambiguous_input)
 
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.preprocessor)
+        new_preprocessor = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_preprocessor.get_config(),
+            self.preprocessor.get_config(),
+        )
+
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.preprocessor(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data)["token_ids"],
             restored_model(input_data)["token_ids"],
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             "description": (
                 "12-layer XLM-RoBERTa model where case is maintained. "
                 "Trained on CommonCrawl in 100 languages."
             ),
             "params": 277450752,
             "official_name": "XLM-RoBERTa",
             "path": "xlm_roberta",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/xlmr/README.md",
         },
         "config": {
             "vocabulary_size": 250002,
             "num_layers": 12,
             "num_heads": 12,
             "hidden_dim": 768,
             "intermediate_dim": 3072,
@@ -44,14 +45,15 @@
             "description": (
                 "24-layer XLM-RoBERTa model where case is maintained. "
                 "Trained on CommonCrawl in 100 languages."
             ),
             "params": 558837760,
             "official_name": "XLM-RoBERTa",
             "path": "xlm_roberta",
+            "model_card": "https://github.com/facebookresearch/fairseq/blob/main/examples/xlmr/README.md",
         },
         "config": {
             "vocabulary_size": 250002,
             "num_layers": 24,
             "num_heads": 16,
             "hidden_dim": 1024,
             "intermediate_dim": 4096,
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,30 @@
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output(self, load_weights):
         input_data = tf.constant(["The quick brown fox."])
         model = XLMRobertaClassifier.from_preset(
-            "xlm_roberta_base_multi", load_weights=load_weights
+            "xlm_roberta_base_multi", num_classes=2, load_weights=load_weights
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
         ("preset_weights", True), ("random_weights", False)
     )
     def test_classifier_output_without_preprocessing(self, load_weights):
         input_data = {
             "token_ids": tf.constant([[0, 581, 63773, 2]]),
             "padding_mask": tf.constant([[1, 1, 1, 1]]),
         }
         model = XLMRobertaClassifier.from_preset(
             "xlm_roberta_base_multi",
+            num_classes=2,
             load_weights=load_weights,
             preprocessor=None,
         )
         # Never assert output values, as the head weights are random.
         model.predict(input_data)
 
     @parameterized.named_parameters(
@@ -107,23 +108,23 @@
     )
     def test_preset_docstring(self, cls):
         """Check we did our docstring formatting correctly."""
         for name in cls.presets:
             self.assertRegex(cls.from_preset.__doc__, name)
 
     @parameterized.named_parameters(
-        ("xlm_roberta_tokenizer", XLMRobertaTokenizer),
-        ("xlm_roberta_preprocessor", XLMRobertaPreprocessor),
-        ("xlm_roberta", XLMRobertaBackbone),
-        ("xlm_roberta_classifier", XLMRobertaClassifier),
+        ("xlm_roberta_tokenizer", XLMRobertaTokenizer, {}),
+        ("xlm_roberta_preprocessor", XLMRobertaPreprocessor, {}),
+        ("xlm_roberta", XLMRobertaBackbone, {}),
+        ("xlm_roberta_classifier", XLMRobertaClassifier, {"num_classes": 2}),
     )
-    def test_unknown_preset_error(self, cls):
+    def test_unknown_preset_error(self, cls, kwargs):
         # Not a preset name
         with self.assertRaises(ValueError):
-            cls.from_preset("xlm_roberta_base_clowntown")
+            cls.from_preset("xlm_roberta_base_clowntown", **kwargs)
 
 
 @pytest.mark.extra_large
 class XLMRobertaPresetFullTest(tf.test.TestCase, parameterized.TestCase):
     """
     Test the full enumeration of our preset.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,53 +13,65 @@
 # limitations under the License.
 
 """XLM-RoBERTa tokenizer."""
 
 import copy
 
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.models.xlm_roberta.xlm_roberta_presets import backbone_presets
 from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
 from keras_nlp.utils.python_utils import classproperty
 from keras_nlp.utils.tf_utils import tensor_to_string_list
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.models.XLMRobertaTokenizer")
 class XLMRobertaTokenizer(SentencePieceTokenizer):
-    """XLM-RoBERTa tokenizer layer based on SentencePiece.
+    """An XLM-RoBERTa tokenizer using SentencePiece subword segmentation.
 
     This tokenizer class will tokenize raw strings into integer sequences and
     is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
     underlying tokenizer, it will check for all special tokens needed by
     XLM-RoBERTa models and provides a `from_preset()` method to automatically
-    download a matching vocabulary for a XLM-RoBERTa preset.
+    download a matching vocabulary for an XLM-RoBERTa preset.
 
-    The original fairseq implementation of XLM-RoBERTa modifies the indices of
-    the SentencePiece tokenizer output. To preserve compatibility, we make the
-    same changes, i.e., `"<s>"`, `"<pad>"`, `"</s>"` and `"<unk>"` are mapped to
-    0, 1, 2, 3, respectively, and non-special token indices are shifted right
-    by one.
+    Note: If you are providing your own custom SentencePiece model, the original
+    fairseq implementation of XLM-RoBERTa re-maps some token indices from the
+    underlying sentencepiece output. To preserve compatibility, we do the same
+    re-mapping here.
 
     If input is a batch of strings (rank > 0), the layer will output a
     `tf.RaggedTensor` where the last dimension of the output is ragged.
 
     If input is a scalar string (rank == 0), the layer will output a dense
     `tf.Tensor` with static shape `[None]`.
 
     Args:
-        proto: Either a `string` path to a SentencePiece proto file, or a
+        proto: Either a `string` path to a SentencePiece proto file or a
             `bytes` object with a serialized SentencePiece proto. See the
             [SentencePiece repository](https://github.com/google/sentencepiece)
             for more details on the format.
 
     Examples:
-
     ```python
+    tokenizer = keras_nlp.models.XLMRobertaTokenizer.from_preset(
+        "xlm_roberta_base_multi",
+    )
+
+    # Unbatched inputs.
+    tokenizer("the quick brown fox")
+
+    # Batched inputs.
+    tokenizer(["the quick brown fox", "الأرض كروية"])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("the quick brown fox"))
+
+    # Custom vocabulary
     def train_sentencepiece(ds, vocab_size):
         bytes_io = io.BytesIO()
         sentencepiece.SentencePieceTrainer.train(
             sentence_iterator=ds.as_numpy_iterator(),
             model_writer=bytes_io,
             vocab_size=vocab_size,
             model_type="WORD",
@@ -68,95 +80,82 @@
             eos_id=2,
         )
         return bytes_io.getvalue()
 
     ds = tf.data.Dataset.from_tensor_slices(
         ["the quick brown fox", "the earth is round"]
     )
-
     proto = train_sentencepiece(ds, vocab_size=10)
     tokenizer = keras_nlp.models.XLMRobertaTokenizer(proto=proto)
-
-    # Batched inputs.
-    tokenizer(["the quick brown fox", "the earth is round"])
-
-    # Unbatched inputs.
-    tokenizer("the quick brown fox")
-
-    # Detokenization.
-    tokenizer.detokenize(tf.constant([[0, 4, 9, 5, 7, 2]]))
     ```
     """
 
     def __init__(self, proto, **kwargs):
         super().__init__(proto=proto, **kwargs)
 
         # List of special tokens.
         self._vocabulary_prefix = ["<s>", "<pad>", "</s>", "<unk>"]
 
         # IDs of special tokens.
         self.start_token_id = 0  # <s>
         self.pad_token_id = 1  # <pad>
         self.end_token_id = 2  # </s>
         self.unk_token_id = 3  # <unk>
+        self.mask_token_id = self.vocabulary_size() - 1  # <mask>
 
     def vocabulary_size(self):
         """Get the size of the tokenizer vocabulary."""
-        return super().vocabulary_size() + 1
+        return super().vocabulary_size() + 2
 
     def get_vocabulary(self):
         """Get the size of the tokenizer vocabulary."""
         vocabulary = tensor_to_string_list(
             self._sentence_piece.id_to_string(
                 tf.range(super().vocabulary_size())
             )
         )
-        return self._vocabulary_prefix + vocabulary[3:]
+        return self._vocabulary_prefix + vocabulary[3:] + ["<mask>"]
 
     def id_to_token(self, id):
         """Convert an integer id to a string token."""
+
+        if id == self.mask_token_id:
+            return "<mask>"
+
         if id < len(self._vocabulary_prefix):
             return self._vocabulary_prefix[id]
 
         return tensor_to_string_list(self._sentence_piece.id_to_string(id - 1))
 
     def token_to_id(self, token):
         """Convert a string token to an integer id."""
+
         if token in self._vocabulary_prefix:
             return self._vocabulary_prefix.index(token)
 
-        return int(self._sentence_piece.string_to_id(token).numpy()) + 1
+        spm_token_id = self._sentence_piece.string_to_id(token)
+
+        # OOV token
+        spm_unk_token_id = self._sentence_piece.string_to_id("<unk>")
+        if spm_token_id == spm_unk_token_id:
+            return self.unk_token_id
+
+        return int(spm_token_id.numpy()) + 1
 
     def tokenize(self, inputs):
         tokens = super().tokenize(inputs)
 
         # Correct `unk_token_id` (0 -> 3). Note that we do not correct
         # `start_token_id` and `end_token_id`; they are dealt with in
         # `XLMRobertaPreprocessor`.
         tokens = tf.where(tf.equal(tokens, 0), self.unk_token_id - 1, tokens)
 
         # Shift the tokens IDs right by one.
         return tf.add(tokens, 1)
 
-    def detokenize(self, inputs):
-        if inputs.dtype == tf.string:
-            return super().detokenize(inputs)
-
-        # Shift the tokens IDs left by one.
-        tokens = tf.subtract(inputs, 1)
-
-        # Correct `unk_token_id`, `end_token_id`, `start_token_id`, respectively.
-        # Note: The `pad_token_id` is taken as 0 (`unk_token_id`) since the
-        # proto does not contain `pad_token_id`. This mapping of the pad token
-        # is done automatically by the above subtraction.
-        tokens = tf.where(tf.equal(tokens, self.unk_token_id - 1), 0, tokens)
-        tokens = tf.where(tf.equal(tokens, self.end_token_id - 1), 2, tokens)
-        tokens = tf.where(tf.equal(tokens, self.start_token_id - 1), 1, tokens)
-
-        # Note: Even though we map `"<s>" and `"</s>"` to the correct IDs,
-        # the `detokenize` method will return empty strings for these tokens.
-        # This is a vagary of the `sentencepiece` library.
-        return super().detokenize(tokens)
+    def detokenize(self, ids):
+        ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
+        return super().detokenize(ids)
 
     @classproperty
     def presets(cls):
         return copy.deepcopy(backbone_presets)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Tests for XLM-RoBERTa tokenizer."""
 
 import io
 import os
 
+import pytest
 import sentencepiece
 import tensorflow as tf
 from absl.testing import parameterized
 from tensorflow import keras
 
 from keras_nlp.models.xlm_roberta.xlm_roberta_tokenizer import (
     XLMRobertaTokenizer,
@@ -61,15 +62,15 @@
 
         output = self.tokenizer(input_data)
         self.assertAllEqual(output, [4, 9, 5, 7, 3])
 
     def test_detokenize(self):
         input_data = tf.constant([[4, 9, 5, 7]])
         output = self.tokenizer.detokenize(input_data)
-        self.assertEqual(output, tf.constant(["the quick brown fox"]))
+        self.assertEqual(output, tf.constant(["brown round earth is"]))
 
     def test_vocabulary(self):
         vocabulary = self.tokenizer.get_vocabulary()
         self.assertAllEqual(
             vocabulary,
             [
                 "<s>",
@@ -79,39 +80,55 @@
                 "▁the",
                 "▁brown",
                 "▁earth",
                 "▁fox",
                 "▁is",
                 "▁quick",
                 "▁round",
+                "<mask>",
             ],
         )
-        self.assertEqual(self.tokenizer.vocabulary_size(), 11)
+        self.assertEqual(self.tokenizer.vocabulary_size(), 12)
 
     def test_id_to_token(self):
         print(self.tokenizer.id_to_token(9))
         self.assertEqual(self.tokenizer.id_to_token(9), "▁quick")
         self.assertEqual(self.tokenizer.id_to_token(5), "▁brown")
 
     def test_token_to_id(self):
         self.assertEqual(self.tokenizer.token_to_id("▁the"), 4)
         self.assertEqual(self.tokenizer.token_to_id("▁round"), 10)
+        # Test any random OOV token.
+        self.assertEqual(self.tokenizer.token_to_id("<oov-token>"), 3)
+        # Test a special token.
+        self.assertEqual(self.tokenizer.token_to_id("<pad>"), 1)
+
+    def test_serialization(self):
+        config = keras.utils.serialize_keras_object(self.tokenizer)
+        new_tokenizer = keras.utils.deserialize_keras_object(config)
+        self.assertEqual(
+            new_tokenizer.get_config(),
+            self.tokenizer.get_config(),
+        )
 
     @parameterized.named_parameters(
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
+    @pytest.mark.large  # Saving is slow, so mark these large.
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown fox"])
 
         inputs = keras.Input(dtype="string", shape=())
         outputs = self.tokenizer(inputs)
         model = keras.Model(inputs, outputs)
 
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
 
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,41 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.samplers.beam_sampler import BeamSampler
+from keras_nlp.samplers.contrastive_sampler import ContrastiveSampler
 from keras_nlp.samplers.greedy_sampler import GreedySampler
-from keras_nlp.samplers.sampler import Sampler
+from keras_nlp.samplers.random_sampler import RandomSampler
 from keras_nlp.samplers.top_k_sampler import TopKSampler
 from keras_nlp.samplers.top_p_sampler import TopPSampler
 
 
+@keras_nlp_export("keras_nlp.samplers.serialize")
 def serialize(sampler):
     return keras.utils.serialize_keras_object(sampler)
 
 
+@keras_nlp_export("keras_nlp.samplers.deserialize")
 def deserialize(config, custom_objects=None):
     """Return a `Sampler` object from its config."""
     all_classes = {
         "beam": BeamSampler,
+        "contrastive": ContrastiveSampler,
         "greedy": GreedySampler,
+        "random": RandomSampler,
         "top_k": TopKSampler,
         "top_p": TopPSampler,
     }
     return keras.utils.deserialize_keras_object(
         config,
         module_objects=all_classes,
         custom_objects=custom_objects,
         printable_module_name="samplers",
     )
 
 
+@keras_nlp_export("keras_nlp.samplers.get")
 def get(identifier):
     """Retrieve a KerasNLP sampler by the identifier.
 
     The `identifier` may be the string name of a sampler class or class.
 
     >>> identifier = 'greedy'
     >>> sampler = keras_nlp.samplers.get(identifier)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/beam_sampler.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/beam_sampler.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,207 +11,225 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Beam Sampler."""
 
 import tensorflow as tf
 from tensorflow import keras
+from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import base_sampler_args_docstring
 from keras_nlp.samplers.sampler import call_args_docstring
 from keras_nlp.utils.python_utils import format_docstring
 
 
-@format_docstring(
-    base_sampler_args=base_sampler_args_docstring, call_args=call_args_docstring
-)
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@format_docstring(call_args=call_args_docstring)
+@keras_nlp_export("keras_nlp.samplers.BeamSampler")
 class BeamSampler(Sampler):
     """Beam Sampler class.
 
     This sampler implements beam search algorithm. At each time-step, beam
     search keeps the beams (sequences) of the top `num_beams` highest
     accumulated probabilities, and uses each one of the beams to predict
     candidate next tokens.
 
     Args:
         num_beams: int. The number of beams that should be kept at each
             time-step. `num_beams` should be strictly positive.
-        {{base_sampler_args}}
+        return_all_beams: bool. When set to `True`, the sampler will return all
+            beams and their respective probabilities score.
 
-    Call Args:
+    Call arguments:
         {{call_args}}
 
     Examples:
+    Return only the beam with the highest accumulated probability.
     ```python
-    VOCAB_SIZE = 10
+    # Use a simple alphabet of lowercase characters with ids in range [0, 25].
+    int_lookup = {i: chr(i + ord('a')) for i in range(26)}
+    char_lookup = {v: k for k, v in int_lookup.items()}
+    batch_size, length, vocab_size = 1, 12, len(int_lookup)
+
+    def next(prompt, cache, index):
+        prompt_batch_size = tf.shape(prompt)[0]
+        hidden_states = tf.ones((prompt_batch_size, 10))
+        # A uniform distribution over our alphabet.
+        logits = tf.ones((prompt_batch_size, vocab_size))
+        return logits, hidden_states, cache
+
+    output = keras_nlp.samplers.BeamSampler()(
+        next=next,
+        prompt=tf.fill((batch_size, length), char_lookup["z"]),
+        index=5,
+    )
+    print(["".join([int_lookup[i] for i in s]) for s in output.numpy()])
+    # >>> ['zzzzzeeeeeee']
+    ```
 
-    # Create a dummy model to predict the next token.
-    model = keras.Sequential(
-        [
-            keras.Input(shape=[None]),
-            keras.layers.Embedding(
-                input_dim=VOCAB_SIZE,
-                output_dim=16,
-            ),
-            keras.layers.Dense(VOCAB_SIZE, activation="softmax"),
-        ]
+    Return all beams and their probabilities.
+    ```python
+    # Use a simple alphabet of lowercase characters with ids in range [0, 25].
+    int_lookup = {i: chr(i + ord('a')) for i in range(26)}
+    char_lookup = {v: k for k, v in int_lookup.items()}
+    batch_size, length, vocab_size = 1, 8, len(int_lookup)
+
+    def next(prompt, cache, index):
+        prompt_batch_size = tf.shape(prompt)[0]
+        hidden_states = tf.ones((prompt_batch_size, 10))
+        # A uniform distribution over our alphabet.
+        logits = tf.ones((batch_size, vocab_size))
+        return logits, hidden_states, cache
+
+    beams, probs = keras_nlp.samplers.BeamSampler(return_all_beams=True)(
+        next=next,
+        prompt=tf.fill((batch_size, length,), char_lookup['z']),
+        index=5,
     )
 
-    # Define a function that outputs the next token's probability for each token
-    # in the input sequence.
-    def token_probability_fn(inputs, mask):
-        return model(inputs)
-
-    prompt = tf.fill((8, 1), 1)
-
-    sampler = keras_nlp.samplers.BeamSampler(num_beams=3)
-    # Print the generated sequence (token ids).
-    print(sampler(prompt, token_probability_fn, max_length=10))
+    print(beams.shape)
+    # >>> (1, 5, 8)
+    print(probs.shape)
+    # >>> (1, 5)
+    print(["".join([int_lookup[i] for i in s]) for s in beams[0].numpy()])
+    # >>> ['zzzzzeee', 'zzzzzeed', 'zzzzzeec', 'zzzzzeea', 'zzzzzeeb']
     ```
     """
 
     def __init__(
         self,
         num_beams=5,
-        jit_compile=True,
-        run_eagerly=False,
+        return_all_beams=False,
+        **kwargs,
     ):
+        super().__init__(**kwargs)
         self.num_beams = num_beams
-        super().__init__(jit_compile=jit_compile, run_eagerly=run_eagerly)
-
-    def get_next_token(self, next_token_probs):
-        # Beam search overrides the whole `sample` method.
-        pass
+        self.return_all_beams = return_all_beams
 
-    def sample(
-        self, prompt, token_probability_fn, mask, num_steps, from_logits=True
+    def __call__(
+        self,
+        next,
+        prompt,
+        cache=None,
+        index=0,
+        mask=None,
+        end_token_id=None,
+        hidden_states=None,
     ):
-        """Sampling logic implementation.
-
-        Because beam search uses a different loop body, we have to override the
-        whole `sample` method instead of just the `get_next_token` method.
-        """
         batch_size, max_length = tf.shape(prompt)[0], tf.shape(prompt)[1]
-        max_length = tf.cast(max_length, num_steps.dtype)
-        length = max_length - num_steps
-        dummy_preds = token_probability_fn(prompt, mask=mask)
-        vocab_size = tf.shape(dummy_preds)[-1]
-        pred_dtype = dummy_preds.dtype
-
-        num_beams = self.num_beams
-
-        # Initialize beam with shape `(batch_size, num_beams, length)`.
-        beams = tf.repeat(tf.expand_dims(prompt, axis=1), num_beams, axis=1)
-        # Initialize `beams_prob` with shape `(batch_size, num_beams)`.
-        beams_prob = tf.zeros([batch_size, 1], dtype=pred_dtype)
-        beams_prob = tf.concat(
-            [beams_prob, tf.fill((batch_size, num_beams - 1), pred_dtype.min)],
-            axis=-1,
-        )
+        # Make sure max length and start index are the same dtype.
+        index = tf.cast(index, max_length.dtype)
 
-        def one_step(beams, beams_prob, length, mask):
-            flattened_beams = tf.reshape(
-                beams, shape=[batch_size * num_beams, -1]
-            )
-            repeated_mask = tf.tile(mask, [num_beams, 1])
-            probs = token_probability_fn(flattened_beams, repeated_mask)
-            preds = tf.gather(
-                probs,
-                tf.repeat(length - 1, batch_size * num_beams),
-                axis=1,
-                batch_dims=1,
-            )
-            if from_logits:
-                preds = keras.activations.softmax(preds, axis=-1)
-            # Reshape `preds` to shape `(batch_size, num_beams * vocab_size)`.
-
-            preds = tf.reshape(preds, shape=[batch_size, -1])
-
-            cum_probs = tf.math.log(preds) + tf.repeat(
-                beams_prob, repeats=vocab_size, axis=1
-            )
-
-            candidate_prob, candidate_indexes = tf.math.top_k(
-                cum_probs, k=num_beams, sorted=False
-            )
+        def create_beams(x):
+            """Add initial beam state."""
+            return tf.repeat(x, self.num_beams, axis=0)
+
+        def flatten_beams(x):
+            """Combine the beam dim and batch dim."""
+            flat_shape = [batch_size * self.num_beams] + x.shape.as_list()[2:]
+            return tf.reshape(x, shape=flat_shape)
+
+        def unflatten_beams(x):
+            """Separate the beam dim and batch dim."""
+            unflat_shape = [batch_size, self.num_beams] + x.shape.as_list()[1:]
+            return tf.reshape(x, shape=unflat_shape)
+
+        if mask is None:
+            mask = tf.zeros_like(prompt, dtype=tf.bool)
+        else:
+            mask = tf.cast(mask, dtype=tf.bool)
+        # `tf.while_loop` will not accept `None` as a value for `loop_vars`.
+        cache = () if cache is None else cache
+        # Add extra sequences for each beam.
+        prompt, mask = create_beams(prompt), create_beams(mask)
+        cache = tf.nest.map_structure(create_beams, cache)
+        # Setup the initial beam log-likelihoods.
+        # On the first loop, make sure only the original beam is considered.
+        log_probs = tf.constant([[0.0] + [-1e9] * (self.num_beams - 1)])
+        log_probs = flatten_beams(tf.repeat(log_probs, batch_size, axis=0))
+
+        def cond(prompt, cache, index, log_probs):
+            if end_token_id is None:
+                return True
+            # Stop if all sequences have produced a *new* end_token_id.
+            end_tokens = (prompt == end_token_id) & (~mask)
+            prompt_done = tf.reduce_any(end_tokens, axis=-1)
+            return not tf.reduce_all(prompt_done)
+
+        def body(prompt, cache, index, log_probs):
+            # Compute the softmax distribution for the next token.
+            logits, _, cache = next(prompt, cache, index)
+            vocab_size = tf.shape(logits)[-1]
+            probs = keras.activations.softmax(logits / self.temperature)
 
-            candidate_beam_indexes = candidate_indexes // vocab_size
-            next_token = candidate_indexes % vocab_size
-
-            beams = tf.gather(
-                beams, candidate_beam_indexes, axis=1, batch_dims=1
-            )
-
-            # Build a new column of updates to scatter into the beam tensor.
-            next_token = tf.where(
-                condition=mask[..., length, tf.newaxis],
-                x=beams[..., length],
-                y=next_token,
-            )
-            next_token = tf.reshape(next_token, shape=[-1])
-
-            mask = tf.tensor_scatter_nd_update(
-                tensor=mask,
-                indices=tf.stack(
-                    (
-                        tf.cast(tf.range(batch_size), dtype=length.dtype),
-                        tf.repeat(length, batch_size),
-                    ),
-                    axis=1,
-                ),
-                updates=tf.repeat(True, batch_size),
-            )
-
-            # Generate `(batch_index, beam_index)` tuples for each beam.
-            beam_indices = tf.where(tf.ones((batch_size, num_beams), tf.bool))
-            beam_indices = tf.cast(beam_indices, dtype=length.dtype)
-            # Build a tensor of repeated `length` values.
-            length_indices = tf.fill((batch_size * num_beams, 1), length)
-            # Concatenate to a triplet of `(batch_index, beam_index, length)`.
-            indices = tf.concat([beam_indices, length_indices], axis=-1)
-
-            # Update `beams[:, :, length]` with `next_token`.
-            beams = tf.tensor_scatter_nd_update(
-                tensor=beams,
-                indices=indices,
-                updates=next_token,
-            )
-
-            beams_prob = candidate_prob
-
-            length = tf.add(length, 1)
-            return beams, beams_prob, length, mask
+            # Compute the running log-likelihood of each new candidate.
+            next_log_probs = tf.math.log(probs) + log_probs[..., tf.newaxis]
+            # Reshape `preds` to shape `(batch_size, num_beams * vocab_size)`.
+            next_log_probs = tf.reshape(next_log_probs, shape=[batch_size, -1])
 
-        # Run a while loop till text of length `max_length` has been generated.
-        beams, beams_prob, length, mask = tf.while_loop(
-            cond=lambda beams, beams_prob, length, mask: tf.less(
-                length, max_length
-            ),
-            body=one_step,
-            loop_vars=[beams, beams_prob, length, mask],
-            # There is a strange issue that when `batch_size=1`, the first loop
-            # iteration changes `beams_prob`'s shape from [1, None] to
-            # [None, None], which does not happen for `batch_size>1`.
-            # As a workaround, we set shape invariants.
-            shape_invariants=[
-                beams.get_shape(),
-                tf.TensorShape([None, None]),
-                length.get_shape(),
-                mask.get_shape(),
-            ],
+            # Compute the top beam indices and next tokens.
+            next_log_probs, indices = tf.math.top_k(
+                next_log_probs, k=self.num_beams, sorted=False
+            )
+            beam_indices = indices // vocab_size
+            next_token = flatten_beams(indices % vocab_size)
+            # Ensure shape is `[None]`, otherwise it causes issues after
+            # converting to TFLite.
+            next_token = tf.ensure_shape(next_token, [None])
+            # We need `ensure_shape` as `top_k` will change the static shape.
+            next_log_probs = flatten_beams(next_log_probs)
+            log_probs = tf.ensure_shape(next_log_probs, log_probs.shape)
+
+            def gather_beams(x):
+                x = unflatten_beams(x)
+                x = tf.gather(x, beam_indices, axis=1, batch_dims=1)
+                return flatten_beams(x)
+
+            prompt = gather_beams(prompt)
+            cache = tf.nest.map_structure(gather_beams, cache)
+
+            # Update each beam with the next token.
+            next_token = tf.cast(next_token, prompt.dtype)
+            # Don't overwrite anywhere mask is True.
+            next_token = tf.where(mask[:, index], prompt[:, index], next_token)
+            # Update the prompt with the next token.
+            next_token = next_token[:, tf.newaxis]
+            prompt = dynamic_update_slice(prompt, next_token, [0, index])
+            # Return the iteration of the loop state.
+            return (prompt, cache, index + 1, log_probs)
+
+        prompt, _, _, log_probs = tf.while_loop(
+            cond=cond,
+            body=body,
+            loop_vars=(prompt, cache, index, log_probs),
+            maximum_iterations=(max_length - index),
         )
 
-        # Get the beam with the maximum probability.
-        max_indexes = tf.math.argmax(beams_prob, axis=-1)
-        max_beams = tf.gather(
-            beams, max_indexes[:, tf.newaxis], axis=1, batch_dims=1
-        )
+        all_prompts = unflatten_beams(prompt)
+        all_log_probs = unflatten_beams(log_probs)
 
-        return tf.squeeze(max_beams, axis=1)
+        if self.return_all_beams:
+            sorted_indices = tf.argsort(
+                all_log_probs, axis=-1, direction="DESCENDING"
+            )
+            sorted_log_probs = tf.gather(
+                all_log_probs, sorted_indices, axis=-1, batch_dims=1
+            )
+            sorted_prompts = tf.gather(
+                all_prompts, sorted_indices, axis=1, batch_dims=1
+            )
+            return sorted_prompts, sorted_log_probs
+        else:
+            # Gather the top beam at each batch index.
+            top_beams = tf.math.argmax(all_log_probs, axis=-1)[:, tf.newaxis]
+            prompt = tf.gather(all_prompts, top_beams, axis=1, batch_dims=1)
+            return tf.squeeze(prompt, axis=1)
 
     def get_config(self):
         config = super().get_config()
-
-        config.update({"num_beams": self.num_beams})
+        config.update(
+            {
+                "num_beams": self.num_beams,
+                "return_all_beams": self.return_all_beams,
+            }
+        )
         return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/greedy_sampler.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_k_sampler.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,72 +7,88 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Greedy Sampler."""
+"""Top-k Sampler."""
 
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import base_sampler_args_docstring
 from keras_nlp.samplers.sampler import call_args_docstring
 from keras_nlp.utils.python_utils import format_docstring
 
 
-@format_docstring(
-    base_sampler_args=base_sampler_args_docstring, call_args=call_args_docstring
-)
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class GreedySampler(Sampler):
-    """Greedy sampler class.
-
-    This sampler is implemented on greedy search, i.e., always picking up the
-    token of the largest probability as the next token.
+@format_docstring(call_args=call_args_docstring)
+@keras_nlp_export("keras_nlp.samplers.TopKSampler")
+class TopKSampler(Sampler):
+    """Top-K Sampler class.
+
+    This sampler implements top-k search algorithm. Briefly, top-k algorithm
+    randomly selects a token from the tokens of top K probability, with
+    selection chance determined by the probability.
 
     Args:
-        {{base_sampler_args}}
+        k: int, the `k` value of top-k.
+        seed: int, defaults to None. The random seed.
 
-    Call Args:
+    Call arguments:
         {{call_args}}
 
     Examples:
     ```python
-    VOCAB_SIZE = 10
-
-    # Create a dummy model to predict the next token.
-    model = keras.Sequential(
-        [
-            keras.Input(shape=[None]),
-            keras.layers.Embedding(
-                input_dim=VOCAB_SIZE,
-                output_dim=16,
-            ),
-            keras.layers.Dense(VOCAB_SIZE, activation="softmax"),
-        ]
+    # Use a simple alphabet of lowercase characters with ids in range [0, 25].
+    int_lookup = {i: chr(i + ord('a')) for i in range(26)}
+    char_lookup = {v: k for k, v in int_lookup.items()}
+    batch_size, length, vocab_size = 1, 12, len(int_lookup)
+
+    def next(prompt, cache, index):
+        hidden_states = tf.ones((batch_size, 10))
+        # A uniform distribution over our alphabet.
+        logits = tf.ones((batch_size, vocab_size))
+        return logits, hidden_states, cache
+
+    output = keras_nlp.samplers.TopKSampler(k=3)(
+        next=next,
+        prompt=tf.fill((batch_size, length,), char_lookup['z']),
+        index=5,
     )
-
-    # Define a function that outputs the next token's probability for each token
-    # in the input sequence.
-    def token_probability_fn(inputs, mask):
-        return model(inputs)
-
-    prompt = tf.fill((8, 1), 1)
-
-    sampler = keras_nlp.samplers.GreedySampler()
-    # Print the generated sequence (token ids).
-    print(sampler(prompt, token_probability_fn, max_length=10))
+    print(["".join([int_lookup[i] for i in s]) for s in output.numpy()])
+    # >>> ['zzzzzacbbcaa']
     ```
     """
 
     def __init__(
         self,
-        jit_compile=True,
-        run_eagerly=False,
+        k=5,
+        seed=None,
+        **kwargs,
     ):
-        super().__init__(jit_compile=jit_compile, run_eagerly=run_eagerly)
-
-    def get_next_token(self, next_token_probs):
-        return tf.argmax(next_token_probs, axis=-1)
+        super().__init__(**kwargs)
+        self.k = k
+        self.seed = seed
+
+    def get_next_token(self, probabilities):
+        # Filter out top-k tokens.
+        top_k_pred, top_k_indices = tf.math.top_k(
+            probabilities, k=self.k, sorted=False
+        )
+        # Sample the next token from the probability distribution.
+        next_token = tf.random.categorical(
+            tf.math.log(top_k_pred), 1, seed=self.seed
+        )
+
+        # Rearrange to get the next token idx from the original order.
+        return tf.gather_nd(top_k_indices, next_token, batch_dims=1)
+
+    def get_config(self):
+        config = super().get_config()
+        config.update(
+            {
+                "k": self.k,
+                "seed": self.seed,
+            }
+        )
+        return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_k_sampler.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/random_sampler.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,100 +7,78 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Top-k Sampler."""
+"""Random Sampler."""
 
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import base_sampler_args_docstring
 from keras_nlp.samplers.sampler import call_args_docstring
 from keras_nlp.utils.python_utils import format_docstring
 
 
-@format_docstring(
-    base_sampler_args=base_sampler_args_docstring, call_args=call_args_docstring
-)
-@keras.utils.register_keras_serializable(package="keras_nlp")
-class TopKSampler(Sampler):
-    """Top-K Sampler class.
-
-    This sampler implements top-k search algorithm. Briefly top-k algorithm
-    randomly selects a token from the tokens of top K probability, with
-    selection chance determined by the probability.
+@format_docstring(call_args=call_args_docstring)
+@keras_nlp_export("keras_nlp.samplers.RandomSampler")
+class RandomSampler(Sampler):
+    """Random Sampler class.
+
+    This sampler implements random sampling. Briefly, random sampler randomly
+    selects a token from the entire distribution of the tokens, with selection
+    chance determined by the probability of each token.
 
     Args:
-        k: int, the `k` value of top-k.
         seed: int, defaults to None. The random seed.
-        {{base_sampler_args}}
 
-    Call Args:
+    Call arguments:
         {{call_args}}
 
     Examples:
     ```python
-    VOCAB_SIZE = 10
-
-    # Create a dummy model to predict the next token.
-    model = keras.Sequential(
-        [
-            keras.Input(shape=[None]),
-            keras.layers.Embedding(
-                input_dim=VOCAB_SIZE,
-                output_dim=16,
-            ),
-            keras.layers.Dense(VOCAB_SIZE, activation="softmax"),
-        ]
+    # Use a simple alphabet of lowercase characters with ids in range [0, 25].
+    int_lookup = {i: chr(i + ord('a')) for i in range(26)}
+    char_lookup = {v: k for k, v in int_lookup.items()}
+    batch_size, length, vocab_size = 1, 12, len(int_lookup)
+
+    def next(prompt, state, index):
+        hidden_states = tf.ones((batch_size, 10))
+        # A uniform distribution over our alphabet.
+        logits = tf.ones((batch_size, vocab_size))
+        return logits, hidden_states, state
+
+    output = keras_nlp.samplers.RandomSampler()(
+        next=next,
+        prompt=tf.fill((batch_size, length,), char_lookup['z']),
+        index=5,
     )
-
-    # Define a function that outputs the next token's probability for each token
-    # in the input sequence.
-    def token_probability_fn(inputs, mask):
-        return model(inputs)
-
-    prompt = tf.fill((8, 1), 1)
-
-    sampler = keras_nlp.samplers.TopKSampler(k=5)
-    # Print the generated sequence (token ids).
-    print(sampler(prompt, token_probability_fn, max_length=10))
+    print(["".join([int_lookup[i] for i in s]) for s in output.numpy()])
+    # >>> ['zzzzzcpnjqij']
     ```
     """
 
     def __init__(
         self,
-        k=5,
         seed=None,
-        jit_compile=True,
-        run_eagerly=False,
+        **kwargs,
     ):
-        self.k = k
+        super().__init__(**kwargs)
         self.seed = seed
-        super().__init__(jit_compile=jit_compile, run_eagerly=run_eagerly)
 
-    def get_next_token(self, next_token_probs):
-        # Filter out top-k tokens.
-        top_k_pred, top_k_indices = tf.math.top_k(
-            next_token_probs, k=self.k, sorted=False
-        )
+    def get_next_token(self, probabilities):
         # Sample the next token from the probability distribution.
-        next_token = tf.random.categorical(
-            tf.math.log(top_k_pred), 1, seed=self.seed
+        next_token_id = tf.random.categorical(
+            tf.math.log(probabilities), 1, seed=self.seed, dtype="int32"
         )
-
-        # Rearrange to get the next token idx from the original order.
-        return tf.gather_nd(top_k_indices, next_token, batch_dims=1)
+        return tf.squeeze(next_token_id, axis=-1)
 
     def get_config(self):
         config = super().get_config()
-
         config.update(
             {
-                "k": self.k,
                 "seed": self.seed,
             }
         )
         return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_p_sampler.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,110 +10,110 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Top-p Sampler."""
 
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.samplers.sampler import Sampler
-from keras_nlp.samplers.sampler import base_sampler_args_docstring
 from keras_nlp.samplers.sampler import call_args_docstring
 from keras_nlp.utils.python_utils import format_docstring
 
 
-@format_docstring(
-    base_sampler_args=base_sampler_args_docstring, call_args=call_args_docstring
-)
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@format_docstring(call_args=call_args_docstring)
+@keras_nlp_export("keras_nlp.samplers.TopPSampler")
 class TopPSampler(Sampler):
     """Top-P Sampler class.
 
     This sampler implements top-p search algorithm. Top-p search selects tokens
     from the smallest subset of output probabilities that sum to greater than
     `p`. Put in another way, top-p will first order token predictions by
     likelihood, and ignore all tokens after the cumulative probability of
     selected tokens exceeds `p`, then select a token from the remaining tokens.
 
     Args:
         p: float, the `p` value of top-p.
+        k: int, defaults to None. If set, this argument defines a
+            heuristic "top-k" cutoff applied before the "top-p" sampling. All
+            logits not in the top `k` will be discarded, and the remaining
+            logits will be sorted to find a cutoff point for `p`. Setting this
+            arg can significantly speed sampling up by reducing the number
+            of tokens to sort.
         seed: int, defaults to None. The random seed.
-        {{base_sampler_args}}
 
-    Call Args:
+    Call arguments:
         {{call_args}}
 
     Examples:
     ```python
-    VOCAB_SIZE = 10
-
-    # Create a dummy model to predict the next token.
-    model = keras.Sequential(
-        [
-            keras.Input(shape=[None]),
-            keras.layers.Embedding(
-                input_dim=VOCAB_SIZE,
-                output_dim=16,
-            ),
-            keras.layers.Dense(VOCAB_SIZE, activation="softmax"),
-        ]
+    # Use a simple alphabet of lowercase characters with ids in range [0, 25].
+    int_lookup = {i: chr(i + ord('a')) for i in range(26)}
+    char_lookup = {v: k for k, v in int_lookup.items()}
+    batch_size, length, vocab_size = 1, 12, len(int_lookup)
+
+    def next(prompt, cache, index):
+        hidden_states = tf.ones((batch_size, 10))
+        # A uniform distribution over our alphabet.
+        logits = tf.ones((batch_size, vocab_size))
+        return logits, hidden_states, cache
+
+    output = keras_nlp.samplers.TopPSampler(p=0.1)(
+        next=next,
+        prompt=tf.fill((batch_size, length,), char_lookup['z']),
+        index=5,
     )
-
-    # Define a function that outputs the next token's probability for each token
-    # in the input sequence.
-    def token_probability_fn(inputs, mask):
-        return model(inputs)
-
-    prompt = tf.fill((8, 1), 1)
-
-    sampler = keras_nlp.samplers.TopPSampler(p=0.1)
-    # Print the generated sequence (token ids).
-    print(sampler(prompt, token_probability_fn, max_length=10))
+    print(["".join([int_lookup[i] for i in s]) for s in output.numpy()])
+    # >>> ['zzzzzbabcccb']
     ```
     """
 
     def __init__(
         self,
         p=0.1,
+        k=None,
         seed=None,
-        jit_compile=True,
-        run_eagerly=False,
+        **kwargs,
     ):
+        super().__init__(**kwargs)
         self.p = p
+        self.k = k
         self.seed = seed
-        super().__init__(jit_compile=jit_compile, run_eagerly=run_eagerly)
 
-    def get_next_token(self, next_token_probs):
-        # Sort preds in descending order.
+    def get_next_token(self, probabilities):
+        cutoff = tf.shape(probabilities)[1]
+        if self.k is not None:
+            # If `k` is set, only sample from top `k` tokens.
+            cutoff = tf.math.minimum(cutoff, self.k)
         sorted_preds, sorted_indices = tf.math.top_k(
-            next_token_probs, k=tf.shape(next_token_probs)[1], sorted=True
+            probabilities, k=cutoff, sorted=True
         )
         # Calculate cumulative probability distribution.
-        cumulative_probs = tf.math.cumsum(sorted_preds, axis=-1)
+        cumulative_probabilities = tf.math.cumsum(sorted_preds, axis=-1)
         # Create a mask for the tokens to keep.
-        keep_mask = cumulative_probs <= self.p
+        keep_mask = cumulative_probabilities <= self.p
         # Shift to include the last token that exceed p.
         shifted_keep_mask = tf.concat(
             [tf.ones_like(keep_mask[:, :1]), keep_mask[:, :-1]], axis=-1
         )
         # Filter out unmasked tokens and sample from filtered distribution.
-        probs = tf.where(
+        probabilities = tf.where(
             shifted_keep_mask,
             sorted_preds,
-            tf.zeros(tf.shape(next_token_probs), dtype=sorted_preds.dtype),
+            tf.zeros(tf.shape(sorted_preds), dtype=sorted_preds.dtype),
         )
         sorted_next_token = tf.random.categorical(
-            tf.math.log(probs), 1, seed=self.seed
+            tf.math.log(probabilities), 1, seed=self.seed
         )
         return tf.gather_nd(sorted_indices, sorted_next_token, batch_dims=1)
 
     def get_config(self):
         config = super().get_config()
-
         config.update(
             {
                 "p": self.p,
+                "k": self.k,
                 "seed": self.seed,
             }
         )
         return config
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/samplers/top_p_sampler_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/samplers/top_p_sampler_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,160 +12,143 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for Top-P sampler."""
 
 import numpy as np
 import tensorflow as tf
 from absl.testing import parameterized
-from tensorflow import keras
 
 from keras_nlp.samplers.top_p_sampler import TopPSampler
 
 
 class TopPSamplerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
-        self.vocab_size = 10
-        self.feature_size = 16
+        # Use a simple alphabet of lowercase characters to [0, 26).
+        self.int_lookup = {i: chr(i + ord("a")) for i in range(26)}
+        self.char_lookup = {v: k for k, v in self.int_lookup.items()}
+        self.batch_size = 1
+        self.length = 12
+        self.vocab_size = len(self.int_lookup)
+
+        def next(prompt, cache, index):
+            # Dummy hidden states.
+            hidden_states = tf.ones([self.batch_size, 5])
+            # Return a distribution favoring the next char in cache.
+            logits = tf.one_hot(cache[:, index], self.vocab_size) * 1e9
+            return logits, hidden_states, cache
 
-        # Create a dummy model to predict the next token.
-        model = keras.Sequential(
-            [
-                keras.Input(shape=[None]),
-                keras.layers.Embedding(
-                    input_dim=self.vocab_size,
-                    output_dim=self.feature_size,
-                ),
-                keras.layers.Dense(self.vocab_size),
-                keras.layers.Softmax(),
-            ]
-        )
-
-        def token_probability_fn(inputs, mask):
-            return model(inputs)
-
-        self.token_probability_fn = token_probability_fn
+        self.next = next
         self.sampler = TopPSampler(p=0.1)
 
-    def test_generate_with_1d_prompt(self):
-        inputs = tf.constant([1])
+    def join_as_string(self, x):
+        return ["".join([self.int_lookup[i] for i in s]) for s in x.numpy()]
 
-        outputs = self.sampler(inputs, self.token_probability_fn, max_length=5)
-        self.assertEqual(outputs.shape, [5])
+    def test_stateless_call(self):
+        def next(prompt, cache, index):
+            # Dummy hidden states.
+            hidden_states = tf.ones([self.batch_size, 5])
+            # Return a distribution favoring the first token in the vocab.
+            logits = (
+                tf.one_hot(
+                    tf.zeros(self.batch_size, dtype=tf.int32),
+                    self.vocab_size,
+                )
+                * 1e9
+            )
+            return logits, hidden_states, cache
 
-    def test_generate_with_2d_prompt(self):
-        inputs = tf.constant([[1], [1]])
-        outputs = self.sampler(inputs, self.token_probability_fn, max_length=5)
-        self.assertEqual(outputs.shape, [2, 5])
-
-    def test_generate_with_list_prompt(self):
-        inputs = [[1], [1]]
-        outputs = self.sampler(inputs, self.token_probability_fn, max_length=5)
-        self.assertEqual(outputs.shape, [2, 5])
-
-    def test_generate_with_ragged_prompt(self):
-        def token_probability_fn(inputs, mask):
-            batch_size, seq_length = tf.shape(inputs)[0], tf.shape(inputs)[1]
-            prob = tf.constant([[[0.0, 0.0, 0.0, 1.0]]])
-            return tf.tile(prob, [batch_size, seq_length, 1])
-
-        inputs = tf.ragged.constant([[1], [2, 1, 2]])
-        outputs = self.sampler(
-            inputs,
-            token_probability_fn,
-            max_length=5,
-            from_logits=False,
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+        output = self.sampler(
+            next=next,
+            prompt=prompt,
+            index=5,
+        )
+        self.assertEqual(self.join_as_string(output), ["zzzzzaaaaaaa"])
+
+    def test_stateful_call(self):
+        cache_chars = list("sequentially")
+        cache = tf.constant([[self.char_lookup[c] for c in cache_chars]])
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+        output = self.sampler(
+            next=self.next,
+            prompt=prompt,
+            cache=cache,
+        )
+        self.assertEqual(self.join_as_string(output), ["sequentially"])
+
+    def test_early_stopping(self):
+        cache_chars = list("sequentially")
+        cache = tf.constant([[self.char_lookup[c] for c in cache_chars]])
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+        output = self.sampler(
+            next=self.next,
+            prompt=prompt,
+            cache=cache,
+            end_token_id=self.char_lookup["t"],
+        )
+        self.assertEqual(self.join_as_string(output), ["sequentzzzzz"])
+
+    def test_only_sample_from_top_k_tokens(self):
+        def next(prompt, cache, index):
+            # Dummy hidden states.
+            hidden_states = tf.ones([self.batch_size, 5])
+            # Return a distribution where each id is progressively less likely.
+            logits = tf.range(self.vocab_size, 0, -1, dtype="float32")
+            logits = tf.repeat(logits[tf.newaxis, :], self.batch_size, axis=0)
+            return logits, hidden_states, cache
+
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+        output = TopPSampler(p=1, k=5)(
+            next=next,
+            prompt=prompt,
+            index=5,
+        )
+        generated_str = self.join_as_string(output[:, 5:])[0]
+        token_set = set(generated_str)
+        self.assertContainsSubset(token_set, set("abcde"))
+
+    def test_outputs_in_top_p(self):
+        def next(prompt, cache, index):
+            # Dummy hidden states.
+            hidden_states = tf.ones([self.batch_size, 5])
+            logits = np.zeros((self.batch_size, self.vocab_size))
+            return tf.constant(logits), hidden_states, cache
+
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+        output = TopPSampler(p=(2.0 / self.vocab_size))(
+            next=next,
+            prompt=prompt,
+        )
+        output_ids = set(output[0].numpy())
+        self.assertContainsSubset(output_ids, range(3))
+
+    def test_temperature(self):
+        def next(prompt, cache, index):
+            # Dummy hidden states.
+            hidden_states = tf.ones([self.batch_size, 5])
+            logits = tf.range(self.vocab_size, 0, -1, dtype=tf.float32)
+            logits = tf.reshape(logits[tf.newaxis, :], (self.batch_size, -1))
+            return tf.constant(logits), hidden_states, cache
+
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+
+        output = TopPSampler(p=0.5, temperature=1e-9)(
+            next=next,
+            prompt=prompt,
         )
-        self.assertEqual(outputs.shape, [2, 5])
+        self.assertAllEqual(output, tf.zeros_like(output))
 
     @parameterized.named_parameters(
-        ("xla_graph", True, False),
-        ("non_xla_graph", False, False),
-        ("eager", False, True),
+        ("jit_compile_false", False), ("jit_compile_true", True)
     )
-    def test_assert_probability_distribution_generation_is_correct(
-        self, jit_compile, run_eagerly
-    ):
-        def token_probability_fn(inputs, mask):
-            batch_size, seq_length = tf.shape(inputs)[0], tf.shape(inputs)[1]
-            prob = tf.constant([[[0.0, 0.0, 0.0, 1.0]]])
-            return tf.tile(prob, [batch_size, seq_length, 1])
-
-        batch_size = 10
-        inputs = 3 * tf.ones([batch_size, 1], dtype=tf.int32)
-        max_length = 3
-
-        outputs_count = np.array([0, 0, 0, 0])
-        tf.random.set_seed(42)
-        sampler = TopPSampler(
-            p=0.1,
-            seed=42,
-            run_eagerly=jit_compile,
-            jit_compile=run_eagerly,
-        )
-        for _ in range(8):
-            outputs = sampler(
-                inputs,
-                token_probability_fn,
-                max_length=max_length,
-                from_logits=False,
-            )
-            flatten_predictions = tf.reshape(outputs[:, 1:], [-1])
-            for pred in flatten_predictions:
-                outputs_count[pred] += 1
-        self.assertAllClose(
-            outputs_count / np.sum(outputs_count),
-            [0.0, 0.0, 0.0, 1.0],
-            rtol=0.2,
-        )
-
-    def test_only_choose_from_top_p_tokens(self):
-        # Test that there are only the top-p tokens in the output.
-        def token_probability_fn(inputs, mask):
-            batch_size, seq_length = tf.shape(inputs)[0], tf.shape(inputs)[1]
-            prob = tf.constant([[[0.4, 0.3, 0.2, 0.1]]])
-            return tf.tile(prob, [batch_size, seq_length, 1])
-
-        # Test that it only samples from top-p tokens.
-        for i, p in enumerate([0.399, 0.699, 0.899]):
-            inputs = tf.constant([[0, 0], [0, 0]])
-            sampler = TopPSampler(p=p)
-            for _ in range(10):
-                outputs = sampler(
-                    inputs,
-                    token_probability_fn,
-                    max_length=5,
-                    from_logits=False,
-                )
-                self.assertAllEqual(outputs <= i, tf.ones_like(outputs))
+    def test_compilation(self, jit_compile):
+        cache_chars = list("sequentially")
+        cache = tf.constant([[self.char_lookup[c] for c in cache_chars]])
+        prompt = tf.fill((self.batch_size, self.length), self.char_lookup["z"])
+
+        @tf.function(jit_compile=jit_compile)
+        def generate(prompt, cache):
+            return self.sampler(self.next, prompt=prompt, cache=cache)
 
-    def test_end_token_id(self):
-        def token_probability_fn(inputs, mask):
-            batch_size, seq_length = tf.shape(inputs)[0], tf.shape(inputs)[1]
-            prob = tf.constant([[[0.0, 0.0, 0.0, 1.0]]])
-            return tf.tile(prob, [batch_size, seq_length, 1])
-
-        tf.random.set_seed(42)
-        sampler = TopPSampler(p=0.1, seed=42)
-        max_length = 4
-        inputs = tf.constant([[0, 1], [1, 2]])
-        outputs = sampler(
-            inputs,
-            token_probability_fn,
-            max_length=max_length,
-            end_token_id=2,
-            from_logits=False,
-        )
-        # end_token in prompt does not trigger truncation.
-        expected_outputs = tf.ragged.constant([[0, 1, 3, 3], [1, 2, 3, 3]])
-        self.assertAllEqual(outputs, expected_outputs)
-
-        outputs = sampler(
-            inputs,
-            token_probability_fn,
-            max_length=max_length,
-            end_token_id=3,
-            from_logits=False,
-        )
-        # Generated end_token will be truncated.
-        expected_outputs = tf.ragged.constant([[0, 1], [1, 2]])
-        self.assertAllEqual(outputs, expected_outputs)
+        output = generate(prompt, cache)
+        self.assertEqual(self.join_as_string(output), ["sequentially"])
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/docstring_lib.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/docstring_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/docstring_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,144 +8,147 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import doctest
-import io
-import os
-import sys
-import unittest
-
-import numpy as np
-import pytest
-import sentencepiece
-import tensorflow as tf
-from tensorflow import keras
+"""DeBERTa tokenizer."""
+
+import copy
 
-import keras_nlp
-from keras_nlp.tests.doc_tests import docstring_lib
-from keras_nlp.tests.doc_tests import fenced_docstring_lib
-from keras_nlp.tests.doc_tests.fenced_docstring_lib import (
-    astor,  # For checking conditional import.
-)
-
-PACKAGE = "keras_nlp."
-
-
-def find_modules():
-    keras_nlp_modules = []
-    for name, module in sys.modules.items():
-        if name.startswith(PACKAGE):
-            keras_nlp_modules.append(module)
-
-    return keras_nlp_modules
-
-
-def test_docstrings():
-    keras_nlp_modules = find_modules()
-    # As of this writing, it doesn't seem like pytest support load_tests
-    # protocol for unittest:
-    #     https://docs.pytest.org/en/7.1.x/how-to/unittest.html
-    # So we run the unittest.TestSuite manually and report the results back.
-    runner = unittest.TextTestRunner()
-    suite = unittest.TestSuite()
-    for module in keras_nlp_modules:
-        # Stop testing some docstrings until we are exporting the symbols.
-        if [name in module.__name__ for name in ["bart", "gpt2", "opt"]]:
-            continue
-        suite.addTest(
-            doctest.DocTestSuite(
-                module,
-                test_finder=doctest.DocTestFinder(exclude_empty=False),
-                extraglobs={
-                    "tf": tf,
-                    "np": np,
-                    "os": os,
-                    "keras": keras,
-                    "keras_nlp": keras_nlp,
-                },
-                checker=docstring_lib.DoctestOutputChecker(),
-                optionflags=(
-                    doctest.ELLIPSIS
-                    | doctest.NORMALIZE_WHITESPACE
-                    | doctest.IGNORE_EXCEPTION_DETAIL
-                    | doctest.DONT_ACCEPT_BLANKLINE
-                ),
-            )
-        )
-    result = runner.run(suite)
-    if not result.wasSuccessful():
-        print(result)
-    assert result.wasSuccessful()
-
-
-@pytest.mark.extra_large
-@pytest.mark.skipif(
-    astor is None,
-    reason="This test requires `astor`. Please `pip install astor` to run.",
-)
-def test_fenced_docstrings():
-    """Tests fenced code blocks in docstrings.
+import tensorflow as tf
 
-    This can only be run manually. Run with:
-    `pytest keras_nlp/tests/doc_tests/docstring_test.py --run_extra_large`
+from keras_nlp.api_export import keras_nlp_export
+from keras_nlp.models.deberta_v3.deberta_v3_presets import backbone_presets
+from keras_nlp.tokenizers.sentence_piece_tokenizer import SentencePieceTokenizer
+from keras_nlp.utils.python_utils import classproperty
+
+
+@keras_nlp_export("keras_nlp.models.DebertaV3Tokenizer")
+class DebertaV3Tokenizer(SentencePieceTokenizer):
+    """DeBERTa tokenizer layer based on SentencePiece.
+
+    This tokenizer class will tokenize raw strings into integer sequences and
+    is based on `keras_nlp.tokenizers.SentencePieceTokenizer`. Unlike the
+    underlying tokenizer, it will check for all special tokens needed by
+    DeBERTa models and provides a `from_preset()` method to automatically
+    download a matching vocabulary for a DeBERTa preset.
+
+    This tokenizer does not provide truncation or padding of inputs. It can be
+    combined with a `keras_nlp.models.DebertaV3Preprocessor` layer for input
+    packing.
+
+    If input is a batch of strings (rank > 0), the layer will output a
+    `tf.RaggedTensor` where the last dimension of the output is ragged.
+
+    If input is a scalar string (rank == 0), the layer will output a dense
+    `tf.Tensor` with static shape `[None]`.
+
+    Note: The mask token (`"[MASK]"`) is handled differently in this tokenizer.
+    If the token is not present in the provided SentencePiece vocabulary, the
+    token will be appended to the vocabulary. For example, if the vocabulary
+    size is 100, the mask token will be assigned the ID 100.
+
+    Args:
+        proto: Either a `string` path to a SentencePiece proto file, or a
+            `bytes` object with a serialized SentencePiece proto. See the
+            [SentencePiece repository](https://github.com/google/sentencepiece)
+            for more details on the format.
+
+    Examples:
+
+    ```python
+    # Unbatched input.
+    tokenizer = keras_nlp.models.DebertaV3Tokenizer.from_preset(
+        "deberta_v3_base_en",
+    )
+    tokenizer("The quick brown fox jumped.")
+
+    # Batched inputs.
+    tokenizer(["the quick brown fox", "the earth is round"])
+
+    # Detokenization.
+    tokenizer.detokenize(tokenizer("The quick brown fox jumped."))
+
+    # Custom vocabulary.
+    bytes_io = io.BytesIO()
+    ds = tf.data.Dataset.from_tensor_slices(["The quick brown fox jumped."])
+    sentencepiece.SentencePieceTrainer.train(
+        sentence_iterator=ds.as_numpy_iterator(),
+        model_writer=bytes_io,
+        vocab_size=9,
+        model_type="WORD",
+        pad_id=0,
+        bos_id=1,
+        eos_id=2,
+        unk_id=3,
+        pad_piece="[PAD]",
+        bos_piece="[CLS]",
+        eos_piece="[SEP]",
+        unk_piece="[UNK]",
+    )
+    tokenizer = keras_nlp.models.DebertaV3Tokenizer(
+        proto=bytes_io.getvalue(),
+    )
+    tokenizer("The quick brown fox jumped.")
+    ```
     """
-    keras_nlp_modules = find_modules()
 
-    runner = unittest.TextTestRunner()
-    suite = unittest.TestSuite()
-    for module in keras_nlp_modules:
-        # Stop testing some docstrings until we are exporting the symbols.
-        if [name in module.__name__ for name in ["bart", "gpt2", "opt"]]:
-            continue
-        # Do not test certain modules.
-        if module.__name__ in [
-            # Base classes.
-            "keras_nlp.models.backbone",
-            "keras_nlp.models.preprocessor",
-            "keras_nlp.models.task",
-            # Preprocessors and tokenizers which use `model.spm` (temporary).
-            "keras_nlp.models.albert.albert_preprocessor",
-            "keras_nlp.models.albert.albert_tokenizer",
-            "keras_nlp.models.xlm_roberta.xlm_roberta_preprocessor",
-            "keras_nlp.models.f_net.f_net_preprocessor",
-            "keras_nlp.models.f_net.f_net_tokenizer",
-        ]:
-            continue
-
-        suite.addTest(
-            doctest.DocTestSuite(
-                module,
-                test_finder=doctest.DocTestFinder(
-                    exclude_empty=False,
-                    parser=fenced_docstring_lib.FencedCellParser(
-                        fence_label="python"
-                    ),
-                ),
-                globs={
-                    "_print_if_not_none": fenced_docstring_lib._print_if_not_none
-                },
-                extraglobs={
-                    "tf": tf,
-                    "np": np,
-                    "os": os,
-                    "keras": keras,
-                    "keras_nlp": keras_nlp,
-                    "io": io,
-                    "sentencepiece": sentencepiece,
-                },
-                checker=docstring_lib.DoctestOutputChecker(),
-                optionflags=(
-                    doctest.ELLIPSIS
-                    | doctest.NORMALIZE_WHITESPACE
-                    | doctest.IGNORE_EXCEPTION_DETAIL
-                    | doctest.DONT_ACCEPT_BLANKLINE
-                ),
-            )
-        )
-    result = runner.run(suite)
-    if not result.wasSuccessful():
-        print(result)
-    assert result.wasSuccessful()
+    def __init__(self, proto, **kwargs):
+        super().__init__(proto=proto, **kwargs)
+
+        # Check for necessary special tokens.
+        cls_token = "[CLS]"
+        sep_token = "[SEP]"
+        pad_token = "[PAD]"
+        mask_token = "[MASK]"
+
+        # We do not throw an error if `mask_token` is not present in the
+        # vocabulary.
+        for token in [cls_token, pad_token, sep_token]:
+            if token not in super().get_vocabulary():
+                raise ValueError(
+                    f"Cannot find token `'{token}'` in the provided "
+                    f"`vocabulary`. Please provide `'{token}'` in your "
+                    "`vocabulary` or use a pretrained `vocabulary` name."
+                )
+
+        self.cls_token_id = self.token_to_id(cls_token)
+        self.sep_token_id = self.token_to_id(sep_token)
+        self.pad_token_id = self.token_to_id(pad_token)
+        # If the mask token is not in the vocabulary, add it to the end of the
+        # vocabulary.
+        if mask_token in super().get_vocabulary():
+            self.mask_token_id = super().token_to_id(mask_token)
+        else:
+            self.mask_token_id = super().vocabulary_size()
+
+    def vocabulary_size(self):
+        sentence_piece_size = super().vocabulary_size()
+        if sentence_piece_size == self.mask_token_id:
+            return sentence_piece_size + 1
+        return sentence_piece_size
+
+    def get_vocabulary(self):
+        sentence_piece_vocabulary = super().get_vocabulary()
+        if self.mask_token_id < super().vocabulary_size():
+            return sentence_piece_vocabulary
+        return sentence_piece_vocabulary + ["[MASK]"]
+
+    def id_to_token(self, id):
+        if id == self.mask_token_id:
+            return "[MASK]"
+        return super().id_to_token(id)
+
+    def token_to_id(self, token):
+        if token == "[MASK]":
+            return self.mask_token_id
+        return super().token_to_id(token)
+
+    def detokenize(self, ids):
+        ids = tf.ragged.boolean_mask(ids, tf.not_equal(ids, self.mask_token_id))
+        return super().detokenize(ids)
+
+    @classproperty
+    def presets(cls):
+        return copy.deepcopy(backbone_presets)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/fenced_docstring_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,19 @@
         self, string: str, name: str = "<string>"
     ) -> List[doctest.Example]:
         tests = []
         for match in self.fence_cell_re.finditer(string):
             if re.search("doctest.*skip", match.group(0), re.IGNORECASE):
                 continue
 
+            # Do not test any docstring with our format string markers.
+            # These will not run until formatted.
+            if re.search("{{", match.group(0)):
+                continue
+
             groups = match.groupdict()
 
             source = textwrap.dedent(groups["doctest"])
             want = groups["output"]
             if want is not None:
                 want = textwrap.dedent(want)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/__init__.py` & `keras-nlp-0.5.0.dev0/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/basic_usage_test.py` & `keras-nlp-0.5.0.dev0/integration_tests/basic_usage_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tests/integration_tests/import_test.py` & `keras-nlp-0.5.0.dev0/integration_tests/import_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 """
 
 import json
 import os
 from typing import Iterable
 from typing import List
 
+import regex as re
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.tokenizers import tokenizer
 from keras_nlp.utils.python_utils import classproperty
 from keras_nlp.utils.python_utils import format_docstring
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
@@ -46,17 +48,28 @@
     r"'s|'t|'re|'ve|'m|'ll|'d"
     + r"|[\s{special_spaces}]+[\n\r\t\f६{special_spaces}]| ?\p{L}+|"
     + r" ?[\p{N}]+| ?[^\s\p{L}\p{N}{special_spaces}]+"
 )
 SPLIT_PATTERN_1 = SPLIT_PATTERN_1.replace(
     "{special_spaces}", SPECIAL_WHITESPACES
 )
+SPLIT_PATTERN_2 = rf"""[\s६{SPECIAL_WHITESPACES}]$"""
 
 
-SPLIT_PATTERN_2 = rf"""[\s६{SPECIAL_WHITESPACES}]$"""
+def create_alts_for_unsplittable_tokens(unsplittable_tokens):
+    # Create alternates for all special tokens that will be not split during
+    # tokenization.
+    alts = []
+    prefix = "Ĵ"
+    # Trim out splitters.
+    replace_pattern = r"'|\s+|[^\p{L}\p{N}]+"
+    for token in unsplittable_tokens:
+        token = re.sub(replace_pattern, "", token)
+        alts.append(prefix + token)
+    return alts
 
 
 def bytes_to_unicode():
     bs = (
         list(range(ord("!"), ord("~") + 1))
         + list(range(ord("¡"), ord("¬") + 1))
         + list(range(ord("®"), ord("ÿ") + 1))
@@ -83,32 +96,45 @@
     result = tf.RaggedTensor.from_row_lengths(
         values=flatten_result,
         row_lengths=row_lengths,
     )
     return result
 
 
-def split_strings_for_bpe(inputs):
+def split_strings_for_bpe(inputs, unsplittable_tokens=None):
     # We need to recreate the exact behavior of token presplitting in the
     # original gpt2 tokenizer which uses a lookahead. As re2 does not
     # support lookahead match, we are using an alternative insert a special
     # token "६" before leading space of non-space characters and after the
     # trailing space, e.g., " keras" will be "६ keras".
     inputs = tf.strings.regex_replace(
         inputs, rf"( )([^\s{SPECIAL_WHITESPACES}])", r"६\1\2"
     )
     inputs = tf.strings.regex_replace(
         inputs, rf"(\s{SPECIAL_WHITESPACES})$", r"\1६"
     )
+    if unsplittable_tokens:
+        alts = create_alts_for_unsplittable_tokens(unsplittable_tokens)
+        for token, alt in zip(unsplittable_tokens, alts):
+            escaped_token = re.escape(token)
+            inputs = tf_text.regex_split(inputs, escaped_token, escaped_token)
+            inputs = tf.strings.regex_replace(inputs, escaped_token, alt)
     raw_tokens = tf_text.regex_split(inputs, SPLIT_PATTERN_1, SPLIT_PATTERN_1)
     # Second pass splits out the last whilespace char or "६".
     raw_tokens = tf_text.regex_split(
         raw_tokens, SPLIT_PATTERN_2, SPLIT_PATTERN_2
     )
-    if raw_tokens.shape.rank > 2:
+    if unsplittable_tokens:
+        # Replace special tokens alternate with originals.
+        for token, alt in zip(unsplittable_tokens, alts):
+            escaped_alt = re.escape(alt)
+            raw_tokens = tf.strings.regex_replace(
+                raw_tokens, escaped_alt, token
+            )
+    while raw_tokens.shape.rank > 2:
         raw_tokens = raw_tokens.merge_dims(1, 2)
     return remove_strings_from_inputs(raw_tokens, "६")
 
 
 class BytePairTokenizerCache(tf.Module):
     """Cache that stores the encoded result of seen tokens.
 
@@ -123,15 +149,17 @@
     ```
     """
 
     def __init__(self):
         # `tf.lookup.experimental.MutableHashTable` does not support string to
         # string mapping. So we first convert to string to an integer key, and
         # use the integer key to find the value.
-        self.factors = tf.pow(256, tf.range(0, 8, dtype=tf.int64))
+        self.factors = tf.pow(
+            tf.constant(256, dtype=tf.int64), tf.range(0, 8, dtype=tf.int64)
+        )
         self.id2value = tf.lookup.experimental.MutableHashTable(
             tf.int64, tf.string, ""
         )
 
     def _get_key(self, keys):
         """Get the hash key for given inputs."""
         # `tf.fingerprint` converts token to a array of uint8 of length 8, we
@@ -163,15 +191,15 @@
             tf.convert_to_tensor(keys),
             tf.convert_to_tensor(values),
         ),
         default_value=default,
     )
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.tokenizers.BytePairTokenizer")
 class BytePairTokenizer(tokenizer.Tokenizer):
     """Bype-pair encoding tokenizer layer.
 
     This BPE tokenizer provides the same functionality as the official GPT-2
     tokenizer. Given the same `vocabulary` which maps tokens to ids, and `merges`
     which describes BPE merge rules, it should provide the same output
     as OpenAI implementation (https://github.com/openai/gpt-2/blob/master/src/encoder.py).
@@ -197,14 +225,20 @@
         sequence_length: int, defaults to None. If set, the output will be
             padded or truncated to the `sequence_length`.
         add_prefix_space: bool, defaults to False. Whether or not to add an
             initial space to the input. This tokenizer is whitespace aware,
             and will tokenize a word with a leading space differently. Adding
             a prefix space to the first word will cause it to be tokenized
             equivalently to all subsequent words in the sequence.
+        unsplittable_tokens: list, defaults to None. A list of strings that will
+            never be split during the word-level splitting applied before the
+            byte-pair encoding. This can be used to ensure special tokens map to
+            unique indices in the vocabulary, even if these special tokens
+            contain splittable characters such as punctuation. Special tokens
+            must still be included in `vocabulary`.
 
     Examples:
 
     Tokenize
     >>> vocab = {"butter": 1, "fly": 2}
     >>> merge = ["b u", "t t", "e r", "bu tt", "butt er", "f l", "fl y"]
     >>> tokenizer = keras_nlp.tokenizers.BytePairTokenizer(vocab, merge)
@@ -232,14 +266,15 @@
 
     def __init__(
         self,
         vocabulary,
         merges,
         sequence_length=None,
         add_prefix_space=False,
+        unsplittable_tokens=None,
         **kwargs,
     ) -> None:
         assert_tf_text_installed(self.__class__.__name__)
 
         # Check dtype and provide a default.
         if "dtype" not in kwargs or kwargs["dtype"] is None:
             kwargs["dtype"] = tf.int32
@@ -271,26 +306,31 @@
         else:
             raise ValueError(
                 "Merges must be a file path or a list of merge rules. "
                 f"Received: `type(merges)={type(merges)}`"
             )
         self.sequence_length = sequence_length
         self.add_prefix_space = add_prefix_space
+        self.unsplittable_tokens = unsplittable_tokens
 
         # Create byte <=> unicode mapping. This is useful for handling
         # whitespace tokens.
         byte_list, unicode_list = bytes_to_unicode()
         self.byte2unicode = create_static_hashtable(
             byte_list, unicode_list, default=""
         )
         self.unicode2byte = create_static_hashtable(
             unicode_list, byte_list, default=""
         )
 
         self.cache = BytePairTokenizerCache()
+        if unsplittable_tokens:
+            # Put special tokens into cache, so it won't be further split and
+            # merged.
+            self.cache.insert(unsplittable_tokens, unsplittable_tokens)
 
         # Create mapping between string tokens to int ids, and vice versa.
         byte_pairs = [x[0] for x in self.vocabulary.items()]
         byte_pair_encoding_indices = [x[1] for x in self.vocabulary.items()]
         self.token_to_id_map = create_static_hashtable(
             byte_pairs,
             byte_pair_encoding_indices,
@@ -341,14 +381,16 @@
             {
                 # Ideally vocabulary and merge list would be saved as plain text
                 # assets in the saved model. We have no good way to support
                 # this currently, so we save the vocabulary in the config.
                 "vocabulary": self.vocabulary,
                 "merges": self.merges,
                 "sequence_length": self.sequence_length,
+                "add_prefix_space": self.add_prefix_space,
+                "unsplittable_tokens": self.unsplittable_tokens,
             }
         )
         return config
 
     @tf.function
     def _bpe_merge_one_step(self, words, mask):
         """Perform one step of byte-pair merge."""
@@ -461,15 +503,15 @@
         if self.add_prefix_space:
             inputs = tf.strings.join([" ", inputs])
 
         scalar_input = inputs.shape.rank == 0
         if scalar_input:
             inputs = tf.expand_dims(inputs, 0)
 
-        raw_tokens = split_strings_for_bpe(inputs)
+        raw_tokens = split_strings_for_bpe(inputs, self.unsplittable_tokens)
         token_row_splits = raw_tokens.row_splits
         flat_tokens = raw_tokens.flat_values
 
         # Check cache.
         cache_lookup = self.cache.lookup(flat_tokens)
         cache_mask = cache_lookup == ""
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_pair_tokenizer_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 )
 
 
 @pytest.mark.large
 class BytePairTokenizerTest(tf.test.TestCase, parameterized.TestCase):
     def setUp(self):
         super().setUp()
-
         self.tokenizer = BytePairTokenizer(
             vocabulary=VOCAB_PATH, merges=MERGE_PATH
         )
 
     def test_tokenize_list_input(self):
         input_data = ["brown.", "black."]
         call_output = self.tokenizer(input_data)
@@ -62,14 +61,33 @@
             [
                 ["quick", "Ġbrown", "Ġfox", "."],
                 ["slow", "Ġblack", "Ġbear", "."],
             ]
         )
         self.assertAllEqual(call_output, expected)
 
+    def test_tokenize_with_special_tokens(self):
+        vocab = {"sp": 0, "s": 1, "p": 2}
+        merges = ["s p"]
+        tokenizer = BytePairTokenizer(
+            vocabulary=vocab,
+            merges=merges,
+            unsplittable_tokens=["s", "p"],
+        )
+        output = tokenizer("sp")
+        self.assertAllEqual(output, [1, 2])
+
+        # If not setting special tokens, "sp" is one token.
+        tokenizer = BytePairTokenizer(
+            vocabulary=vocab,
+            merges=merges,
+        )
+        output = tokenizer("sp")
+        self.assertEqual(output, [0])
+
     def test_tokenize_prefix_space(self):
         input_data = ["brown.", "black."]
         tokenizer = BytePairTokenizer(
             vocabulary=VOCAB_PATH,
             merges=MERGE_PATH,
             dtype=tf.string,
             add_prefix_space=True,
@@ -160,13 +178,15 @@
     def test_saved_model(self, save_format, filename):
         input_data = tf.constant(["the quick brown whale."])
         tokenizer = self.tokenizer
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Byte Tokenizer."""
 
 import numpy as np
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.tokenizers import tokenizer
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.tokenizers.ByteTokenizer")
 class ByteTokenizer(tokenizer.Tokenizer):
     """Raw byte tokenizer.
 
     This tokenizer is a vocabulary-free tokenizer which will tokenize text as
     as raw bytes from [0, 256).
 
     Tokenizer outputs can either be padded and truncated with a
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/byte_tokenizer_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,13 +257,15 @@
             normalization_form="NFKC",
             errors="replace",
         )
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 import binascii
 import os
 from typing import List
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.tokenizers import tokenizer
 from keras_nlp.utils.python_utils import classproperty
 from keras_nlp.utils.python_utils import format_docstring
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 from keras_nlp.utils.tf_utils import tensor_to_string_list
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.tokenizers.SentencePieceTokenizer")
 class SentencePieceTokenizer(tokenizer.Tokenizer):
     """A SentencePiece tokenizer layer.
 
     This layer provides an implementation of SentencePiece tokenization
     as described in the [SentencePiece paper](https://arxiv.org/abs/1808.06226)
     and the [SentencePiece package](https://pypi.org/project/sentencepiece/).
     The tokenization will run entirely within the Tensorflow graph, and can
@@ -155,17 +156,19 @@
         self.sequence_length = sequence_length
 
     def vocabulary_size(self) -> int:
         """Get the size of the tokenizer vocabulary."""
         return int(self._sentence_piece.vocab_size().numpy())
 
     def get_vocabulary(self) -> List[str]:
-        """Get the size of the tokenizer vocabulary."""
+        """Get the tokenizer vocabulary."""
         return tensor_to_string_list(
-            self._sentence_piece.id_to_string(tf.range(self.vocabulary_size()))
+            self._sentence_piece.id_to_string(
+                tf.range(int(self._sentence_piece.vocab_size().numpy()))
+            )
         )
 
     def id_to_token(self, id: int) -> str:
         """Convert an integer id to a string token."""
         return tensor_to_string_list(self._sentence_piece.id_to_string(id))
 
     def token_to_id(self, token: str) -> int:
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,13 +197,15 @@
         tokenizer = SentencePieceTokenizer(
             proto=filepath,
         )
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/sentence_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+
+@keras_nlp_export("keras_nlp.tokenizers.Tokenizer")
 class Tokenizer(keras.layers.Layer):
     """A base class for tokenizer layers.
 
     Tokenizers in the KerasNLP library should all subclass this layer.
     The class provides two core methods `tokenize()` and `detokenize()` for
     going from plain text to sequences and back. A tokenizer is a subclass of
     `keras.layers.Layer` and can be combined into a `keras.Model`.
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
-from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.tokenizers import tokenizer
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
 except ImportError:
     tf_text = None
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.tokenizers.UnicodeCodepointTokenizer")
 class UnicodeCodepointTokenizer(tokenizer.Tokenizer):
     """A unicode character tokenizer layer.
 
     This tokenizer is a vocabulary free tokenizer which tokenizes text as
     unicode character codepoints.
 
     Tokenizer outputs can either be padded and truncated with a
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/unicode_codepoint_tokenizer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,13 +359,15 @@
             errors="replace",
             vocabulary_size=None,
         )
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 from typing import Iterable
 from typing import List
 
 import tensorflow as tf
 from tensorflow import keras
 
+from keras_nlp.api_export import keras_nlp_export
 from keras_nlp.tokenizers import tokenizer
 from keras_nlp.utils.python_utils import classproperty
 from keras_nlp.utils.python_utils import format_docstring
 from keras_nlp.utils.tf_utils import assert_tf_text_installed
 
 try:
     import tensorflow_text as tf_text
@@ -151,15 +152,15 @@
             text,
             delim_regex_pattern=split_pattern,
             keep_delim_regex_pattern=keep_split_pattern,
         )
     return text
 
 
-@keras.utils.register_keras_serializable(package="keras_nlp")
+@keras_nlp_export("keras_nlp.tokenizers.WordPieceTokenizer")
 class WordPieceTokenizer(tokenizer.Tokenizer):
     """A WordPiece tokenizer layer.
 
     This layer provides an efficient, in graph, implementation of the WordPiece
     algorithm used by BERT and other models.
 
     To make this layer more useful out of the box, the layer will pre-tokenize
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,17 @@
             suffix_indicator="@@",
             dtype="string",
         )
         inputs = keras.Input(dtype="string", shape=())
         outputs = tokenizer(inputs)
         model = keras.Model(inputs, outputs)
         path = os.path.join(self.get_temp_dir(), filename)
-        model.save(path, save_format=save_format)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(path)
         self.assertAllEqual(
             model(input_data),
             restored_model(input_data),
         )
 
     def test_no_oov_token_in_vocabulary(self):
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tokenizers/word_piece_tokenizer_trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/keras_utils_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/keras_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/pipeline_model.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/pipeline_model_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/pipeline_model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,18 +136,20 @@
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model = NoopPipeline()
         x = tf.random.uniform((8, 5))
         model_output = model.predict(x)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        model.save(save_path, save_format=save_format)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(
-            save_path, custom_objects={"NoopPipeline": NoopPipeline}
+            path, custom_objects={"NoopPipeline": NoopPipeline}
         )
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, NoopPipeline)
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
@@ -252,18 +254,20 @@
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model = FeaturePipeline()
         x = tf.strings.as_string(tf.random.uniform((8, 5)))
         model_output = model.predict(x)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        model.save(save_path, save_format=save_format)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(
-            save_path, custom_objects={"FeaturePipeline": FeaturePipeline}
+            path, custom_objects={"FeaturePipeline": FeaturePipeline}
         )
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, FeaturePipeline)
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
@@ -361,18 +365,20 @@
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model = LabelPipeline()
         x = tf.random.uniform((8, 5))
         model_output = model.predict(x)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        model.save(save_path, save_format=save_format)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(
-            save_path, custom_objects={"LabelPipeline": LabelPipeline}
+            path, custom_objects={"LabelPipeline": LabelPipeline}
         )
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, LabelPipeline)
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
@@ -453,18 +459,20 @@
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model = DataPipeline()
         data = tf.strings.as_string(tf.random.uniform((8, 1)))
         model_output = model.predict(data)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        model.save(save_path, save_format=save_format)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(
-            save_path, custom_objects={"DataPipeline": DataPipeline}
+            path, custom_objects={"DataPipeline": DataPipeline}
         )
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, DataPipeline)
         # Check that output matches.
         restored_output = restored_model.predict(data)
         self.assertAllClose(model_output, restored_output)
@@ -502,18 +510,20 @@
         ("tf_format", "tf", "model"),
         ("keras_format", "keras_v3", "model.keras"),
     )
     def test_saved_model(self, save_format, filename):
         model = FunctionalPipeline()
         x = tf.strings.as_string(tf.random.uniform((8, 5)))
         model_output = model.predict(x)
-        save_path = os.path.join(self.get_temp_dir(), filename)
-        model.save(save_path, save_format=save_format)
+        path = os.path.join(self.get_temp_dir(), filename)
+        # Don't save traces in the tf format, we check compilation elsewhere.
+        kwargs = {"save_traces": False} if save_format == "tf" else {}
+        model.save(path, save_format=save_format, **kwargs)
         restored_model = keras.models.load_model(
-            save_path, custom_objects={"FunctionalPipeline": FunctionalPipeline}
+            path, custom_objects={"FunctionalPipeline": FunctionalPipeline}
         )
 
         # Check we got the real object back.
         self.assertIsInstance(restored_model, FunctionalPipeline)
         # Check that output matches.
         restored_output = restored_model.predict(x)
         self.assertAllClose(model_output, restored_output)
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/python_utils.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/python_utils_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/tf_utils.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,22 @@
     Args:
         inputs: Input tensor, or dict/list/tuple of input tensors.
     """
     list_outputs = tensor_to_list(inputs)
     return _decode_strings_to_utf8(list_outputs)
 
 
+def truncate_at_token(inputs, token, mask):
+    """Truncate at first instance of `token`, ignoring `mask`."""
+    matches = (inputs == token) & (~mask)
+    end_indices = tf.cast(tf.math.argmax(matches, -1), "int32")
+    end_indices = tf.where(end_indices == 0, tf.shape(inputs)[-1], end_indices)
+    return tf.RaggedTensor.from_tensor(inputs, end_indices)
+
+
 def assert_tf_text_installed(symbol_name):
     """Detokenize and convert tensor to nested lists of python strings."""
     if tf_text is None:
         raise ImportError(
             f"{symbol_name} requires the `tensorflow-text` package. "
             "Please install with `pip install tensorflow-text`."
         )
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp/utils/tf_utils_test.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/tf_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp.egg-info/PKG-INFO` & `keras-nlp-0.5.0.dev0/keras_nlp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nlp
-Version: 0.4.1.dev0
+Version: 0.5.0.dev0
 Summary: Industry-strength Natural Language Processing extensions for Keras.
 Home-page: https://github.com/keras-team/keras-nlp
 Author: Keras team
 Author-email: keras-nlp@google.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +36,15 @@
 that have state-of-the-art preset weights and architectures when used 
 out-of-the-box and are easily customizable when more control is needed. We 
 emphasize in-graph computation for all workflows so that developers can expect 
 easy productionization using the TensorFlow ecosystem.
 
 This library is an extension of the core Keras API; all high-level modules are 
 [`Layers`](https://keras.io/api/layers/) or 
-[`Models`](https://keras.io/api/models/) that recieve that same level of polish 
+[`Models`](https://keras.io/api/models/) that receive that same level of polish 
 as core Keras. If you are familiar with Keras, congratulations! You already 
 understand most of KerasNLP.
 
 See our [Getting Started guide](https://keras.io/guides/keras_nlp/getting_started) 
 for example usage of our modular API starting with evaluating pretrained models 
 and building up to designing a novel transformer architecture and training a 
 tokenizer from scratch.  
@@ -69,57 +69,48 @@
 - [Call for Contributions](https://github.com/keras-team/keras-nlp/issues?q=is%3Aissue+is%3Aopen+label%3A%22contributions+welcome%22)
 
 ## Installation
 
 To install the latest official release:
 
 ```
-pip install keras-nlp tensorflow --upgrade
+pip install keras-nlp --upgrade
 ```
 
 To install the latest unreleased changes to the library, we recommend using
 pip to install directly from the master branch on github:
 
 ```
-pip install git+https://github.com/keras-team/keras-nlp.git tensorflow --upgrade
+pip install git+https://github.com/keras-team/keras-nlp.git --upgrade
 ```
 
 ## Quickstart
 
 Fine-tune BERT on a small sentiment analysis task using the 
 [`keras_nlp.models`](https://keras.io/api/keras_nlp/models/) API:
 
 ```python
 import keras_nlp
-from tensorflow import keras
 import tensorflow_datasets as tfds
 
 imdb_train, imdb_test = tfds.load(
     "imdb_reviews",
     split=["train", "test"],
     as_supervised=True,
     batch_size=16,
 )
+# Load a BERT model.
 classifier = keras_nlp.models.BertClassifier.from_preset(
-    "bert_base_en_uncased",
+    "bert_base_en_uncased", 
+    num_classes=2,
 )
-classifier.compile(
-    loss=keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-    optimizer=keras.optimizers.Adam(5e-5),
-    metrics=keras.metrics.SparseCategoricalAccuracy(),
-    jit_compile=True,
-)
-classifier.fit(
-    imdb_train,
-    validation_data=imdb_test,
-    epochs=1,
-)
-
-# Predict a new example
-classifier.predict(["What an amazing movie, three hours of pure bliss!"])
+# Fine-tune on IMDb movie reviews.
+classifier.fit(imdb_train, validation_data=imdb_test)
+# Predict two new examples.
+classifier.predict(["What an amazing movie!", "A total waste of my time."])
 ```
 
 For more in depth guides and examples, visit https://keras.io/keras_nlp/.
 
 ## Compatibility
 
 We follow [Semantic Versioning](https://semver.org/), and plan to
@@ -129,15 +120,15 @@
 
 ## Disclaimer
 
 KerasNLP provides access to pre-trained models via the `keras_nlp.models` API.
 These pre-trained models are provided on an "as is" basis, without warranties
 or conditions of any kind. The following underlying models are provided by third
 parties, and subject to separate licenses:
-DistilBERT, RoBERTa, XLM-RoBERTa, DeBERTa, and GPT-2.
+BART, DeBERTa, DistilBERT, GPT-2, OPT, RoBERTa, Whisper, and XLM-RoBERTa.
 
 ## Citing KerasNLP
 
 If KerasNLP helps your research, we appreciate your citations.
 Here is the BibTeX entry:
 
 ```bibtex
```

### Comparing `keras-nlp-0.4.1.dev0/keras_nlp.egg-info/SOURCES.txt` & `keras-nlp-0.5.0.dev0/keras_nlp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 examples/__init__.py
 examples/bert_pretraining/__init__.py
 examples/bert_pretraining/bert_config.py
 examples/bert_pretraining/bert_create_pretraining_data.py
 examples/bert_pretraining/bert_pretrain.py
@@ -14,25 +15,28 @@
 examples/machine_translation/train.py
 examples/tools/__init__.py
 examples/tools/split_sentences.py
 examples/tools/train_word_piece_vocab.py
 examples/utils/__init__.py
 examples/utils/data_utils.py
 examples/utils/scripting_utils.py
+integration_tests/__init__.py
+integration_tests/basic_usage_test.py
+integration_tests/import_test.py
 keras_nlp/__init__.py
+keras_nlp/api_export.py
 keras_nlp/conftest.py
 keras_nlp.egg-info/PKG-INFO
 keras_nlp.egg-info/SOURCES.txt
 keras_nlp.egg-info/dependency_links.txt
 keras_nlp.egg-info/requires.txt
 keras_nlp.egg-info/top_level.txt
-keras_nlp/benchmarks/__init__.py
-keras_nlp/benchmarks/sentiment_analysis.py
-keras_nlp/benchmarks/text_generation.py
 keras_nlp/layers/__init__.py
+keras_nlp/layers/cached_multi_head_attention.py
+keras_nlp/layers/cached_multi_head_attention_test.py
 keras_nlp/layers/f_net_encoder.py
 keras_nlp/layers/f_net_encoder_test.py
 keras_nlp/layers/masked_lm_head.py
 keras_nlp/layers/masked_lm_head_test.py
 keras_nlp/layers/masked_lm_mask_generator.py
 keras_nlp/layers/masked_lm_mask_generator_test.py
 keras_nlp/layers/multi_segment_packer.py
@@ -67,14 +71,15 @@
 keras_nlp/metrics/rouge_l_test.py
 keras_nlp/metrics/rouge_n.py
 keras_nlp/metrics/rouge_n_test.py
 keras_nlp/models/__init__.py
 keras_nlp/models/backbone.py
 keras_nlp/models/preprocessor.py
 keras_nlp/models/task.py
+keras_nlp/models/task_test.py
 keras_nlp/models/albert/__init__.py
 keras_nlp/models/albert/albert_backbone.py
 keras_nlp/models/albert/albert_backbone_test.py
 keras_nlp/models/albert/albert_classifier.py
 keras_nlp/models/albert/albert_classifier_test.py
 keras_nlp/models/albert/albert_masked_lm.py
 keras_nlp/models/albert/albert_masked_lm_preprocessor.py
@@ -85,59 +90,79 @@
 keras_nlp/models/albert/albert_presets.py
 keras_nlp/models/albert/albert_presets_test.py
 keras_nlp/models/albert/albert_tokenizer.py
 keras_nlp/models/albert/albert_tokenizer_test.py
 keras_nlp/models/bart/__init__.py
 keras_nlp/models/bart/bart_backbone.py
 keras_nlp/models/bart/bart_backbone_test.py
+keras_nlp/models/bart/bart_preprocessor.py
+keras_nlp/models/bart/bart_preprocessor_test.py
 keras_nlp/models/bart/bart_presets.py
 keras_nlp/models/bart/bart_presets_test.py
+keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor.py
+keras_nlp/models/bart/bart_seq_2_seq_lm_preprocessor_test.py
 keras_nlp/models/bart/bart_tokenizer.py
 keras_nlp/models/bart/bart_tokenizer_test.py
 keras_nlp/models/bert/__init__.py
 keras_nlp/models/bert/bert_backbone.py
 keras_nlp/models/bert/bert_backbone_test.py
 keras_nlp/models/bert/bert_classifier.py
 keras_nlp/models/bert/bert_classifier_test.py
+keras_nlp/models/bert/bert_masked_lm.py
+keras_nlp/models/bert/bert_masked_lm_preprocessor.py
+keras_nlp/models/bert/bert_masked_lm_preprocessor_test.py
+keras_nlp/models/bert/bert_masked_lm_test.py
 keras_nlp/models/bert/bert_preprocessor.py
 keras_nlp/models/bert/bert_preprocessor_test.py
 keras_nlp/models/bert/bert_presets.py
 keras_nlp/models/bert/bert_presets_test.py
 keras_nlp/models/bert/bert_tokenizer.py
 keras_nlp/models/bert/bert_tokenizer_test.py
 keras_nlp/models/deberta_v3/__init__.py
 keras_nlp/models/deberta_v3/deberta_v3_backbone.py
 keras_nlp/models/deberta_v3/deberta_v3_backbone_test.py
 keras_nlp/models/deberta_v3/deberta_v3_classifier.py
 keras_nlp/models/deberta_v3/deberta_v3_classifier_test.py
+keras_nlp/models/deberta_v3/deberta_v3_masked_lm.py
+keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor.py
+keras_nlp/models/deberta_v3/deberta_v3_masked_lm_preprocessor_test.py
+keras_nlp/models/deberta_v3/deberta_v3_masked_lm_test.py
 keras_nlp/models/deberta_v3/deberta_v3_preprocessor.py
 keras_nlp/models/deberta_v3/deberta_v3_preprocessor_test.py
 keras_nlp/models/deberta_v3/deberta_v3_presets.py
 keras_nlp/models/deberta_v3/deberta_v3_presets_test.py
 keras_nlp/models/deberta_v3/deberta_v3_tokenizer.py
 keras_nlp/models/deberta_v3/deberta_v3_tokenizer_test.py
 keras_nlp/models/deberta_v3/disentangled_attention_encoder.py
 keras_nlp/models/deberta_v3/disentangled_self_attention.py
 keras_nlp/models/deberta_v3/relative_embedding.py
 keras_nlp/models/distil_bert/__init__.py
 keras_nlp/models/distil_bert/distil_bert_backbone.py
 keras_nlp/models/distil_bert/distil_bert_backbone_test.py
 keras_nlp/models/distil_bert/distil_bert_classifier.py
 keras_nlp/models/distil_bert/distil_bert_classifier_test.py
+keras_nlp/models/distil_bert/distil_bert_masked_lm.py
+keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor.py
+keras_nlp/models/distil_bert/distil_bert_masked_lm_preprocessor_test.py
+keras_nlp/models/distil_bert/distil_bert_masked_lm_test.py
 keras_nlp/models/distil_bert/distil_bert_preprocessor.py
 keras_nlp/models/distil_bert/distil_bert_preprocessor_test.py
 keras_nlp/models/distil_bert/distil_bert_presets.py
 keras_nlp/models/distil_bert/distil_bert_presets_test.py
 keras_nlp/models/distil_bert/distil_bert_tokenizer.py
 keras_nlp/models/distil_bert/distil_bert_tokenizer_test.py
 keras_nlp/models/f_net/__init__.py
 keras_nlp/models/f_net/f_net_backbone.py
 keras_nlp/models/f_net/f_net_backbone_test.py
 keras_nlp/models/f_net/f_net_classifier.py
 keras_nlp/models/f_net/f_net_classifier_test.py
+keras_nlp/models/f_net/f_net_masked_lm.py
+keras_nlp/models/f_net/f_net_masked_lm_preprocessor.py
+keras_nlp/models/f_net/f_net_masked_lm_preprocessor_test.py
+keras_nlp/models/f_net/f_net_masked_lm_test.py
 keras_nlp/models/f_net/f_net_preprocessor.py
 keras_nlp/models/f_net/f_net_preprocessor_test.py
 keras_nlp/models/f_net/f_net_presets.py
 keras_nlp/models/f_net/f_net_presets_test.py
 keras_nlp/models/f_net/f_net_tokenizer.py
 keras_nlp/models/f_net/f_net_tokenizer_test.py
 keras_nlp/models/gpt2/__init__.py
@@ -152,14 +177,20 @@
 keras_nlp/models/gpt2/gpt2_presets.py
 keras_nlp/models/gpt2/gpt2_presets_test.py
 keras_nlp/models/gpt2/gpt2_tokenizer.py
 keras_nlp/models/gpt2/gpt2_tokenizer_test.py
 keras_nlp/models/opt/__init__.py
 keras_nlp/models/opt/opt_backbone.py
 keras_nlp/models/opt/opt_backbone_test.py
+keras_nlp/models/opt/opt_causal_lm.py
+keras_nlp/models/opt/opt_causal_lm_preprocessor.py
+keras_nlp/models/opt/opt_causal_lm_preprocessor_test.py
+keras_nlp/models/opt/opt_causal_lm_test.py
+keras_nlp/models/opt/opt_preprocessor.py
+keras_nlp/models/opt/opt_preprocessor_test.py
 keras_nlp/models/opt/opt_presets.py
 keras_nlp/models/opt/opt_presets_test.py
 keras_nlp/models/opt/opt_tokenizer.py
 keras_nlp/models/opt/opt_tokenizer_test.py
 keras_nlp/models/roberta/__init__.py
 keras_nlp/models/roberta/roberta_backbone.py
 keras_nlp/models/roberta/roberta_backbone_test.py
@@ -172,44 +203,63 @@
 keras_nlp/models/roberta/roberta_multi_segment_packer.py
 keras_nlp/models/roberta/roberta_preprocessor.py
 keras_nlp/models/roberta/roberta_preprocessor_test.py
 keras_nlp/models/roberta/roberta_presets.py
 keras_nlp/models/roberta/roberta_presets_test.py
 keras_nlp/models/roberta/roberta_tokenizer.py
 keras_nlp/models/roberta/roberta_tokenizer_test.py
+keras_nlp/models/t5/__init__.py
+keras_nlp/models/t5/t5_backbone.py
+keras_nlp/models/t5/t5_backbone_test.py
+keras_nlp/models/t5/t5_layer_norm.py
+keras_nlp/models/t5/t5_multi_head_attention.py
+keras_nlp/models/t5/t5_tokenizer.py
+keras_nlp/models/t5/t5_tokenizer_test.py
+keras_nlp/models/t5/t5_transformer_layer.py
+keras_nlp/models/whisper/__init__.py
+keras_nlp/models/whisper/whisper_backbone.py
+keras_nlp/models/whisper/whisper_backbone_test.py
+keras_nlp/models/whisper/whisper_decoder.py
+keras_nlp/models/whisper/whisper_encoder.py
 keras_nlp/models/xlm_roberta/__init__.py
 keras_nlp/models/xlm_roberta/xlm_roberta_backbone.py
 keras_nlp/models/xlm_roberta/xlm_roberta_backbone_test.py
 keras_nlp/models/xlm_roberta/xlm_roberta_classifier.py
 keras_nlp/models/xlm_roberta/xlm_roberta_classifier_test.py
+keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm.py
+keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor.py
+keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_preprocessor_test.py
+keras_nlp/models/xlm_roberta/xlm_roberta_masked_lm_test.py
 keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor.py
 keras_nlp/models/xlm_roberta/xlm_roberta_preprocessor_test.py
 keras_nlp/models/xlm_roberta/xlm_roberta_presets.py
 keras_nlp/models/xlm_roberta/xlm_roberta_presets_test.py
 keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer.py
 keras_nlp/models/xlm_roberta/xlm_roberta_tokenizer_test.py
 keras_nlp/samplers/__init__.py
 keras_nlp/samplers/beam_sampler.py
 keras_nlp/samplers/beam_sampler_test.py
+keras_nlp/samplers/contrastive_sampler.py
+keras_nlp/samplers/contrastive_sampler_test.py
 keras_nlp/samplers/greedy_sampler.py
 keras_nlp/samplers/greedy_sampler_test.py
+keras_nlp/samplers/random_sampler.py
+keras_nlp/samplers/random_sampler_test.py
 keras_nlp/samplers/sampler.py
-keras_nlp/samplers/sampler_test.py
+keras_nlp/samplers/serialization.py
+keras_nlp/samplers/serialization_test.py
 keras_nlp/samplers/top_k_sampler.py
 keras_nlp/samplers/top_k_sampler_test.py
 keras_nlp/samplers/top_p_sampler.py
 keras_nlp/samplers/top_p_sampler_test.py
 keras_nlp/tests/__init__.py
 keras_nlp/tests/doc_tests/__init__.py
 keras_nlp/tests/doc_tests/docstring_lib.py
 keras_nlp/tests/doc_tests/docstring_test.py
 keras_nlp/tests/doc_tests/fenced_docstring_lib.py
-keras_nlp/tests/integration_tests/__init__.py
-keras_nlp/tests/integration_tests/basic_usage_test.py
-keras_nlp/tests/integration_tests/import_test.py
 keras_nlp/tokenizers/__init__.py
 keras_nlp/tokenizers/byte_pair_tokenizer.py
 keras_nlp/tokenizers/byte_pair_tokenizer_test.py
 keras_nlp/tokenizers/byte_tokenizer.py
 keras_nlp/tokenizers/byte_tokenizer_test.py
 keras_nlp/tokenizers/sentence_piece_tokenizer.py
 keras_nlp/tokenizers/sentence_piece_tokenizer_test.py
@@ -226,16 +276,14 @@
 keras_nlp/utils/__init__.py
 keras_nlp/utils/keras_utils.py
 keras_nlp/utils/keras_utils_test.py
 keras_nlp/utils/pipeline_model.py
 keras_nlp/utils/pipeline_model_test.py
 keras_nlp/utils/python_utils.py
 keras_nlp/utils/python_utils_test.py
-keras_nlp/utils/text_generation.py
-keras_nlp/utils/text_generation_test.py
 keras_nlp/utils/tf_utils.py
 keras_nlp/utils/tf_utils_test.py
 tools/__init__.py
 tools/count_preset_params.py
 tools/checkpoint_conversion/__init__.py
 tools/checkpoint_conversion/checkpoint_conversion_utils.py
 tools/checkpoint_conversion/convert_albert_checkpoints.py
```

### Comparing `keras-nlp-0.4.1.dev0/setup.cfg` & `keras-nlp-0.5.0.dev0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 	ignore::PendingDeprecationWarning
 	ignore::FutureWarning
 	ignore::UserWarning
 	ignore:Custom mask layers require a config
 addopts = -vv
 norecursedirs = build
 
-[isort]
-known_first_party = keras_nlp,tests
-default_section = THIRDPARTY
-line_length = 80
-profile = black
-
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	@abstract
 	raise NotImplementedError
 omit = *_test.py
 
@@ -31,13 +25,13 @@
 	N802
 	N812
 	E722
 exclude = 
 	*_pb2.py
 	*_pb2_grpc.py
 per-file-ignores = **/__init__.py:F401
-max-line-length = 80
+max-line-length = 200
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `keras-nlp-0.4.1.dev0/setup.py` & `keras-nlp-0.5.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 setup(
     name="keras-nlp",
     description=(
         "Industry-strength Natural Language Processing extensions for Keras."
     ),
     long_description=README,
     long_description_content_type="text/markdown",
-    version="0.4.1.dev0",
+    version="0.5.0.dev0",
     url="https://github.com/keras-team/keras-nlp",
     author="Keras team",
     author_email="keras-nlp@google.com",
     license="Apache License 2.0",
     install_requires=[
         "absl-py",
         "numpy",
```

### Comparing `keras-nlp-0.4.1.dev0/tools/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/tests/doc_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/__init__.py` & `keras-nlp-0.5.0.dev0/keras_nlp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/checkpoint_conversion_utils.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/checkpoint_conversion_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import hashlib
+import tarfile
+import zipfile
 
 
 def get_md5_checksum(file_path):
     md5_hash = hashlib.md5()
     with open(file_path, "rb") as f:
         for byte_block in iter(lambda: f.read(4096), b""):
             md5_hash.update(byte_block)
     return md5_hash.hexdigest()
+
+
+def extract_files_from_archive(archive_file_path):
+    if archive_file_path.endswith(".tar.gz"):
+        with tarfile.open(archive_file_path, "r:gz") as tar:
+            return tar.extractall()
+    elif archive_file_path.endswith(".zip"):
+        with zipfile.ZipFile(archive_file_path, "r") as zip_ref:
+            return zip_ref.extractall()
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_albert_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_albert_checkpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import shutil
 
 import numpy as np
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
     "albert_base_en_uncased": "albert-base-v2",
     "albert_large_en_uncased": "albert-large-v2",
     "albert_extra_large_en_uncased": "albert-xlarge-v2",
     "albert_extra_extra_large_en_uncased": "albert-xxlarge-v2",
 }
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_bart_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_bart_checkpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import shutil
 
 import numpy as np
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
     "bart_base_en": "facebook/bart-base",
     "bart_large_en": "facebook/bart-large",
 }
 
 FLAGS = flags.FLAGS
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_deberta_v3_checkpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 
 import numpy as np
 import requests
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 from keras_nlp.models.deberta_v3.deberta_v3_backbone import DebertaV3Backbone
 from keras_nlp.models.deberta_v3.deberta_v3_preprocessor import (
     DebertaV3Preprocessor,
 )
 from keras_nlp.models.deberta_v3.deberta_v3_tokenizer import DebertaV3Tokenizer
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
     "deberta_v3_extra_small_en": "microsoft/deberta-v3-xsmall",
     "deberta_v3_small_en": "microsoft/deberta-v3-small",
     "deberta_v3_base_en": "microsoft/deberta-v3-base",
     "deberta_v3_large_en": "microsoft/deberta-v3-large",
     "deberta_v3_base_multi": "microsoft/mdeberta-v3-base",
@@ -42,18 +40,18 @@
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "preset", None, f'Must be one of {",".join(PRESET_MAP.keys())}'
 )
 
 
-def download_files(preset, hf_model_name):
+def download_files(hf_model_name):
     print("-> Download original vocabulary and config.")
 
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     if not os.path.exists(extract_dir):
         os.makedirs(extract_dir)
 
     # Config.
     config_path = os.path.join(extract_dir, "config.json")
     response = requests.get(
         f"https://huggingface.co/{hf_model_name}/raw/main/config.json"
@@ -66,43 +64,43 @@
     response = requests.get(
         f"https://huggingface.co/{hf_model_name}/resolve/main/spm.model"
     )
     open(spm_path, "wb").write(response.content)
     print(f"`{spm_path}`")
 
 
-def define_preprocessor(preset, hf_model_name):
+def define_preprocessor(hf_model_name):
     print("\n-> Define the tokenizers.")
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     spm_path = os.path.join(extract_dir, "spm.model")
 
     keras_nlp_tokenizer = DebertaV3Tokenizer(proto=spm_path)
 
     # Avoid having padding tokens. This is because the representations of the
     # padding token may be vastly different from the representations computed in
     # the original model. See https://github.com/keras-team/keras/pull/16619#issuecomment-1156338394.
     sequence_length = 14
-    if preset == "deberta_v3_base_multi":
+    if FLAGS.preset == "deberta_v3_base_multi":
         sequence_length = 17
     keras_nlp_preprocessor = DebertaV3Preprocessor(
         keras_nlp_tokenizer, sequence_length=sequence_length
     )
 
     hf_tokenizer = transformers.AutoTokenizer.from_pretrained(hf_model_name)
 
     print("\n-> Print MD5 checksum of the vocab files.")
     print(f"`{spm_path}` md5sum: ", get_md5_checksum(spm_path))
 
     return keras_nlp_preprocessor, hf_tokenizer
 
 
-def convert_checkpoints(preset, keras_nlp_model, hf_model):
+def convert_checkpoints(keras_nlp_model, hf_model):
     print("\n-> Convert original weights to KerasNLP format.")
 
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     config_path = os.path.join(extract_dir, "config.json")
 
     # Build config.
     cfg = {}
     with open(config_path, "r") as pt_cfg_handler:
         pt_cfg = json.load(pt_cfg_handler)
     cfg["vocabulary_size"] = pt_cfg["vocab_size"]
@@ -252,22 +250,21 @@
         keras_nlp_model.get_layer(
             f"disentangled_attention_encoder_layer_{i}"
         )._feedforward_layernorm.beta.assign(
             hf_wts[f"encoder.layer.{i}.output.LayerNorm.bias"].numpy()
         )
 
     # Save the model.
-    print(f"\n-> Save KerasNLP model weights to `{preset}.h5`.")
-    keras_nlp_model.save_weights(f"{preset}.h5")
+    print(f"\n-> Save KerasNLP model weights to `{FLAGS.preset}.h5`.")
+    keras_nlp_model.save_weights(f"{FLAGS.preset}.h5")
 
     return keras_nlp_model
 
 
 def check_output(
-    preset,
     keras_nlp_preprocessor,
     keras_nlp_model,
     hf_tokenizer,
     hf_model,
 ):
     print("\n-> Check the outputs.")
     sample_text = ["cricket is awesome, easily the best sport in the world!"]
@@ -283,41 +280,36 @@
     hf_output = hf_model(**hf_inputs).last_hidden_state
 
     print("KerasNLP output:", keras_nlp_output[0, 0, :10])
     print("HF output:", hf_output[0, 0, :10])
     print("Difference:", np.mean(keras_nlp_output - hf_output.detach().numpy()))
 
     # Show the MD5 checksum of the model weights.
-    print("Model md5sum: ", get_md5_checksum(f"./{preset}.h5"))
+    print("Model md5sum: ", get_md5_checksum(f"./{FLAGS.preset}.h5"))
 
 
 def main(_):
     hf_model_name = PRESET_MAP[FLAGS.preset]
 
-    download_files(FLAGS.preset, hf_model_name)
+    download_files(hf_model_name)
 
-    keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(
-        FLAGS.preset, hf_model_name
-    )
+    keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(hf_model_name)
 
     print("\n-> Load KerasNLP model.")
     keras_nlp_model = DebertaV3Backbone.from_preset(
         FLAGS.preset, load_weights=False
     )
 
     print("\n-> Load HF model.")
     hf_model = transformers.AutoModel.from_pretrained(hf_model_name)
     hf_model.eval()
 
-    keras_nlp_model = convert_checkpoints(
-        FLAGS.preset, keras_nlp_model, hf_model
-    )
+    keras_nlp_model = convert_checkpoints(keras_nlp_model, hf_model)
 
     check_output(
-        FLAGS.preset,
         keras_nlp_preprocessor,
         keras_nlp_model,
         hf_tokenizer,
         hf_model,
     )
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_distilbert_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_distilbert_checkpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "preset", None, f'Must be one of {",".join(PRESET_MAP.keys())}'
 )
 
 
-def download_files(preset, hf_model_name):
+def download_files(hf_model_name):
     print("-> Download original vocab and config.")
 
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     if not os.path.exists(extract_dir):
         os.makedirs(extract_dir)
 
     # Config.
     config_path = os.path.join(extract_dir, "config.json")
     response = requests.get(
         f"https://huggingface.co/{hf_model_name}/raw/main/config.json"
@@ -60,17 +60,17 @@
     response = requests.get(
         f"https://huggingface.co/{hf_model_name}/raw/main/vocab.txt"
     )
     open(vocab_path, "wb").write(response.content)
     print(f"`{vocab_path}`")
 
 
-def define_preprocessor(preset, hf_model_name):
+def define_preprocessor(hf_model_name):
     print("\n-> Define the tokenizers.")
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     vocab_path = os.path.join(extract_dir, "vocab.txt")
 
     keras_nlp_tokenizer = keras_nlp.models.DistilBertTokenizer(
         vocabulary=vocab_path,
     )
     keras_nlp_preprocessor = keras_nlp.models.DistilBertPreprocessor(
         keras_nlp_tokenizer
@@ -80,18 +80,18 @@
 
     print("\n-> Print MD5 checksum of the vocab files.")
     print(f"`{vocab_path}` md5sum: ", get_md5_checksum(vocab_path))
 
     return keras_nlp_preprocessor, hf_tokenizer
 
 
-def convert_checkpoints(preset, keras_nlp_model, hf_model):
+def convert_checkpoints(keras_nlp_model, hf_model):
     print("\n-> Convert original weights to KerasNLP format.")
 
-    extract_dir = EXTRACT_DIR.format(preset)
+    extract_dir = EXTRACT_DIR.format(FLAGS.preset)
     config_path = os.path.join(extract_dir, "config.json")
 
     # Build config.
     cfg = {}
     with open(config_path, "r") as pt_cfg_handler:
         pt_cfg = json.load(pt_cfg_handler)
     cfg["vocabulary_size"] = pt_cfg["vocab_size"]
@@ -240,22 +240,21 @@
         keras_nlp_model.get_layer(
             f"transformer_layer_{i}"
         )._feedforward_layernorm.beta.assign(
             hf_wts[f"transformer.layer.{i}.output_layer_norm.bias"].numpy()
         )
 
     # Save the model.
-    print(f"\n-> Save KerasNLP model weights to `{preset}.h5`.")
-    keras_nlp_model.save_weights(f"{preset}.h5")
+    print(f"\n-> Save KerasNLP model weights to `{FLAGS.preset}.h5`.")
+    keras_nlp_model.save_weights(f"{FLAGS.preset}.h5")
 
     return keras_nlp_model
 
 
 def check_output(
-    preset,
     keras_nlp_preprocessor,
     keras_nlp_model,
     hf_tokenizer,
     hf_model,
 ):
     print("\n-> Check the outputs.")
     sample_text = ["cricket is awesome, easily the best sport in the world!"]
@@ -271,41 +270,36 @@
     hf_output = hf_model(**hf_inputs).last_hidden_state
 
     print("KerasNLP output:", keras_nlp_output[0, 0, :10])
     print("HF output:", hf_output[0, 0, :10])
     print("Difference:", np.mean(keras_nlp_output - hf_output.detach().numpy()))
 
     # Show the MD5 checksum of the model weights.
-    print("Model md5sum: ", get_md5_checksum(f"./{preset}.h5"))
+    print("Model md5sum: ", get_md5_checksum(f"./{FLAGS.preset}.h5"))
 
 
 def main(_):
     hf_model_name = PRESET_MAP[FLAGS.preset]
 
-    download_files(FLAGS.preset, hf_model_name)
+    download_files(hf_model_name)
 
-    keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(
-        FLAGS.preset, hf_model_name
-    )
+    keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(hf_model_name)
 
     print("\n-> Load KerasNLP model.")
     keras_nlp_model = keras_nlp.models.DistilBertBackbone.from_preset(
         FLAGS.preset, load_weights=False
     )
 
     print("\n-> Load HF model.")
     hf_model = transformers.AutoModel.from_pretrained(hf_model_name)
     hf_model.eval()
 
-    keras_nlp_model = convert_checkpoints(
-        FLAGS.preset, keras_nlp_model, hf_model
-    )
+    keras_nlp_model = convert_checkpoints(keras_nlp_model, hf_model)
 
     check_output(
-        FLAGS.preset,
         keras_nlp_preprocessor,
         keras_nlp_model,
         hf_tokenizer,
         hf_model,
     )
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_f_net_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_f_net_checkpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import shutil
 
 import numpy as np
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
     "f_net_base_en": "google/fnet-base",
     "f_net_large_en": "google/fnet-large",
 }
 
 FLAGS = flags.FLAGS
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_gpt2_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_gpt2_checkpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,50 +16,48 @@
 
 import numpy as np
 import requests
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 # Temporarily directly import gpt2 until we expose it.
 from keras_nlp.models.gpt2.gpt2_backbone import GPT2Backbone
 from keras_nlp.models.gpt2.gpt2_tokenizer import GPT2Tokenizer
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
-    "gpt2_base": ("124M", "gpt2"),
-    "gpt2_medium": ("355M", "gpt2-medium"),
-    "gpt2_large": ("774M", "gpt2-large"),
-    "gpt2_extra_large": ("1558M", "gpt2-xl"),
+    "gpt2_base_en": ("124M", "gpt2"),
+    "gpt2_medium_en": ("355M", "gpt2-medium"),
+    "gpt2_large_en": ("774M", "gpt2-large"),
+    "gpt2_extra_large_en": ("1558M", "gpt2-xl"),
 }
 
 DOWNLOAD_SCRIPT_URL = (
     "https://raw.githubusercontent.com/openai/gpt-2/master/download_model.py"
 )
 
 EXTRACT_DIR = "./models/{}"
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "preset", None, f'Must be one of {",".join(PRESET_MAP.keys())}'
 )
 
 
-def download_model(preset, num_params):
+def download_model(num_params):
     print("-> Download original weights.")
     response = requests.get(DOWNLOAD_SCRIPT_URL)
     open("download_model.py", "wb").write(response.content)
 
     os.system(f"python download_model.py {num_params}")
 
 
-def convert_checkpoints(preset, num_params):
+def convert_checkpoints(num_params):
     print("\n-> Convert original weights to KerasNLP format.")
     # GPT-2 paths.
     extract_dir = EXTRACT_DIR.format(num_params)
     checkpoint_path = os.path.join(extract_dir, "model.ckpt")
     config_path = os.path.join(extract_dir, "hparams.json")
 
     with open(config_path, "r") as f:
@@ -72,15 +70,15 @@
     for name, shape in vars:
         print(name, shape)
         weight = tf.train.load_variable(checkpoint_path, name)
         weights[name] = weight
 
     # Temporary direct import, as we aren't exposing this quite yet.
     keras_nlp_model = GPT2Backbone.from_preset(
-        preset,
+        FLAGS.preset,
         load_weights=False,
     )
 
     keras_nlp_model.get_layer("token_embedding").embeddings.assign(
         weights["model/wte"]
     )
     keras_nlp_model.get_layer("position_embedding").position_embeddings.assign(
@@ -187,21 +185,21 @@
     keras_nlp_model.get_layer("layer_norm").gamma.assign(
         weights["model/ln_f/g"]
     )
 
     keras_nlp_model.get_layer("layer_norm").beta.assign(weights["model/ln_f/b"])
 
     # Save the model.
-    print(f"\n-> Save KerasNLP model weights to `{preset}.h5`.")
-    keras_nlp_model.save_weights(f"{preset}.h5")
+    print(f"\n-> Save KerasNLP model weights to `{FLAGS.preset}.h5`.")
+    keras_nlp_model.save_weights(f"{FLAGS.preset}.h5")
 
     return keras_nlp_model
 
 
-def define_tokenizer(preset, num_params, hf_model_name):
+def define_tokenizer(num_params, hf_model_name):
     print("\n-> Define the tokenizers.")
     extract_dir = extract_dir = EXTRACT_DIR.format(num_params)
     merges_path = os.path.join(extract_dir, "vocab.bpe")
     vocab_path = os.path.join(extract_dir, "encoder.json")
 
     keras_nlp_tokenizer = GPT2Tokenizer(
         vocabulary=vocab_path,
@@ -213,15 +211,14 @@
     print(f"`{vocab_path}` md5sum: ", get_md5_checksum(vocab_path))
     print(f"`{merges_path}` md5sum: ", get_md5_checksum(merges_path))
 
     return keras_nlp_tokenizer, hf_tokenizer
 
 
 def check_output(
-    preset,
     keras_nlp_model,
     keras_nlp_tokenizer,
     hf_model,
     hf_tokenizer,
 ):
     print("\n-> Check the outputs.")
     input_str = ["the quick brown fox ran, galloped and jumped."]
@@ -241,40 +238,39 @@
     hf_output = hf_model(**hf_inputs).last_hidden_state
 
     print("KerasNLP output:", keras_nlp_output[0, 0, :10])
     print("HF output:", hf_output[0, 0, :10])
     print("Difference:", np.mean(keras_nlp_output - hf_output.detach().numpy()))
 
     # Show the MD5 checksum of the model weights.
-    print("Model md5sum: ", get_md5_checksum(f"./{preset}.h5"))
+    print("Model md5sum: ", get_md5_checksum(f"./{FLAGS.preset}.h5"))
 
     return keras_nlp_output
 
 
 def main(_):
     assert (
         FLAGS.preset in PRESET_MAP.keys()
     ), f'Invalid preset {FLAGS.preset}. Must be one of {",".join(PRESET_MAP.keys())}'
     num_params = PRESET_MAP[FLAGS.preset][0]
     hf_model_name = PRESET_MAP[FLAGS.preset][1]
 
-    download_model(FLAGS.preset, num_params)
+    download_model(num_params)
 
-    keras_nlp_model = convert_checkpoints(FLAGS.preset, num_params)
+    keras_nlp_model = convert_checkpoints(num_params)
 
     print("\n-> Load HF model.")
     hf_model = transformers.AutoModel.from_pretrained(hf_model_name)
     hf_model.eval()
 
     keras_nlp_tokenizer, hf_tokenizer = define_tokenizer(
-        FLAGS.preset, num_params, hf_model_name
+        num_params, hf_model_name
     )
 
     check_output(
-        FLAGS.preset,
         keras_nlp_model,
         keras_nlp_tokenizer,
         hf_model,
         hf_tokenizer,
     )
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_opt_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_opt_checkpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 import shutil
 
 import numpy as np
 import tensorflow as tf
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import get_md5_checksum
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
     "opt_125m_en": "facebook/opt-125m",
     "opt_1.3b_en": "facebook/opt-1.3b",
     "opt_2.7b_en": "facebook/opt-2.7b",
     "opt_6.7b_en": "facebook/opt-6.7b",
 }
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_roberta_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_roberta_checkpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,46 +16,45 @@
 
 import numpy as np
 import tensorflow as tf
 import torch
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import extract_files_from_archive
+from checkpoint_conversion_utils import get_md5_checksum
 from tensorflow import keras
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
-    "roberta_base": ("roberta.base", "roberta-base"),
-    "roberta_large": ("roberta.large", "roberta-large"),
+    "roberta_base_en": ("roberta.base", "roberta-base"),
+    "roberta_large_en": ("roberta.large", "roberta-large"),
 }
 
 DOWNLOAD_SCRIPT_URL = "https://dl.fbaipublicfiles.com/fairseq/models/{}.tar.gz"
 
 EXTRACT_DIR = "./{}"
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "preset", None, f'Must be one of {",".join(PRESET_MAP.keys())}'
 )
 
 
-def download_model(preset, size, hf_model_name):
+def download_model(size, hf_model_name):
     print("-> Download original weights.")
     extract_dir = EXTRACT_DIR.format(size)
     archive_file_path = keras.utils.get_file(
         fname=None,
         origin=DOWNLOAD_SCRIPT_URL.format(size),
-        cache_subdir=os.path.join("checkpoint_conversion", preset),
+        cache_subdir=os.path.join("checkpoint_conversion", FLAGS.preset),
     )
 
-    os.system(f"tar -xvf {archive_file_path}")
+    extract_files_from_archive(archive_file_path)
 
     # The original `tar.gz` file does not have the vocab files. Let's fetch
     # them from HF.
     vocabulary_path = keras.utils.get_file(
         fname=None,
         origin=f"https://huggingface.co/{hf_model_name}/raw/main/vocab.json",
     )
@@ -63,15 +62,15 @@
     merges_path = keras.utils.get_file(
         fname=None,
         origin=f"https://huggingface.co/{hf_model_name}/raw/main/merges.txt",
     )
     shutil.copy(merges_path, extract_dir)
 
 
-def convert_checkpoints(preset, size):
+def convert_checkpoints(size):
     print("\n-> Convert original weights to KerasNLP format.")
     # RoBERTa paths.
     extract_dir = EXTRACT_DIR.format(size)
     checkpoint_path = os.path.join(extract_dir, "model.pt")
 
     # Load PyTorch RoBERTa checkpoint.
     pt_ckpt = torch.load(checkpoint_path, map_location=torch.device("cpu"))
@@ -90,15 +89,15 @@
             .numpy()
             .shape[0]
         ),
     }
     print("Config:", cfg)
 
     keras_nlp_model = keras_nlp.models.RobertaBackbone.from_preset(
-        preset, load_weights=False
+        FLAGS.preset, load_weights=False
     )
 
     # Embedding Layer.
     keras_nlp_model.get_layer("embeddings").token_embedding.embeddings.assign(
         pt_model["decoder.sentence_encoder.embed_tokens.weight"].numpy()
     )
     keras_nlp_model.get_layer(
@@ -261,21 +260,21 @@
         )._feedforward_layernorm.beta.assign(
             pt_model[
                 f"decoder.sentence_encoder.layers.{i}.final_layer_norm.bias"
             ].numpy()
         )
 
     # Save the model.
-    print(f"\n-> Save KerasNLP model weights to `{preset}.h5`.")
-    keras_nlp_model.save_weights(f"{preset}.h5")
+    print(f"\n-> Save KerasNLP model weights to `{FLAGS.preset}.h5`.")
+    keras_nlp_model.save_weights(f"{FLAGS.preset}.h5")
 
     return keras_nlp_model
 
 
-def define_preprocessor(preset, hf_model_name, size):
+def define_preprocessor(hf_model_name, size):
     print("\n-> Define the tokenizers.")
     extract_dir = EXTRACT_DIR.format(size)
     vocabulary_path = os.path.join(extract_dir, "vocab.json")
     merges_path = os.path.join(extract_dir, "merges.txt")
 
     keras_nlp_tokenizer = keras_nlp.models.RobertaTokenizer(
         vocabulary=vocabulary_path, merges=merges_path
@@ -290,15 +289,14 @@
     print(f"`{vocabulary_path}` md5sum: ", get_md5_checksum(vocabulary_path))
     print(f"`{merges_path}` md5sum: ", get_md5_checksum(merges_path))
 
     return keras_nlp_preprocessor, hf_tokenizer
 
 
 def check_output(
-    preset,
     keras_nlp_model,
     keras_nlp_preprocessor,
     hf_model,
     hf_tokenizer,
 ):
     print("\n-> Check the outputs.")
     input_str = ["the quick brown fox ran, galloped and jumped."]
@@ -314,40 +312,39 @@
     hf_output = hf_model(**hf_inputs).last_hidden_state
 
     print("KerasNLP output:", keras_nlp_output[0, 0, :10])
     print("HF output:", hf_output[0, 0, :10])
     print("Difference:", np.mean(keras_nlp_output - hf_output.detach().numpy()))
 
     # Show the MD5 checksum of the model weights.
-    print("Model md5sum: ", get_md5_checksum(f"./{preset}.h5"))
+    print("Model md5sum: ", get_md5_checksum(f"./{FLAGS.preset}.h5"))
 
     return keras_nlp_output
 
 
 def main(_):
     assert (
         FLAGS.preset in PRESET_MAP.keys()
     ), f'Invalid preset {FLAGS.preset}. Must be one of {",".join(PRESET_MAP.keys())}'
     size = PRESET_MAP[FLAGS.preset][0]
     hf_model_name = PRESET_MAP[FLAGS.preset][1]
 
-    download_model(FLAGS.preset, size, hf_model_name)
+    download_model(size, hf_model_name)
 
-    keras_nlp_model = convert_checkpoints(FLAGS.preset, size)
+    keras_nlp_model = convert_checkpoints(size)
 
     print("\n-> Load HF model.")
     hf_model = transformers.AutoModel.from_pretrained(hf_model_name)
     hf_model.eval()
 
     keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(
-        FLAGS.preset, hf_model_name, size
+        hf_model_name, size
     )
 
     check_output(
-        FLAGS.preset,
         keras_nlp_model,
         keras_nlp_preprocessor,
         hf_model,
         hf_tokenizer,
     )
```

### Comparing `keras-nlp-0.4.1.dev0/tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py` & `keras-nlp-0.5.0.dev0/tools/checkpoint_conversion/convert_xlm_roberta_checkpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,48 +15,47 @@
 
 import numpy as np
 import tensorflow as tf
 import torch
 import transformers
 from absl import app
 from absl import flags
+from checkpoint_conversion_utils import extract_files_from_archive
+from checkpoint_conversion_utils import get_md5_checksum
 from tensorflow import keras
 
 import keras_nlp
-from tools.checkpoint_conversion.checkpoint_conversion_utils import (
-    get_md5_checksum,
-)
 
 PRESET_MAP = {
-    "xlm_roberta_base": ("xlmr.base", "xlm-roberta-base"),
-    "xlm_roberta_large": ("xlmr.large", "xlm-roberta-large"),
+    "xlm_roberta_base_multi": ("xlmr.base", "xlm-roberta-base"),
+    "xlm_roberta_large_multi": ("xlmr.large", "xlm-roberta-large"),
 }
 
 DOWNLOAD_SCRIPT_URL = "https://dl.fbaipublicfiles.com/fairseq/models/{}.tar.gz"
 
 EXTRACT_DIR = "./{}"
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string(
     "preset", None, f'Must be one of {",".join(PRESET_MAP.keys())}'
 )
 
 
-def download_model(preset, size):
+def download_model(size):
     print("-> Download original weights.")
     archive_file_path = keras.utils.get_file(
         fname=None,
         origin=DOWNLOAD_SCRIPT_URL.format(size),
-        cache_subdir=os.path.join("checkpoint_conversion", preset),
+        cache_subdir=os.path.join("checkpoint_conversion", FLAGS.preset),
     )
 
-    os.system(f"tar -xvf {archive_file_path}")
+    extract_files_from_archive(archive_file_path)
 
 
-def convert_checkpoints(preset, size):
+def convert_checkpoints(size):
     print("\n-> Convert original weights to KerasNLP format.")
     # XLM-RoBERTa paths.
     extract_dir = EXTRACT_DIR.format(size)
     checkpoint_path = os.path.join(extract_dir, "model.pt")
 
     # Load PyTorch XLM-R checkpoint.
     pt_ckpt = torch.load(checkpoint_path, map_location=torch.device("cpu"))
@@ -75,15 +74,15 @@
             .numpy()
             .shape[0]
         ),
     }
     print("Config:", cfg)
 
     keras_nlp_model = keras_nlp.models.XLMRobertaBackbone.from_preset(
-        preset, load_weights=False
+        FLAGS.preset, load_weights=False
     )
 
     # Embedding Layer.
     keras_nlp_model.get_layer("embeddings").token_embedding.embeddings.assign(
         pt_model["decoder.sentence_encoder.embed_tokens.weight"].numpy()
     )
     keras_nlp_model.get_layer(
@@ -242,21 +241,21 @@
         )._feedforward_layernorm.beta.assign(
             pt_model[
                 f"decoder.sentence_encoder.layers.{i}.final_layer_norm.bias"
             ].numpy()
         )
 
     # Save the model.
-    print(f"\n-> Save KerasNLP model weights to `{preset}.h5`.")
-    keras_nlp_model.save_weights(f"{preset}.h5")
+    print(f"\n-> Save KerasNLP model weights to `{FLAGS.preset}.h5`.")
+    keras_nlp_model.save_weights(f"{FLAGS.preset}.h5")
 
     return keras_nlp_model
 
 
-def define_preprocessor(preset, hf_model_name, size):
+def define_preprocessor(hf_model_name, size):
     print("\n-> Define the tokenizers.")
     extract_dir = EXTRACT_DIR.format(size)
     spm_path = os.path.join(extract_dir, "sentencepiece.bpe.model")
 
     keras_nlp_tokenizer = keras_nlp.models.XLMRobertaTokenizer(
         proto=spm_path,
     )
@@ -269,15 +268,14 @@
     print("\n-> Print MD5 checksum of the vocab files.")
     print(f"`{spm_path}` md5sum: ", get_md5_checksum(spm_path))
 
     return keras_nlp_preprocessor, hf_tokenizer
 
 
 def check_output(
-    preset,
     keras_nlp_model,
     keras_nlp_preprocessor,
     hf_model,
     hf_tokenizer,
 ):
     print("\n-> Check the outputs.")
     input_str = ["the quick brown fox ran, galloped and jumped."]
@@ -293,40 +291,39 @@
     hf_output = hf_model(**hf_inputs).last_hidden_state
 
     print("KerasNLP output:", keras_nlp_output[0, 0, :10])
     print("HF output:", hf_output[0, 0, :10])
     print("Difference:", np.mean(keras_nlp_output - hf_output.detach().numpy()))
 
     # Show the MD5 checksum of the model weights.
-    print("Model md5sum: ", get_md5_checksum(f"./{preset}.h5"))
+    print("Model md5sum: ", get_md5_checksum(f"./{FLAGS.preset}.h5"))
 
     return keras_nlp_output
 
 
 def main(_):
     assert (
         FLAGS.preset in PRESET_MAP.keys()
     ), f'Invalid preset {FLAGS.preset}. Must be one of {",".join(PRESET_MAP.keys())}'
     size = PRESET_MAP[FLAGS.preset][0]
     hf_model_name = PRESET_MAP[FLAGS.preset][1]
 
-    download_model(FLAGS.preset, size)
+    download_model(size)
 
-    keras_nlp_model = convert_checkpoints(FLAGS.preset, size)
+    keras_nlp_model = convert_checkpoints(size)
 
     print("\n-> Load HF model.")
     hf_model = transformers.AutoModel.from_pretrained(hf_model_name)
     hf_model.eval()
 
     keras_nlp_preprocessor, hf_tokenizer = define_preprocessor(
-        FLAGS.preset, hf_model_name, size
+        hf_model_name, size
     )
 
     check_output(
-        FLAGS.preset,
         keras_nlp_model,
         keras_nlp_preprocessor,
         hf_model,
         hf_tokenizer,
     )
```

### Comparing `keras-nlp-0.4.1.dev0/tools/count_preset_params.py` & `keras-nlp-0.5.0.dev0/tools/count_preset_params.py`

 * *Files identical despite different names*


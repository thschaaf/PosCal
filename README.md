# PosCal
Jung et al's ACL 2020 paper titled "Posterior Calibrated Training on Sentence Classification Tasks"

## Requirements
transformers (v 2.2.0)

## Running BERT + PosCal training on ShortRomance datsaet in xSLUE (Kang et al., 2019)
python classify_bert.py \
    --model_type bert \
    --model_name_or_path bert-base-uncased \
    --task_name ShortRomance \
    --do_train \
    --poscal_train \
    --data_dir $PATH/to/the/data \
    --output_dir $PATH/to/the/output

## Citation
    @inproceedings{jung20acl_poscal,
        title = {Posterior Calibrated Training on Sentence Classification Tasks},
        author = {Taehee Jung, Dongyeop Kang, Hua Cheng, Lucas Mentch, and Thomas Schaaf},
        booktitle = {2020 Annual Conference of the Association for Computational Linguistics (ACL)},
        url = {https://arxiv.org/abs/2004.14500},
        year = {2020}
    }

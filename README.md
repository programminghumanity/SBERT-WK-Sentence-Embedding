# SBERT-WK: A Sentence Embedding Method By Dissecting BERT-based Word Models

Pre-trained language models are quite powerful in a wide range of NLP tasks. But current models mostly provide word/token level representations. How to obtain good sentence representation from deep contextualized models remains challenging. Previous approaches includes averaging token representations or use CLS tokens provides rather poor performance in either textual similarity tasks, clustering and supervised tasks. In this work, we provide a new approach in finding sentence representations by dissecting deep contextualized models. Through geometric analysis, our model is capable in finding salient components in representation arocss layers and unified token representations. We evaluate our approach on a wide range of tasks and showed its effectiveness.

Note that our model is not focus on further tuning with sentence objective. But find ways to merge the learned token representation across layers and compute sentence embedding with better quality.

Details of our method can be found in our publication: [SBERT-WK]()

## Setup
We are using Python 3.7 and the model is implemented with Pytorch 1.3.

For backbone models: we use 
[transformers v2.2.1](https://github.com/huggingface/transformers)

```
    conda create -n SBERT-WK python=3.7
    conda install numpy
    conda install pytorch=1.3 torchvision cudatoolkit=10.1 -c pytorch
    pip install transformers==2.2.1
    conda install -c anaconda scikit-learn
```

## Get Started to Duplicate the result from the Paper



## Performance



## Citing and Authors
If you find our model is useful in your research, please consider cite our paper: [SBERT-WK: A Sentence Embedding Method By Dissecting BERT-based Word Models](https://arxiv.org/abs/xx.xx):

``` 
@inproceedings{xxx,
    title = "SBERT-WK: A Sentence Embedding Method By Dissecting BERT-based Word Models",
    author = "xxx",
    booktitle = "xx",
}
```

Contact person: Bin Wang, bwang28c@gmail.com

http://mcl.usc.edu/



## Acknowledge

Many thanks for [Transformer repo](https://github.com/huggingface/transformers) and [Sentence-BERT repo](https://github.com/UKPLab/sentence-transformers) in providing pretained models and easy to use architecture.
Thanks for SentEval for evlaluation toolkit. [SentEval](https://github.com/facebookresearch/SentEval)

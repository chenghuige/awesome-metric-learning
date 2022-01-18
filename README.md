# awesome-metric-learning
😎 Awesome list about practical Metric Learning and its applications

## Motivation 🤓
At Qdrant, we have one goal: make metric learning more practical. This listing is in line with this purpose, and we aim at providing a concise yet useful list of awesomeness around metric learning. It is intended to be inspirational for productivity rather than serve as a full bibliography.

If you find it useful, or like it in some other way, you may want to join our Discord server where we are running a paper reading club on metric learning.

<p align=center>
    <a href="https://discord.gg/tdtYvXjC4h"><img src="https://img.shields.io/badge/Discord-Qdrant-5865F2.svg?logo=discord" alt="Discord"></a>
</p>


## Surveys 📖
- [What is Metric Learning?](http://contrib.scikit-learn.org/metric-learn/introduction.html)
> A beginner-friendly starting point for traditional metric learning methods from scikit-learn website.

<details>
<summary>More...</summary>

It has proceeding guides for [supervised](http://contrib.scikit-learn.org/metric-learn/supervised.html), [weakly supervised](http://contrib.scikit-learn.org/metric-learn/weakly_supervised.html) and [unsupervised](http://contrib.scikit-learn.org/metric-learn/unsupervised.html) metric learning algorithms in [`metric_learn`](http://contrib.scikit-learn.org/metric-learn/metric_learn.html) package.
</details>

- [Deep Metric Learning: A Survey](https://www.mdpi.com/2073-8994/11/9/1066/htm)
> A comprehensive study for newcomers. 

<details>
<summary>More...</summary>

Factors such as sampling strategies, distance metrics and network structures are systematically analyzed by comparing the quantitative results of the methods.
</details>

- [Deep Metric Learning: A (Long) Survey](https://hav4ik.github.io/articles/deep-metric-learning-survey)
> An intuitive survey of the state-of-the-art.

<details>
<summary>More...</summary>

It discusses the need for metric learning, old and state-of-the-art approaches, and some real world use cases.
</details>

- [A Tutorial on Distance Metric Learning: Mathematical Foundations, Algorithms, Experimental Analysis, Prospects and Challenges (with Appendices on Mathematical Background and Detailed Algorithms Explanation)](https://arxiv.org/abs/1812.05944)
> Intended for those interested in mathematical foundations of metric learning.


## Applications ⚒️
- [CLIP](https://github.com/openai/CLIP)
> Training a unified vector embedding for image and text. 

<details>
<summary>More...</summary>

CLIP offers state-of-the-art zero-shot image classification and image retrieval with a natural language query. See [demo](https://colab.research.google.com/github/openai/clip/blob/master/notebooks/Interacting_with_CLIP.ipynb).
</details>

- [Wav2CLIP](https://github.com/descriptinc/lyrebird-wav2clip)
> Encoding audio into the same vector space as CLIP.

<details>
<summary>More...</summary>

This work achieves  zero-shot classification and cross-modal retrieval of audio from natural language queries.
</details>

- [Detic](https://github.com/facebookresearch/Detic)
> Code released for ["Detecting Twenty-thousand Classes using Image-level Supervision"](https://arxiv.org/abs/2201.02605).
<details>
<summary>More...</summary>

It is an open-class object detector to detect any label encoded by CLIP without finetuning. See [demo](https://huggingface.co/spaces/akhaliq/Detic).
</details>

- [BERTopic](https://github.com/MaartenGr/BERTopic)
> A novel topic modeling toolkit with BERT embeddings.

<details>
<summary>More...</summary>

It leverages HuggingFace Transformers and c-TF-IDF to create dense clusters allowing for easily interpretable topics whilst keeping important words in the topic descriptions. It supports guided, (semi-) supervised, and dynamic topic modeling beautiful visualizations.
</details>

- [Embedding Projector](https://projector.tensorflow.org/)
> A web-based tool to visualize high-dimensional data.

<details>
<summary>More...</summary>

It supports UMAP, T-SNE, PCA or custom techniques to analyze embeddings of encoders.
</details>


## Libraries 🧰
- [sentence-transformers](https://github.com/UKPLab/sentence-transformers)
> A library for sentence-level embeddings.
<details>
<summary>More...</summary>

Developed on top of the well known [Transformers](https://github.com/huggingface/transformers) library, it provides an easy way to finetune Transformer-based models to obtain sequence-level embeddings.
</details>

- [pytorch-metric-learning](https://github.com/KevinMusgrave/pytorch-metric-learning)
> A modular library implementing losses, miners, samplers and trainers in PyTorch.

- [tensorflow-similarity](https://github.com/tensorflow/similarity)
> A metric learning library in TensorFlow with a Keras-like API.

<details>
<summary>More...</summary>

It provides support for self-supervised contrastive learning and state-of-the-art methods such as SimCLR, SimSian and Barlow Twins.
</details>

- [sense2vec](https://github.com/explosion/sense2vec)
> Contextually keyed word vectors.
<details>
<summary>More...</summary>

A PyTorch library to train, and inference with, contextually-keyed word vectors that are augmented with part-of-speech tags to achieve multi-word queries.
</details>

- [lightly](https://github.com/lightly-ai/lightly)
> A Python library for self-supervised learning on images.

<details>
<summary>More...</summary>

> A PyTorch library to efficiently train self-supervised computer vision models with state-of-the-art techniques such as SimCLR, SimSian, Barlow Twins,  BYOL among others.
</details>

- [LightFM](https://linkedin.com/)
> A Python implementation of a number of popular recommender algorithms.
<details>
<summary>More...</summary>

 It supports to incorpoarate user and item features to the traditional matrix factorization. It represents users and items as a sum of the latent representations of their features, thus achieving a better generalization.
</details>

## Papers 🔬
- [Dimensionality Reduction by Learning an Invariant Mapping](http://yann.lecun.com/exdb/publis/pdf/hadsell-chopra-lecun-06.pdf)
> First appearance of Contrastive Loss.

<details>
<summary>More...</summary>

Published by Yann Le Cun et al. (2005), its main focus was on dimensionality reduction. However, the method proposed has excellent properties for metric learning such as preserving neighbourhood relationships and generalization to unseen data, and it has extensive applications with a great number of variations ever since. It is advised that you read [this great post](https://medium.com/@maksym.bekuzarov/losses-explained-contrastive-loss-f8f57fe32246) to better understand its importance for metric learning.
</details>

- [FaceNet: A Unified Embedding for Face Recognition and Clustering](https://arxiv.org/abs/1503.03832)
> First appearance of Triplet Loss.

<details>
<summary>More...</summary>

The paper introduces Triplet Loss, which can be seen as the "ImageNet moment" for deep metric learning. It is still one of the state-of-the-art methods, and has a great number of applications in almost any data modalities.
</details>

- [In Defense of the Triplet Loss for Person Re-Identification](https://arxiv.org/abs/1703.07737)
> It shows that triplet sampling matters and proposes to use batch-hard samples.

- [Deep Metric Learning with Angular Loss](https://arxiv.org/abs/1708.01682)
> A novel loss function with better properties.
<details>
<summary>More...</summary>

It provides scale invariance, robustness against feature variance, and better convergence than Contrastive and Triplet Loss.
</details>

- [ArcFace: Additive Angular Margin Loss for Deep Face Recognition](https://arxiv.org/abs/1801.07698)
> Supervised metric learning without pairs or triplets.

<details>
<summary>More...</summary>

Although it is originally designed for the face recognition task, this loss function achieves state-of-the-art results in many other metric learning problems with a simpler and faster data feeding. It is also robust against unclean and unbalanced data when modified with sub-centers and a dynamic margin.
</details>

- [Learning Distance Metrics from Probabilistic Information](https://cse.buffalo.edu/~lusu/papers/TKDD2020.pdf)
> Working with datasets that contain probabilistic labels instead of deterministic values.

- [VICReg: Variance-Invariance-Covariance Regularization for Self-Supervised Learning](https://arxiv.org/abs/2105.04906)
> Better regularization for high-dimensional embeddings.

<details>
<summary>More...</summary>

The paper introduces a method that explicitly avoids the collapse problem in high dimensions with a simple regularization term on the variance of the embeddings along each dimension individually. This new term can be incorporated into other methods for stabilization of the training and performance improvements.
</details>

- [On the Unreasonable Effectiveness of Centroids in Image Retrieval](https://arxiv.org/abs/2104.13643)
> Higher robustness against outliers with better efficiency.

<details>
<summary>More...</summary>

The paper proposes to use the mean centroid representation both during training and retrieval for robustness against outliers, and more stable features. It further reduces retrieval time and storage requirements, so it is suitable for production deployments.
</details>

- [TSDAE: Using Transformer-based Sequential Denoising Auto-Encoder for Unsupervised Sentence Embedding Learning](https://arxiv.org/abs/2104.06979)
> A SOTA method to learn domain-specific sentence-level embeddings from unlabelled data.


## Datasets ℹ️
> Any labelled or unlabelled data can be used for metric learning with an appropriate method chosen. However some datasets are particularly important in the literature for benchmarking or in some other way, and we list them in this section.

- [SNLI](https://nlp.stanford.edu/projects/snli/)
> The Stanford Natural Language Inference Corpus, serving as a useful benchmark.

<details>
<summary>More...</summary>

Containing pairs of sentences labelled as `contradiction`, `entailment` and `neutral` regarding their semantic relationships, this dataset is used to train semantic search models in metric learning.
</details>

- [MultiNLI](https://cims.nyu.edu/~sbowman/multinli/)
> NLI corpus with samples from multiple genres.

<details>
<summary>More...</summary>

Modeled on the SNLI corpus, the dataset contains sentence pairs from a range of genres of spoken and written text, and it also offers a distinctive cross-genre generalization evaluation.
</details>

- [Google Landmark Recognition 2019](https://www.kaggle.com/c/landmark-recognition-2019)
> Label famous (and no so famous) landmarks from images.
<details>
<summary>More...</summary>

Shared as a part of a Kaggle competition by Google, this dataset is more diverse and thus more interesting than the first version.
</details>

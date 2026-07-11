<div align="center">
  <img src="../assets/logo.svg" width="150" alt="hyper³labs logo" />
  <h1>hyper³labs</h1>
  <p><strong>Embedding models and retrieval infrastructure.</strong></p>
  <p>
    <a href="https://hyper3labs.com">Website</a> ·
    <a href="https://huggingface.co/hyper3labs">Hugging Face</a>
  </p>
</div>

hyper³labs (pronounced *Hypercube Labs*) builds embedding models and retrieval infrastructure across text and vision. We also build open-source tools for evaluating and understanding embedding systems.

We are especially interested in how hierarchy and non-Euclidean geometry affect retrieval, and in the failures that aggregate benchmark scores hide.

## Models

- [hyper3-clip-v0.5](https://huggingface.co/hyper3labs/hyper3-clip-v0.5) is an open-weight vision-language embedding model for hierarchy-sensitive retrieval.

## Open-source tools

- [HyperView](https://github.com/Hyper3Labs/HyperView) is a workbench for exploring embedding spaces and tracing retrieval failures back to real samples.
- [hyper-models](https://github.com/Hyper3Labs/hyper-models) provides loaders and shared interfaces for non-Euclidean embedding models.
- [hyper-scatter](https://github.com/Hyper3Labs/hyper-scatter) is a WebGL scatterplot engine for large Euclidean and Poincaré embedding layouts.
- [hyper-lrp](https://github.com/Hyper3Labs/hyper-lrp) contains attribution experiments for CLIP-style models.

## Research and datasets

- [Are We Recognizing the Jaguar or Its Background?](https://arxiv.org/abs/2604.09690) studies failure modes in jaguar re-identification.
- [jaguar-re-id](https://huggingface.co/datasets/hyper3labs/jaguar-re-id) contains images and metadata used for individual jaguar identification.

<div align="center">
  <img src="../assets/logo.svg" width="150" alt="hyper³labs logo" />
  <h1>hyper³labs</h1>
  <p><strong>Embedding models and retrieval infrastructure.</strong></p>
  <p>
    <a href="https://hyper3labs.com">Website</a> ·
    <a href="https://hyper3labs.github.io/spaces/abo-catalog/">Explore a Space</a> ·
    <a href="https://huggingface.co/hyper3labs">Hugging Face</a>
  </p>
</div>

hyper³labs (pronounced *Hypercube Labs*) builds embedding models and retrieval
infrastructure across text and vision. We also build open-source tools for
evaluating and understanding embedding systems.

We are especially interested in how hierarchy and non-Euclidean geometry affect
retrieval, and in the failures that aggregate benchmark scores hide.

## Explore the failures yourself

Aggregate scores tell you a retrieval system is 57% accurate. They do not tell
you which query put a near-miss above the exact match, or why. Each Space below
is a complete, read-only workbench over one corpus: open it in a browser, no
install and no backend, and inspect the ranked results, the embedding topology,
and the individual samples behind every number.

| Space | The question it answers |
| --- | --- |
| [ABO Catalog](https://hyper3labs.github.io/spaces/abo-catalog/) | Does the model find the right product, not just a plausible category match? |
| [Fashion Products](https://hyper3labs.github.io/spaces/fashion-products/) | Does the exact SKU reach the shopper's first screen? |
| [Precision Regions](https://hyper3labs.github.io/spaces/precision-regions/) | Does the exact region reach the operator's first screen? |
| [Logo Search](https://hyper3labs.github.io/spaces/logo-search/) | Which existing logo best satisfies a detailed creative brief? |
| [GeoSpatial](https://hyper3labs.github.io/spaces/geospatial/) | Do retrieved neighbours preserve land-use identity? |
| [Visual Safety](https://hyper3labs.github.io/spaces/visual-safety/) | Is one extra catch worth five false reviews and six more queue slots? |

Every Space compares `hyper3-clip-v0.5` against OpenAI CLIP ViT-B/32 on the same
bounded probe, and shows the per-case evidence for both — including the cases
CLIP wins.

## Models

- [hyper3-clip-v0.5](https://huggingface.co/hyper3labs/hyper3-clip-v0.5) is an
  open-weight vision-language embedding model for hierarchy-sensitive retrieval.

## Open-source tools

- [HyperView](https://github.com/Hyper3Labs/HyperView) is a workbench for
  exploring embedding spaces and tracing retrieval failures back to real
  samples. It runs locally, drives the same workspace from a CLI for coding
  agents, and exports any workspace as a static bundle like the ones above.
- [hyperview-spaces](https://github.com/Hyper3Labs/hyperview-spaces) holds the
  source for those Spaces — copy a folder, point it at your own dataset.
- [hyper-models](https://github.com/Hyper3Labs/hyper-models) provides loaders
  and shared interfaces for non-Euclidean embedding models.
- [hyper-scatter](https://github.com/Hyper3Labs/hyper-scatter) is a WebGL
  scatterplot engine for large Euclidean and Poincaré embedding layouts.
- [hyper-lrp](https://github.com/Hyper3Labs/hyper-lrp) contains attribution
  experiments for CLIP-style models.

## Research and datasets

- [Are We Recognizing the Jaguar or Its Background?](https://arxiv.org/abs/2604.09690)
  studies failure modes in jaguar re-identification.
- [jaguar-re-id](https://huggingface.co/datasets/hyper3labs/jaguar-re-id)
  contains images and metadata used for individual jaguar identification.

## Run this on your own data

The Spaces above are bounded probes on public corpora. Whether the same
structure holds for your catalog, asset library, or inspection archive is an
empirical question, and the fastest way to answer it is to run the eval.
Get in touch through [hyper3labs.com](https://hyper3labs.com).

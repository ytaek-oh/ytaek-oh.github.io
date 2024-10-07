---
layout: none
title: FSC-CLIP
permalink: /fsc-clip
description: We present a novel framework to increase compositional reasoning in pre-trained vision and language models (VLMs) without sacrificing the multi-modal capabilities..
keywords: "image text matching, cross-modal application, multimodality"
title: "Preserving Multi-Modal Capabilities of Pre-trained VLMs for Improving Vision-Linguistic Compositionality"
venue: "<b>EMNLP 2024 (Long, Main)</b>"
arxiv: 
code: https://github.com/ytaek-oh/fsc-clip
model: https://huggingface.co/ytaek-oh/fsc-clip
slide: 
poster: 
bibtex: >
  @inproceedings{oh2024preserving<br />&nbsp;&nbsp;TBU<br />}
abstract: >
  <p>
  In this paper, we propose a new method to enhance compositional understanding in pre-trained vision and language models (VLMs) without sacrificing performance in zero-shot multi-modal tasks.
  </p>
  <p>
    Traditional fine-tuning approaches often improve compositional reasoning at the cost of degrading multi-modal capabilities, primarily due to the use of global hard negative (HN) loss, which contrasts global representations of images and texts. This global HN loss pushes HN texts that are highly similar to the original ones, damaging the model’s multi-modal representations. 
  </p>
  <p>
    To overcome this limitation, we propose Fine-grained Selective Calibrated CLIP (FSC-CLIP), which integrates local hard negative loss and selective calibrated regularization. These innovations provide fine-grained negative supervision while preserving the model’s representational integrity. 
  </p>
  <p>
    Our extensive evaluations across diverse benchmarks for both compositionality and multi-modal tasks show that FSC-CLIP not only achieves compositionality on par with state-of-the-art models but also retains strong multi-modal capabilities.
  </p>
---

<html>
<head>
  <meta charset="utf-8">
  <meta name="description"
        content="{{ page.description }}">
  <meta name="keywords" content="{{ page.keywords }}">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>{{ page.title }}</title>

  <!-- Global site tag (gtag.js) - Google Analytics -->
  {% include scripts/analytics.html %}
  <!-- mathjax -->
  <script type="text/x-mathjax-config"> 
    MathJax.Hub.Config({ tex2jax: { inlineMath: [ ['$','$'], ["\\(","\\)"] ], processEscapes: true } }); 
  </script>
  <script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML'></script>
  <!--/ mathjax -->
  <link href="https://fonts.googleapis.com/css?family=Inter" rel="stylesheet">

  <link rel="stylesheet" href="./assets/nerfies/css/bulma.min.css">
  <link rel="stylesheet" href="./assets/nerfies/css/bulma-carousel.min.css">
  <link rel="stylesheet" href="./assets/nerfies/css/bulma-slider.min.css">
  <link rel="stylesheet" href="./assets/nerfies/css/fontawesome.all.min.css">
  <link rel="stylesheet"
        href="https://cdn.jsdelivr.net/gh/jpswalsh/academicons@1/css/academicons.min.css">
  <link rel="stylesheet" href="./assets/nerfies/css/index.css">

  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script defer src="./assets/nerfies/js/fontawesome.all.min.js"></script>
  <script src="./assets/nerfies/js/bulma-carousel.min.js"></script>
  <script src="./assets/nerfies/js/bulma-slider.min.js"></script>
  <script src="./assets/nerfies/js/index.js"></script>
  <style>
      body {
          font-family: 'Inter', sans-serif;
      }
      .subtitle {
          font-family: 'Times', serif;
      }
  </style>
</head>
<body>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>
  <div class="navbar-menu">
    <div class="navbar-start" style="flex-grow: 1; justify-content: center;">
      <a class="navbar-item" href="https://ytaek-oh.github.io">
      <span class="icon">
          <i class="fas fa-home"></i>
      </span>
      </a>
    </div>
  </div>
</nav>

<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-3 publication-title">{{ page.title }}</h1>
          <div class="is-size-5 publication-authors">
            <span class="author-block">
              <a href="https://ytaek-oh.github.io">Youngtaek Oh</a><sup>1</sup>&nbsp;&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block">
              <a href="https://chojw.github.io/">Jae Won Cho</a><sup>2</sup>&nbsp;&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block">
              <a href="https://sites.google.com/site/djkimcv/">Dong-Jin Kim</a><sup>3</sup>&nbsp;&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block">
              <a href="#">In So Kweon</a><sup>1</sup>*&nbsp;&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block">
              <a href="#">Junmo Kim</a><sup>1</sup>*</span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>KAIST</span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            <span class="author-block"><sup>2</sup>Sejong University</span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            <span class="author-block"><sup>3</sup>Hanyang University</span>
          </div>
          <div class="is-size-6 publication-authors">
            <span class="author-block">(*Corresponding authors)</span>
          </div>
          <div class="column has-text-centered">
            <div class="publication-links">
              <!-- PDF Link. -->
              {%- if page.pdf %}
              <span class="link-block">
                <a href="{{ page.pdf }}" target="_blank"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fas fa-file-pdf"></i>
                  </span>
                  <span>Paper</span>
                </a>
              </span>
              {%- endif %}
              {%- if page.arxiv %}
              <span class="link-block">
                <a href="{{ page.arxiv }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="ai ai-arxiv"></i>
                  </span>
                  <span>arXiv</span>
                </a>
              </span>
              {%- endif %}
              {%- if page.video %}
              <!-- Video Link. -->
              <span class="link-block">
                <a href="{{ page.video }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fab fa-youtube"></i>
                  </span>
                  <span>Video</span>
                </a>
              </span>
              {%- endif %}
              {%- if page.code %}
              <!-- Code Link. -->
              <span class="link-block">
                <a href="{{ page.code }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fab fa-github"></i>
                  </span>
                  <span>Code</span>
                  </a>
              </span>
              {%- endif %}
              {%- if page.model %}
              <span class="link-block">
                <a href="{{ page.model }}"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      &#129303;
                  </span>
                  <span>Models</span>
                  </a>
              </span>
              {%- endif %}
              {%- if page.slide %}
              <!-- slide Link. -->
              <span class="link-block">
                <a href="{{ page.slide | prepend: '/assets/daso/' }}" target="_blank"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="far fa-file-powerpoint"></i>
                  </span>
                  <span>Slides</span>
                  </a>
              </span>
              {%- endif %}
              {%- if page.poster %}
              <!-- poster Link. -->
              <span class="link-block">
                <a href="{{ page.poster | prepend: '/assets/daso/' }}" target="_blank"
                   class="external-link button is-normal is-rounded is-dark">
                  <span class="icon">
                      <i class="fas fa-file-powerpoint"></i>
                  </span>
                  <span>Poster</span>
                  </a>
              </span>
              {%- endif %}
            </div>
          </div>
          <div class="column has-text-centered">
            <div class="is-size-5 publication-authors">
              {{ page.venue }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- conctent -->
<!-- project_page.html -->
<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <img src="assets/fsc-clip/retrieval.png"/>
      <h2 class="subtitle has-text-centered is-size-5" style="padding-top: 1rem;">
        <b>Image to text retrieval examples on COCO-Counterfactuals.</b> 
        Ours consistently retrieves correct captions against the negatives, demonstrating superior compositional reasoning during retrieval.
      </h2>
    </div>
  </div>
</section>
<section class="section">
  <div class="container is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
          {{ page.abstract }}
        </div>
      </div>
    </div>
    <!--/ Abstract. -->
  </div>
</section>

<!-- Introduction -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Introduction</h2> 
        <div class="content has-text-justified">
          <p>
            Compositional reasoning remains a challenge for vision-language models (VLMs) like CLIP, which struggle to understand complex and fine-grained relationships between images and text. Current fine-tuning methods aimed at improving compositionality often reduce performance in multi-modal tasks. This trade-off is mainly due to global hard negative loss applied to single vector representations, which fails to capture subtle differences between similar texts.
          </p>
        </div>
        <div class="columns is-centered is-vcentered">
          <!-- figure -->
          <div class="column">
            <img src="assets/fsc-clip/teaser.png"/>
          </div>
          <!--/ figure -->
          <!-- caption -->
          <div class="column">
              <h2 class="subtitle">
                 <b>Holistic comparison of fine-tuning methods.</b> Enhancing compositional reasoning often degrades multi-modal task performances in previous models. Our $\texttt{FSC-CLIP}$ bridges this gap, minimizing these trade-offs.
              </h2>
              <h2 class="subtitle">               
The models are evaluated across 11 compositionality tasks, 21 zero-shot classification tasks, and 3 image-text retrieval tasks.
              </h2>
          </div>
          <!--/ caption -->
        </div>
        <div class="content has-text-justified">
          <p>
            To overcome this limitation, we introduce $\texttt{FSC-CLIP}$, a new fine-tuning method for CLIP designed to enhance compositional reasoning without sacrificing multi-modal task performance. By incorporating <b>local hard negative loss</b> and <b>selective calibrated regularization</b>, our approach provides fine-grained supervision while preserving the integrity of multi-modal representations.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>
<!--/ introduction -->

<!-- motivation -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Method</h2> 
        <div class="content has-text-justified">
          <p>
Our method is designed to fine-tune CLIP using hard negative captions, incorporating Local Hard Negative (LHN) Loss and Selective Calibrated Regularization (SCR) to improve compositional understanding while preserving multi-modal performance.
          </p>
        </div>
        <!-- figure -->
        <div style="margin-bottom: 3rem;">
          <img src="assets/fsc-clip/framework.png"/>
          <h2 class="subtitle has-text-centered is-size-5" style="padding-top: 1rem;">
            <b>Overall $\texttt{FSC-CLIP}$ framework.</b> It integrates <b>Local Hard Negative (LHN) Loss</b> and <b>Selective Calibrated Regularization (SCR)</b>, in addition to a global hard negative loss. The LHN loss captures similarities between image patches and text tokens, enabling finer differentiation between original and hard negative texts. SCR combines focal loss with label smoothing, effectively reducing the negative impact of hard negative losses.
          </h2>
        </div>
        <!-- figure -->
        <div class="content has-text-justified">
          <h3 class="title is-5">Local Hard Negative (LHN) Loss</h3>
          <li>The goal is to improve fine-grained image-text alignment by focusing on token-patch level representations. This approach captures subtle differences between the original and hard negative (HN) texts that are often missed when using global similarity alone.</li>
          <li>LHN loss captures local similarity between image patches and text tokens. By aggregating the token-level similarities, it enhances the model's ability to differentiate between original and hard negative texts, leading to more effective hard negative loss computation.</li>
          <h3 class="title is-5">Selective Calibrated Regularization (SCR)</h3>
          <li>Hard negative texts are often too similar to original texts, potentially degrading representations through HN loss. SCR addresses this by selectively focusing on challenging HN samples and adjusting label assignments to account for the potential positiveness in hard negative texts.</li>
          <li>SCR combines focal loss, which emphasizes harder-to-classify HN samples, with label smoothing, which assigns a slight positive margin to account for the potential correctness of HN texts. This approach mitigates the adverse effects of HN losses, preserving model integrity while enhancing the learning of compositionality.</li>
          <h3 class="title is-5">Training Objective</h3>
          <div class="content has-text-justified">
            $\texttt{FSC-CLIP}$ combines the standard CLIP loss ($\mathcal{L}_{\text{clip}}$) with global HN loss ($\mathcal{L}^{g}_{neg}$) and local HN loss ($\mathcal{L}^{l}_{neg}$). Both HN losses incorporate SCR, which uses focal loss and label smoothing to keep representation integrity.
          </div>
          <div class="content has-text-centered">
$\mathcal{L}_{\text{total}} = \mathcal{L}_{\text{clip}} + \lambda_g \mathcal{L}^{g}_{neg} + \lambda_l \mathcal{L}^{l}_{neg}.$
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
<!--/ motivation -->

<!-- Results -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Experiments</h2> 
        <h3 class="title is-5">Highlights</h3>
        <div class="content has-text-justified">
          <li>We fine-tune our model using three image-text datasets (COCO, CC-3M, LAION-COCO), each with 100K randomly sampled subset.</li>
          <li>We provide a comprehensive evaluation of methods across 11 compositionality benchmarks, 21 zero-shot classification tasks, and 3 image-text retrieval tasks.</li>
          <li>$\texttt{FSC-CLIP}$ enhances compositionality to a level comparable to the high-performing DAC-LLM, while simultaneously maintaining strong multi-modal task performance.</li>
        </div>
        <!-- figure -->
        <div style="margin-bottom: 0rem;">
          <img src="assets/fsc-clip/table.png"/>
          <h2 class="subtitle has-text-centered is-size-5" style="padding-top: 1rem;">
            <b>A holistic comparison of fine-tuning methods applied to the pre-trained CLIP ViT-B/32 model.</b> $\texttt{FSC-CLIP}$ achieves superior compositionality scores while maintaining strong multi-modal task performances. For each fine-tuning dataset, the best numbers are $\textbf{bold}$, and the second-best numbers are $\underline{\text{underlined}}$.
          </h2>
        </div>
        <!-- figure -->
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container is-max-desktop">
    <!-- Concurrent Work. -->
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Related Links</h2>
        <div class="content has-text-justified">
          <p>
            Also, please check out our <a href="https://github.com/ytaek-oh/vl_compo">$\texttt{vl-compo}$</a> package, which enabled the comprehensive evaluation across diverse tasks in our work. It supports evaluations for a wide range of compositional and multi-modal task benchmarks, integrating various pre-trained and fine-tuned VLMs, and is continuously evolving.
          </p>
        </div>
        <div class="columns is-centered is-vcentered">
          <!-- figure -->
          <div class="column">
            <img src="assets/fsc-clip/spectrum.png"/>
          </div>
          <!--/ figure -->
          <!-- caption -->
          <div class="column">
              <h2 class="subtitle">
                 <b>Overall trends in pre-trained and fine-tuned CLIP models,</b> covering 274 model checkpoints across 12 compositional reasoning tasks and 21 zero-shot classification tasks.
              </h2>
              <h2 class="subtitle">
               All the models and benchmarks used for evaluation are integrated into our $\texttt{vl-compo}$ package.
              </h2>
          </div>
          <!--/ caption -->
        </div>
      </div>
    </div>
    <!--/ Concurrent Work. -->
  </div>
</section>
<!-- end content -->

{%- if page.bibtex %}
<section class="section" id="BibTeX">
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <p>
      If you find our work useful for your research, please cite with the following bibtex:
    </p>
    <pre><code>{{ page.bibtex }}</code></pre>
  </div>
</section>
{%- endif %}

<footer class="footer">
  <div class="container">
    <div class="content has-text-centered">
      {%- if page.pdf %}
      <a class="icon-link"
         href="{{ page.pdf }}">
        <i class="fas fa-file-pdf"></i>
      </a>
      {%- endif %}
      {%- if page.code %}
      <a class="icon-link" href="{{ page.code }}" class="external-link" disabled>
        <i class="fab fa-github"></i>
      </a>
      {%- endif %}
    </div>
    <div class="columns is-centered">
      <div class="column is-8">
        <div class="content">
          <p>This website is based on the <a href="https://github.com/nerfies/nerfies.github.io">Nerfies website template</a>,
            which is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative
            Commons Attribution-ShareAlike 4.0 International License</a>.
          </p>
        </div>
      </div>
    </div>
  </div>
</footer>

</body>
</html>

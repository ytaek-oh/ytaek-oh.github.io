---
layout: none
permalink: /daso
description: A new framework DASO, Distribution-Aware Semantics-Oriented Pseudo-label alleviates biases in pseudo-labels under diverse imbalanced semi-supervised learning scenarios.
keywords: "Semi-supervised learning, Class-imbalanced learning, Long-tailed distribution"
title: "DASO: Distribution-Aware Semantics-Oriented Pseudo-label for Imbalanced Semi-Supervised Learning"
venue: "IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR 2022)"
pdf: https://openaccess.thecvf.com/content/CVPR2022/html/Oh_DASO_Distribution-Aware_Semantics-Oriented_Pseudo-Label_for_Imbalanced_Semi-Supervised_Learning_CVPR_2022_paper.html
arxiv: https://arxiv.org/abs/2106.05682
code: https://github.com/ytaek-oh/daso
slide: slide.pdf
poster: poster.pdf
bibtex: >
  @inproceedings{oh2022daso, <br />
  &nbsp;&nbsp; title={DASO: Distribution-Aware Semantics-Oriented Pseudo-label for Imbalanced Semi-Supervised Learning}, <br />
  &nbsp;&nbsp; author={Oh, Youngtaek and Kim, Dong-Jin and Kweon, In So}, <br />
  &nbsp;&nbsp; booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)}, <br />
  &nbsp;&nbsp; year={2022}, <br />
  &nbsp;&nbsp; pages={9786-9796} <br />
  }
abstract: >
  <p>
    The capability of the traditional semi-supervised learning (SSL) methods is far from real-world application due to severely biased pseudo-labels caused by (1) class imbalance and (2) class distribution mismatch between labeled and unlabeled data.
  </p>
  <p>
    This paper addresses such a relatively under-explored problem. First, we propose a general pseudo-labeling framework that class-adaptively blends the semantic pseudo-label from a similarity-based classifier to the linear one from the linear classifier, after making the observation that both types of pseudo-labels have complementary properties in terms of bias. We further introduce a novel semantic alignment loss to establish balanced feature representation to reduce the biased predictions from the classifier. 
    We term the whole framework as Distribution-Aware Semantics-Oriented (DASO) Pseudo-label.
  </p>
  <p>
    We conduct extensive experiments in a wide range of imbalanced benchmarks: CIFAR10/100-LT, STL10-LT, and large-scale long-tailed Semi-Aves with open-set class, and demonstrate that, the proposed DASO framework reliably improves SSL learners with unlabeled data especially when both (1) class imbalance and (2) distribution mismatch dominate.
  </p>
---


<!DOCTYPE html>
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
  <link href="https://fonts.googleapis.com/css?family=Google+Sans|Noto+Sans|Castoro" rel="stylesheet">

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
          <div class="is-size-4 publication-authors">
            <span class="author-block">
              <a href="https://ytaek-oh.github.io">Youngtaek Oh</a><sup>1</sup>,</span>
            <span class="author-block">
              <a href="https://sites.google.com/site/djkimcv/">Dong-Jin Kim</a><sup>2</sup>,</span>
            <span class="author-block">
              <a href="#">In So Kweon</a><sup>1</sup>,
            </span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>KAIST, South Korea.</span>
            <span class="author-block"><sup>2</sup>UC Berkeley / ICSI, CA.</span>
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
<!-- project_page.html -->
<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <video id="teaser" autoplay muted loop playsinline height="100%">
        <source src="assets/daso/daso.mp4" type="video/mp4">
      </video>
      <h2 class="subtitle has-text-centered is-size-5">
        DASO framework for debiasing pseudo-labels by blending two complementary pseudo-labels.
        Semantic alignment loss further alleviates the bias with balanced feature representations.
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
            Many real-world datasets exhibit <i>long-tailed</i> distributions. With such class imbalanced data, semi-supervised learning (SSL) methods produce biased pseudo-labels, which can further bias the model during training.
            The bias of pseudo-labels also depends on <i>class distribution mismatch</i> between labeled and unlabeled data, in addition to the class-imbalance.
          </p>
        </div>
        <div class="hero-body">
          <div class="columns is-centered is-vcentered">
            <!-- figure -->
            <div class="column">
              <img src="assets/daso/teaser.PNG"/>
            </div>
            <!--/ figure -->
            <!-- caption -->
            <div class="column">
                <h2 class="subtitle has-text-justified">
                  DASO reduces overall bias in pseudo-labels caused by imbalanced data, by blending two complementary pseudo-labels from different classifiers. We conceptually illustrate the bias as relative pseudo-label size, meaning that pseudo-label size is normalized by the actual label size.
                </h2>
            </div>
            <!--/ caption -->
          </div>
        </div>
        <div class="content has-text-justified">
          <p>
            We present a new imbalanced SSL method for debiasing pseudo-labels under class-imbalanced data, while discarding the common assumption that class distributions of labeled data and unlabeled data are identical. 
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
        <h2 class="title is-3">Motivation</h2> 
        <div class="content has-text-justified">
          <p>
            We observe that semantic pseudo-labels from a similarity-based classifier are biased towards minority classes as opposed to linear classifier-based pseudo-labels being biased towards head classes.
          </p>
          <p>
            FixMatch and USADTM are recent methods that learn solely from linear pseudo-labels and semantic pseudo-labels, respectively.
          </p>
        </div>
        <div class="hero-body">
          <img src="assets/daso/motivation.png"/>
          <h2 class="my-1 subtitle has-text-centered">
            Although USADTM improves the recall of minority classes in (a), the precision of those classes is significantly reduced compared to FixMatch in (b). DASO improves the recall of minority classes while maintaining the precision, leading to higher test accuracy.
          </h2>
        </div>
        <div class="content has-text-justified">
          <p>
            Based on the observation, we exploit the linear and semantic pseudo-labels <i>differently</i> in different classes for debaising. For example, when linear pseudo-label points to the majorities, more semantic pseudo-label component contributes to the final pseudo-label to prevent false positives towards head classes, and the vice versa when the linear pseudo-label predicts minority. 
          </p>
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
        <h2 class="title is-3">Experimental Results</h2> 
        <div class="content has-text-justified">
          <p>
            We use the imbalanced versions of CIFAR-10/100 and STL-10 under diverse cases of imbalances in unlabeled data ($ \gamma_u \neq \gamma_l$), including the same imbalance with labeled data ($ \gamma_u = \gamma_l$). 
          </p>
        </div>
        <!-- same imbalance -->
        <h3 class="title is-5">Same class imbalance ($ \gamma_l = \gamma_u $)</h3>
        <div class="content has-text-justified">
          <p class="mb-4">
            We compare DASO with several baseline methods, with or without applying class re-balancing strategies such as LA and ABC.
          </p>
          <img src="assets/daso/tab1.png"/>
        </div>
        <!-- different imbalance -->
        <h3 class="title is-5">Various class imbalance ($ \gamma_l \neq \gamma_u $)</h3>
        <div class="content has-text-justified">
          <p class="mb-4">
            The class distribution of unlabeled data could be either unknown or arguably different from that of labeled data in real-world. To simulate such scenarios, for CIFAR10-LT, uniform distributions ($ \gamma_u = 1$) and flipped long-tailed distribution with respect to labeled data ($ \gamma_u=1/100 $) are considered. For STL10-LT, we only control the degree of imbalance in labeled data ($ \gamma_l $) due to unknown distribution of unlabeled data.
          </p>
          <img src="assets/daso/tab2.png"/>
        </div>
        <!-- semi-aves -->
        <h3 class="title is-5">Realistic Scenarios</h3>
        <div class="content has-text-justified">
          <p class="mb-4">
            For real-world scenarios, long-tailed Semi-Aves benchmark including large unlabeled open-set data is considered. Both labeled data ($ \mathcal{X} $) and unlabeled data ($ \mathcal{U} $) show long-tailed distributions, while $ \mathcal{U} $ contains large open-set class examples ($ \mathcal{U}_{\text{out}} $). We report the results on both cases: $ \mathcal{U} = \mathcal{U}_{\text{in}} $ and $ \mathcal{U} = \mathcal{U}_{\text{in}} + \mathcal{U}_{\text{out}} $.
          </p>
          <div class="columns is-centered">
            <div class="column is-6">
              <img src="assets/daso/tab3.png"/>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
<!--/ Results -->

<!-- Analysis -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Qualitative Analysis</h2> 
        <div class="content has-text-justified">
          <p>
            We qualitatively analyze how DASO improves the performance under imbalanced SSL setup. We consider FixMatch as baseline trained on CIFAR10-LT under $ \gamma=100 $ and $ N_1 = 500 $.
          </p>
        </div>
        <!-- same imbalance -->
        <h3 class="title is-5">Unbiased pseudo-label improves test accuracy.</h3>
        <div class="content has-text-justified">
          <p>
            DASO significantly improves the recall and test accuracy values on the minority classes, while preserving those from the majority classes.
          </p>
        </div>
        <div class="hero-body">
          <div class="columns is-centered">
            <div class="column is-9">
              <img src="assets/daso/qual1.png"/>
            </div>
          </div>
          <h2 class="subtitle has-text-centered">
            Comparison of train curves for the recall and test accuracy values. 
          </h2>
        </div>
        <!-- different imbalance -->
        <h3 class="title is-5">Tail-class clusters are better identified.</h3>
        <div class="content has-text-justified">
          <p>
            Learning with DASO helps the model to establish tail-class clusters, which can further reduce the biases from the classifier.
          </p>
        </div>
        <div class="hero-body">
          <div class="columns is-centered">
            <div class="column is-9">
              <img src="assets/daso/qual2.png"/>
            </div>
          </div>
          <h2 class="subtitle has-text-centered">
            Comparisons of t-SNE from feature representations.
          </h2>
        </div>
      </div>
    </div>
  </div>
</section>
<!--/ Analysis -->

<section class="section">
  <div class="container is-max-desktop">
    <!-- Concurrent Work. -->
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Related Links</h2>
        <div class="content has-text-justified">
          <p>
            There's a lot of excellent work that was introduced around the same time as ours.
          </p>
          <p>
            <a href="https://arxiv.org/abs/2112.04564">CoSSL</a> introduces a co-learning framework that decouples the learning of representation and classifier in imbalanced SSL.
          </p>
          <p>
            <a href="https://people.eecs.berkeley.edu/~xdwang/projects/DebiasPL/">DebiasMatch</a> proposes a general debiased learning for pseudo-labels based on counterfactual reasoning and adaptive margins.
          </p>
          <p>
            <a href="https://arxiv.org/abs/2204.02070">Spread Spurious Attribute (SSA)</a> proposes a method of adaptive thresholds for pseudo-labeling that does not rely on the assumption: identical class distributions of labeled and unlabeled data (Secs. 4.2 and 5.4).  
          </p>
        </div>
      </div>
    </div>
    <!--/ Concurrent Work. -->
  </div>
</section>

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

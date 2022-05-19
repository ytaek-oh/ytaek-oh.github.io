---
layout: project_page
title: DASO
permalink: /daso
description: A new framework DASO, Distribution-Aware Semantics-Oriented Pseudo-label alleviates biases in pseudo-labels under diverse imbalanced semi-supervised learning scenarios.
keywords: "Semi-supervised learning, Class-imbalanced learning, Long-tailed distribution"
title: "DASO: Distribution-Aware Semantics-Oriented Pseudo-label for Imbalanced Semi-Supervised Learning"
pdf: https://ytaek-oh.github.io/assets/pdf/preprint_daso.pdf
arxiv: https://arxiv.org/abs/2106.05682
code: https://github.com/ytaek-oh/daso
bibtex: >
  @article{oh2021distribution, <br />
  title={Distribution-aware semantics-oriented pseudo-label for imbalanced semi-supervised learning}, <br />
  author={Oh, Youngtaek and Kim, Dong-Jin and Kweon, In So}, <br />
  journal={arXiv preprint arXiv:2106.05682}, <br />
  year={2021} <br />
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

<!-- project_page.html -->
<!--
<section class="hero teaser">
  <div class="container is-max-desktop">
    <div class="hero-body">
      <video id="teaser" autoplay muted loop playsinline height="100%">
        <source src="assets/videos/daso.mp4" type="video/mp4">
      </video>
      <h2 class="subtitle has-text-centered">
        <span class="dnerf">Nerfies</span> turns selfie videos from your phone into
        free-viewpoint
        portraits.
      </h2>
    </div>
  </div>
</section>
-->
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
    {%- if page.video %}
    <!-- Paper video. -->
    <div class="columns is-centered has-text-centered">
      <div class="column is-four-fifths">
        <h2 class="title is-3">Video</h2>
        <div class="publication-video">
          <iframe src="{{ page.video }}"
                  frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
        </div>
      </div>
    </div>
    <!--/ Paper video. -->
    {%- endif %}
  </div>
</section>


<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <!-- Visual Effects. -->
      <div class="column">
        <div class="content">
          <h2 class="title is-3">Visual Effects</h2>
          <p>
            Using <i>nerfies</i> you can create fun visual effects. This Dolly zoom effect
            would be impossible without nerfies since it would require going through a wall.
          </p>
        </div>
      </div>
      <!--/ Visual Effects. -->
      <!-- Matting. -->
      <div class="column">
        <h2 class="title is-3">Matting</h2>
        <div class="columns is-centered">
          <div class="column content">
            <p>
              As a byproduct of our method, we can also solve the matting problem by ignoring
              samples that fall outside of a bounding box during rendering.
            </p>
          </div>
        </div>
      </div>
    </div>
    <!--/ Matting. -->
    <!-- Animation. -->
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Animation</h2>
        <!-- Interpolating. -->
        <h3 class="title is-4">Interpolating states</h3>
        <div class="content has-text-justified">
          <p>
            We can also animate the scene by interpolating the deformation latent codes of two input
            frames. Use the slider here to linearly interpolate between the left frame and the right
            frame.
          </p>
        </div>
        <div class="columns is-vcentered interpolation-panel">
          <div class="column is-3 has-text-centered">
            <img src="https://homes.cs.washington.edu/~kpar/nerfies/images/interpolate_start.jpg"
                 class="interpolation-image"
                 alt="Interpolate start reference image."/>
            <p>Start Frame</p>
          </div>
          <div class="column interpolation-video-column">
            <div id="interpolation-image-wrapper">
              Loading...
            </div>
            <input class="slider is-fullwidth is-large is-info"
                   id="interpolation-slider"
                   step="1" min="0" max="100" value="0" type="range">
          </div>
          <div class="column is-3 has-text-centered">
            <img src="https://homes.cs.washington.edu/~kpar/nerfies/images/interpolate_end.jpg"
                 class="interpolation-image"
                 alt="Interpolation end reference image."/>
            <p class="is-bold">End Frame</p>
          </div>
        </div>
        <br/>
        <!--/ Interpolating. -->
        <!-- Re-rendering. -->
        <h3 class="title is-4">Re-rendering the input video</h3>
        <div class="content has-text-justified">
          <p>
            Using <span class="dnerf">Nerfies</span>, you can re-render a video from a novel
            viewpoint such as a stabilized camera by playing back the training deformations.
          </p>
        </div>
        <div class="content has-text-centered">
        </div>
        <!--/ Re-rendering. -->
      </div>
    </div>
    <!--/ Animation. -->
    <!-- Concurrent Work. -->
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Related Links</h2>
        <div class="content has-text-justified">
          <p>
            There's a lot of excellent work that was introduced around the same time as ours.
          </p>
          <p>
            <a href="https://arxiv.org/abs/2104.09125">Progressive Encoding for Neural Optimization</a> introduces an idea similar to our windowed position encoding for coarse-to-fine optimization.
          </p>
          <p>
            <a href="https://www.albertpumarola.com/research/D-NeRF/index.html">D-NeRF</a> and <a href="https://gvv.mpi-inf.mpg.de/projects/nonrigid_nerf/">NR-NeRF</a>
            both use deformation fields to model non-rigid scenes.
          </p>
          <p>
            Some works model videos with a NeRF by directly modulating the density, such as <a href="https://video-nerf.github.io/">Video-NeRF</a>, <a href="https://www.cs.cornell.edu/~zl548/NSFF/">NSFF</a>, and <a href="https://neural-3d-video.github.io/">DyNeRF</a>
          </p>
          <p>
            There are probably many more by the time you are reading this. Check out <a href="https://dellaert.github.io/NeRF/">Frank Dellart's survey on recent NeRF papers</a>, and <a href="https://github.com/yenchenlin/awesome-NeRF">Yen-Chen Lin's curated list of NeRF papers</a>.
          </p>
        </div>
      </div>
    </div>
    <!--/ Concurrent Work. -->
  </div>
</section>
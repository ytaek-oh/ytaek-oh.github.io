---
layout: basic_project_page
title: >
  SideGuide: A Large-scale Sidewalk Dataset for Guiding Impaired People
permalink: /sideguide
description: >
  SideGuide: A Large-scale Sidewalk Dataset for Guiding Impaired People
keywords: "Object detection, Instance segmentation, Depth estimation, Stereo matching, Assistive computer vision"
venue: "2020 International Conference on Intelligent Robots and Systems (IROS)"
pdf: http://ras.papercept.net/images/temp/IROS/files/1873.pdf
code: https://github.com/ChelseaGH/sidewalk_prototype_AI_Hub
bibtex: >
  @inproceedings{park2020sideguide,
    &nbsp;&nbsp;title={Sideguide: a large-scale sidewalk dataset for guiding impaired people},
    &nbsp;&nbsp;author={Park, Kibaek and Oh, Youngtaek and Ham, Soomin and Joo, Kyungdon and Kim, Hyokyoung and Kum, Hyoyoung and Kweon, In So}, 
    &nbsp;&nbsp;booktitle={2020 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)}, 
    &nbsp;&nbsp;pages={10022--10029}, 
    &nbsp;&nbsp;year={2020}, 
    &nbsp;&nbsp;organization={IEEE} 
  } 
abstract: >
  <p>In this paper, we introduce a new large-scale sidewalk dataset called SideGuide that could potentially help impaired people. Unlike most previous datasets, which are focused on road environments, we paid attention to sidewalks, where understanding the environment could provide the potential for improved walking of humans, especially impaired people. </p> 
  <p>Concretely, we interviewed impaired people and carefully selected target objects from the interviewees' feedback (objects they encounter on sidewalks). We then acquired two different types of data: crowd-sourced data and stereo data. We labeled target objects at instance-level (i.e., bounding box and polygon mask) and generated a ground-truth disparity map for the stereo data. SideGuide consists of 350K images with bounding box annotation, 100K images with a polygon mask, and 180K stereo pairs with the ground-truth disparity. </p>
  <p>We analyzed our dataset by performing baseline analysis for object detection, instance segmentation, and stereo matching tasks. In addition, we developed a prototype that recognizes the target objects and measures distances, which could potentially assist people with disabilities. The prototype suggests the possibility of practical application of our dataset in real life.</p>
---
<section class="hero">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns is-centered">
        <div class="column has-text-centered">
          <h1 class="title is-2 publication-title">{{ page.title }}</h1>
          <div class="is-size-4 publication-authors">
            <span class="author-block">
              <a href="#">Kibaek Park</a><sup>1$\small \ast$</sup>,</span>
            <span class="author-block">
              <a href="https://ytaek-oh.github.io">Youngtaek Oh</a><sup>1$\small \ast$</sup>,</span>
            <span class="author-block">
              <a href="#">Soomin Ham</a><sup>1$\small \ast$</sup>,</span>
            <span class="author-block">
              <a href="https://unist.info/?page_id=194">Kyungdon Joo</a><sup>2$\small \ast\dagger$</sup>,</span><br />
            <span class="author-block">
              <a href="#">Hyokyoung Kim</a><sup>3$\small ¶$</sup>,</span>
            <span class="author-block">
              <a href="#">Hyoyoung Kum</a><sup>3$\small ¶$</sup>,</span>
            <span class="author-block">
              <a href="#">In So Kweon</a><sup>1</sup>,
            </span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>1</sup>KAIST,&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block"><sup>2</sup>UNIST,&nbsp;&nbsp;&nbsp;</span>
            <span class="author-block"><sup>3</sup>Independent</span>
          </div>
          <div class="is-size-5 publication-authors">
            <span class="author-block"><sup>$\ast$</sup><em>Equal contributions,</em>&nbsp;</span>
            <span class="author-block"><sup>$\small \dagger$</sup><em>Work done at KAIST</em>, &nbsp;</span>
            <span class="author-block"><sup>$\small ¶$</sup><em>Work done at TestWorks, Inc.</em></span>
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
        <source src="assets/sideguide/media3_compressed.mp4" type="video/mp4">
      </video>
      <h2 class="subtitle has-text-centered is-size-5">
        An assistance system for impaired people by informing obstacles with distances. <br />The video is taken on a wheelchair, where many safety-related obstacles are scattered on the way. <br />Each bounding box is marked with class label and distance.
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
To date, autonomous driving has been one of the most researched topics. Previous studies have largely been focused on self-driving cars and their driving environment, which has led to ample datasets related to roads (e.g., KITTI [1], Cityscapes [2]). In contrast, there has not been enough data investigating the perspectives of pedestrians and their environments, such as sidewalks. Traditionally for cars, fixed lanes separate cars from other vehicles, which makes it easier to detect moving objects. On the other hand, when it comes to a sidewalk, there are no fixed lanes, and there are lots of objects (e.g., pedestrians, personal mobility vehicles, animals, and bollards) that lack directional consistency. Therefore, in the sidewalk environment, objects often occlude each other (i.e., partially blocked by other objects).
          </p>
          <p>
Our work is the first large-scale dataset (termed the SideGuide) focused on sidewalks, and which can be deployed in the field of recognition to aid impaired or disabled people. We also used a stereo camera system to capture images of sidewalks, which provides ground-truth disparity as well as instance-level annotation (see Fig. 1).
          </p>
          <p>
From the raw data, we annotated 492K images in total for ground-truth (see Table I). Specifically, as instance-level annotation, we generated ground-truth bounding boxes (BB) for 350K images and polygon segmentations for 100K images as a subset of BB. We also generated 180K dense disparity maps from pairs of stereo images. The instance-level annotations and ground-truth disparity provided inference data to the detection model and stereo matching algorithm, respectively, to validate our dataset. The SideGuide was further validated by implementing a prototype that returns the output of object detection and distance of an object from the camera in real-time.
          </p>
        </div>
        <div class="hero-body">
          <div class="columns is-centered">
            <div class="column is-5">
              <img src="assets/sideguide/teaser.png"/>
            </div>
          </div>
          <h2 class="my-1 subtitle has-text-centered">
            <p>
            An example image-pair and annotation of a sidewalk. (a) Stereo image pair captured by a ZED stereo camera (top and bottom images indicate left and right images, respectively), (b) Instance-level bounding box and polygon mask annotations in the left image, and (c) The ground-truth dense disparity map.
            </p>
          </h2>
        </div>
        <div class="content has-text-justified">
          <p>
Our first large-scale sidewalk dataset, the SideGuide will contribute to reducing the gap between technology and real-world deployment for recognition. This dataset could be useful not only for impaired people, but also for other applications like mobile robotics and assistance for vulnerable road users who are not necessarily visually or mobility impaired.
          </p>
        </div>
      </div>
    </div>
  </div>
</section>
<!--/ introduction -->

<!-- Download -->
<section class="section">
  <div class="container is-max-desktop">
    <div class="columns is-centered">
      <div class="column is-full-width">
        <h2 class="title is-3">Download Request</h2> 
        <div class="content has-text-justified">
          <p>
            In order to access our SideGuide dataset, you must first agree to the terms and conditions by completing a brief survey provided <a href="https://docs.google.com/forms/d/e/1FAIpQLScBmoVoj0d-omBOVCHGjhRislXP0TYzRqaUJOmJcqN6ylQcxQ/viewform" target="_blank">here</a>. You will receive the download link shortly after the approval process is completed. 
          </p>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- END -->


<!-- motivation -->
<!--
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
-->
<!--/ motivation -->

<!-- Results -->
<!--
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
        <h3 class="title is-5">Same class imbalance ($ \gamma_l = \gamma_u $)</h3>
        <div class="content has-text-justified">
          <p class="mb-4">
            We compare DASO with several baseline methods, with or without applying class re-balancing strategies such as LA and ABC.
          </p>
          <img src="assets/daso/tab1.png"/>
        </div>
        <h3 class="title is-5">Various class imbalance ($ \gamma_l \neq \gamma_u $)</h3>
        <div class="content has-text-justified">
          <p class="mb-4">
            The class distribution of unlabeled data could be either unknown or arguably different from that of labeled data in real-world. To simulate such scenarios, for CIFAR10-LT, uniform distributions ($ \gamma_u = 1$) and flipped long-tailed distribution with respect to labeled data ($ \gamma_u=1/100 $) are considered. For STL10-LT, we only control the degree of imbalance in labeled data ($ \gamma_l $) due to unknown distribution of unlabeled data.
          </p>
          <img src="assets/daso/tab2.png"/>
        </div>
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
-->
<!--/ Results -->

<!-- Analysis -->
<!--
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
-->
<!--/ Analysis -->

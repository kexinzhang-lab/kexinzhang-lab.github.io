---
layout: about
title: about
permalink: /

selected_papers: false
social: true

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

<div class="home-research-intro">
  <div class="home-research-copy">
    <p>We develop computational imaging and AI methods that push <strong>cryo-EM and cryo-ET beyond current detection limits</strong>, enabling molecular machines and their changing states to be visualized directly in cells.</p>
  </div>
  <figure class="home-research-visual">
    <a href="{{ '/assets/img/research-overview.png' | relative_url }}" aria-label="View the research overview at full size">
      <img src="{{ '/assets/img/research-overview.png' | relative_url }}" alt="Cryo-EM/ET imaging, structural cell biology, and AI come together to detect molecular targets, decode structures and states, and discover hidden patterns of cellular organization." width="1448" height="1086" fetchpriority="high">
    </a>
  </figure>
</div>

<figure class="home-movie">
  <div class="home-movie-labels" aria-hidden="true">
    <span>Template<small>60S ribosomal subunit (PDB 5LZV)</small></span>
    <span>Micrograph<small>BSC-1 cell lysate · EMPIAR-13577</small></span>
  </div>
  <div class="home-movie-stage">
    <video id="home-movie-video" autoplay loop muted playsinline preload="auto" width="1800" height="886" poster="{{ '/assets/img/research/2dtm-lysate-poster.webp' | relative_url }}" aria-label="2D template matching: a 3D template of the 60S ribosomal subunit is searched across a cryo-EM micrograph of cell lysate, and detected ribosomes appear in red.">
      <source src="{{ '/assets/video/research/2dtm-lysate-light.mp4' | relative_url }}" type="video/mp4">
    </video>
    <span class="home-movie-status" aria-hidden="true">searching orientations…</span>
  </div>
  <figcaption><strong>Finding molecules in a single image.</strong> Our fast 2D template matching (2DTM) searches a 3D map across orientations and positions in a cryo-EM micrograph of cell lysate. Accuracy mode: 16 true and 3 false positives. Data: Seraj Z, et al. <em>eLife</em> 2026.</figcaption>
</figure>
<script>
  // The movie is rendered onto each theme's background color; swap files when the theme changes.
  (() => {
    const video = document.getElementById("home-movie-video");
    const sources = {
      light: "{{ '/assets/video/research/2dtm-lysate-light.mp4' | relative_url }}",
      dark: "{{ '/assets/video/research/2dtm-lysate-dark.mp4' | relative_url }}",
    };
    const sync = () => {
      const src = sources[document.documentElement.getAttribute("data-theme") === "dark" ? "dark" : "light"];
      if (video.currentSrc.endsWith(src)) return;
      const time = video.currentTime;
      video.src = src;
      video.currentTime = time;
      video.play().catch(() => {});
    };
    sync();
    new MutationObserver(sync).observe(document.documentElement, { attributes: true, attributeFilter: ["data-theme"] });
  })();
</script>

- **Seeing the unseen** — Small, flexible, and rare molecules hide in noisy images. We build AI-accelerated algorithms that find individual proteins and recover their 3D structures.
- **Biology inside cells** — Molecular machines behave differently in their native environment. We map where they are, which states they adopt, and how cellular structures are organized around them.
- **Catching drugs in the act** — We reveal how drugs bind challenging targets, exposing binding pockets and interactions that can guide drug design.
- **Teaching AI to see molecules** — We develop generative models, simulations, and foundation models that learn from both molecular structures and microscopy images.

[Explore our research →]({{ '/research/' | relative_url }})

## Join us — multiple openings!

The lab is actively recruiting. We welcome applications at every career stage:

- **Postdocs** — strong background in cryo-EM/ET, AI, computational structural biology, or scientific computing. Please email Kexin your CV, a short research statement, and contact info for three references.
- **PhD students** — students interested in doing a PhD in our lab should apply through Yale's [Biological and Biomedical Sciences (BBS) program](https://medicine.yale.edu/bbs/), via either the [Biochemistry, Quantitative Biology, Biophysics and Structural Biology (BQBS)](https://medicine.yale.edu/bbs/tracks/biochemistry-quantitative-biophysics-structural-biology) or the [Computational Biology and Biomedical Informatics (CBB)](https://medicine.yale.edu/bbs/tracks/computational-biology-bioinformatics) track. If you are already a Yale graduate student and would like to do a rotation with us, please email Kexin directly. We are accepting rotation students!
- **Master's students** — Yale master's students interested in cryo-EM/ET methods, computational imaging, AI, or scientific software are encouraged to reach out.
- **Undergraduates** — Yale undergraduates looking for research experience are welcome to inquire about projects. Email Kexin directly with your CV and a brief note about your interests.
- **Postgraduates** — we welcome motivated applicants with a BS or MS and a strong interest in cryo-EM/ET, AI, or computational structural biology who are eager to gain hands-on research experience. Please email Kexin your CV and a brief note about your research interests and goals.

---
layout: page
title: CV
permalink: /cv/
---
{%- assign cv_pdf = site.static_files | where: "path", "/assets/cv.pdf" | first -%}
{%- if cv_pdf %}
<p class="lede"><a href="{{ '/assets/cv.pdf' | relative_url }}">Download PDF</a></p>
{%- endif %}

<h2>Experience</h2>
<dl class="cv">
  <dt>2026&ndash;present</dt>
  <dd>
    <strong>AI Engineer</strong>, Mohamed bin Zayed University of Artificial Intelligence (MBZUAI)
    <ul>
      <li>Building biocomputers as part of the Organoid Intelligence project.</li>
      <li>Built and validated an end-to-end Codabench-based model evaluation platform for a J&amp;J hackathon: data ingestion, GPU inference across NVIDIA A10 and A4000 GPUs, automated scoring, and participant guidelines.</li>
      <!-- TODO: Project B1 (Organoid Intelligence) and Project A (Collective Learning) descriptions -->
    </ul>
  </dd>

  <dt>2024&ndash;present</dt>
  <dd>
    <strong>Research Associate</strong>, Khalifa University
    <ul>
      <li>Developed interpretable-by-design neural vision models (DINOv2, CLIP) grounded in mechanistic interpretability.</li>
      <li>Contributed to grant writing for external funding.</li>
      <li>Designed and supervised nationwide AI workshops for high-school students at the KU AI Winter Camp 2024.</li>
    </ul>
  </dd>

  <dt>2022&ndash;2023</dt>
  <dd>
    <strong>Graduate Research and Teaching Assistant</strong>, Khalifa University
    <ul>
      <li>Designed GAN-based image reconstruction methods from partial sensory data, and physics-based sensor models for IoT radiation monitoring.</li>
      <li>Taught labs and tutorials in Data Structures and Algorithms, Introduction to Computing, and Object-Oriented Programming.</li>
    </ul>
  </dd>

  <dt>2021</dt>
  <dd>
    <strong>Software Engineer Intern</strong>, GamaLearn
    <ul>
      <li>Led the transition to a revamped proprietary OCR system and integrated it into production.</li>
    </ul>
  </dd>
</dl>

<h2>Education</h2>
<dl class="cv">
  <dt>2022&ndash;2023</dt>
  <dd>
    <strong>MSc, Electrical and Computer Engineering</strong> (Artificial Intelligence), Khalifa University<br>
    <span class="muted">Thesis: AI-Driven Target Localization Enabled by UAVs and IoT</span>
  </dd>
  <dt>2017&ndash;2021</dt>
  <dd>
    <strong>BSc, Computer Engineering</strong> (Artificial Intelligence), Abu Dhabi University<br>
    <span class="muted">Dean&rsquo;s List 2018&ndash;2021. Thesis: VR-Controlled System for Remote Wiring of Electronic Circuits on a Trainer</span>
  </dd>
</dl>

<h2>Publications</h2>
<p>See <a href="{{ '/publications/' | relative_url }}">Publications</a>.</p>

<h2>Honors and awards</h2>
<dl class="cv">
  <dt>2024</dt><dd>Teaching Certificate Course for Post Docs, Center for Teaching and Learning, Khalifa University</dd>
  <dt>2023</dt><dd>Elite Young Researcher Award, for publishing master&rsquo;s work in a top 3% signal processing journal</dd>
  <dt>2022</dt><dd>2nd place, Emirates Global Aluminium (EGA) Industrial Robotics Competition</dd>
  <dt>2022</dt><dd>Research and Teaching Scholarship, Khalifa University</dd>
  <dt>2022</dt><dd>UAE 10-Year Golden Residency, outstanding university students category</dd>
  <dt>2020</dt><dd>1st place in Abu Dhabi, NASA Space Apps Challenge</dd>
  <dt>2018</dt><dd>Academic Excellence Scholarship, Abu Dhabi University</dd>
</dl>

<h2>Service</h2>
<dl class="cv">
  <dt>Reviewing</dt><dd>IEEE Transactions on Services Computing; IEEE Internet of Things Magazine; Elsevier Ad Hoc Networks</dd>
  <dt>Organizing</dt><dd>Volunteer organizer, IEEE ICIP 2024, IEEE CloudCom 2024, IEEE MECOM 2024</dd>
</dl>

<h2>Skills</h2>
<dl class="cv">
  <dt>Machine learning</dt><dd>PyTorch, TensorFlow, Keras, OpenCV, SciPy, NumPy, Pandas, scikit-learn</dd>
  <dt>Programming</dt><dd>Python, C/C++, Java, MATLAB, Bash, LaTeX</dd>
  <dt>Hardware</dt><dd>NVIDIA Jetson, Raspberry Pi, ESP32, Arduino</dd>
  <dt>Languages</dt><dd>Arabic (native), English (fluent, IELTS 8)</dd>
</dl>

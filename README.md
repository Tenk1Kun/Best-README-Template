<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="#">
    <img src="images/logo.png" alt="Logo" width="100" height="100">
  </a>

  <h3 align="center">Architecture → Music Generator</h3>

  <p align="center">
    Turn buildings into music — fully in-browser, AI-enhanced, real-time sonification.
    <br />
    <a href="https://hackathon-2025-edge-music.vercel.app/"><strong>View Demo »</strong></a>
    <br />
    <br />
    <a href="https://hackathon-2025-edge-music.vercel.app/">Live App</a>
    ·
    <a href="https://github.com/Tenk1Kun/Music-AI-Hackathon-Osaka-2025-Music-Project/issues/new?labels=bug&template=bug-report.md">Report Bug</a>
    ·
    <a href="https://github.com/Tenk1Kun/Music-AI-Hackathon-Osaka-2025-Music-Project/issues/new?labels=enhancement&template=feature-request.md">Request Feature</a>
  </p>
</div>

---

<!-- TABLE OF CONTENTS -->
<details>
  <summary>📑 Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#how-it-works">How It Works</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

---

## About The Project

[![Product Screenshot][product-screenshot]](https://hackathon-2025-edge-music.vercel.app/)

Convert architecture into music — **directly in your browser**, no backend, no data sent anywhere.

**AI Style Classifier:** Japan vs Austria  
**Vision Processing:** Canny + Sobel  
**Music Engine:** Tone.js, scale-snapped melodies  
**Real-time:** Zero server, instant inference  
**Privacy:** Image never leaves device  

> “Buildings are frozen music — this app lets them play.”

### How It Works

| Step | Action |
|------|-------|
1 | Upload building image  
2 | TF-JS model classifies architectural style  
3 | OpenCV extracts edges + gradient magnitude  
4 | Horizontal band slicing → melodic lines  
5 | y → pitch · x → timing · mag → velocity  
6 | Tone.js renders real-time sound  

### Music Mapping Rules

| Visual Feature | Musical Meaning |
|---|---|
Vertical position (y) | Pitch (height → higher notes)  
Horizontal (x) | Time (left to right → rhythm)  
Gradient magnitude | Velocity (louder if edges strong)  
Architecture style | Scale, tempo, instrument  

Style behaviors:
- **Japan → Kumoi scale, ~100 BPM, Koto**
- **Austria → Harmonic minor, ~90 BPM, Piano**

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 🛠 Built With

* [![Next][Next.js]][Next-url]
* [![React][React.js]][React-url]
* TensorFlow.js
* OpenCV.js (WASM)
* Tone.js (WebAudio)
* TypeScript

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

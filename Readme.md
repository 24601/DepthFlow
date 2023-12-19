👆【☰】Table of Contents

<div align="justify">

<div align="center">
  <img src="./DepthFlow/Resources/DepthFlow.png" width="200">

  <h1>DepthFlow</h1>

  <img src="https://img.shields.io/github/stars/BrokenSource/DepthFlow" alt="Stars Badge"/>
  <img src="https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2FBrokenSource%2FDepthFlow.json%3Fshow%3Dunique&label=Visitors&color=blue"/>
  <img src="https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2FBrokenSource%2FDepthFlow.json&label=Page%20Views&color=blue"/>
  <img src="https://img.shields.io/github/license/BrokenSource/DepthFlow?color=blue" alt="License Badge"/>
  <a href="https://t.me/brokensource">
    <img src="https://img.shields.io/badge/Telegram-Channel-blue?logo=telegram" alt="Telegram Channel Badge"/>
  </a>
  <a href="https://discord.gg/KjqvcYwRHm">
    <img src="https://img.shields.io/discord/1184696441298485370?label=Discord&color=blue" alt="Discord Badge"/>
  </a>

  <sub> 👆 Out of the many **Explorers**, you can be among the **Shining** stars who support us! ⭐️ </sub>

  <br>

  <ins> **[**[**DepthFlow**](https://github.com/BrokenSource/DepthFlow)**]**: Image → **2.5D Parallax** Effect Video. A Professional **[**[**Depthy**](https://depthy.stamina.pl)**]** Alternative. </ins>
</div>

<br>

👇 Right click and **loop me**!

https://github.com/BrokenSource/DepthFlow/assets/29046864/cf9e23f0-e64b-435a-8762-e49936602071

<sup><b>Note:</b> Yes, the only input to DepthFlow was the Original Image</sup>

<br>

<details>
<summary>🎩 <b>Click</b> to see the Original Image </summary>
  <br>
  <a href="https://wallhaven.cc/w/pkz5r9">
    <img src="https://github.com/BrokenSource/DepthFlow/assets/29046864/1975fdc9-9517-4700-88dd-ed8175ab813f" alt="Original Image">
  </a>
  <br>
  <br>
</details>

<details>
<summary>🪄 <b>Click</b> to see the Estimated Depth map </summary>
  <br>
  <img src="https://github.com/BrokenSource/DepthFlow/assets/29046864/7f73775e-0b08-4a4f-bf97-7cb8f3aecad8" alt="Depth Map">
  <br>
  <br>
</details>

<br>

# 🔥 Description

**💡 Base idea:**
1. Given an image and its depth map, have a shader to generate a parallax effect
2. Estimate Depth Maps with Neural Networks for generic images
3. Varying the projections over time generates a 2.5D video

As simple as that, we achieve a similar effect as [**Depthy**](https://depthy.stamina.pl)

<br>
<br>

# 📦 Installation

> 🔴🟡🟢
>
> **Download** and install our [**Monorepo**](https://github.com/BrokenSource/BrokenSource) with all the code and projects first
>
> <sub><b>Note:</b> You cannot run this project in dev mode without the <i>Framework!</i></sub>

## Running the code

- Run the command: `broken depthflow` on the Broken Environment

A real time window should pop up. You can see `broken depthflow --help` for render options

#### Selecting the image
- `broken depthflow settings (url | path) main`

#### Rendering to a video
- `broken depthflow (--render | -r)`
- `broken depthflow -r -w 1280 -h 720 -f 30`
- `broken depthflow -r -o ./video_name -f mkv`
- `broken depthflow settings (url | path) main --render -s 2`

<b>Note</b>: A high SSAA `-s 2` is recommended for antialiasing

<sup><b>Todo:</b> Reimplement the Gradio interface; configurable parallax settings</sup>

<br>
<br>

# 🚀 Using your GPU

> By default, Pytorch will be installed with CPU support.

If you want to **Speed Up** the **Depth Estimation** process, you can install it with GPU support:

<br>

**NVIDIA**<sup>N1</sup> (CUDA):
- Install [CUDA](https://developer.nvidia.com/cuda-downloads) and [cuDNN](https://developer.nvidia.com/cudnn)
- Run the command: `broken depthflow poe cuda`

<sub>*N1: Your GPU must support PyTorch's CUDA version, all >= GTX 900. Preferably install from your package manager</sub>


<br>

**AMD**<sup>R1</sup> (ROCm):
- Run the command: `broken depthflow poe rocm`

<sub>*R1: Check GPU compatibility, <= RX 500 series is not supported. Preferably install from your package manager</sub>


<br>

**CPU / macOS** (Default):

- Run the command: `broken depthflow poe cpu`


<br>
<br>

# ⚖️ License

**See [BrokenSource](https://github.com/BrokenSource/BrokenSource) Repository** for the License of the Code Assets, Projects and User Generated Content.

</div>
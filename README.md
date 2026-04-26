# 🧠 MoE Vision Pro Ultra

&gt; **The World's Most Advanced Browser-Based Mixture of Experts (MoE) Visualization Engine**

[![Version](https://img.shields.io/badge/version-3.0--Ultra-blueviolet)](https://github.com/gotrendwise-com/MoE-Interactive-Simulator-)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Made with](https://img.shields.io/badge/made%20with-Three.js%20%7C%20Chart.js%20%7C%20Vanilla%20JS-orange)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

&lt;p align="center"&gt;
  &lt;img src="https://img.shields.io/badge/MoE-Interactive%20Simulator-6366f1?style=for-the-badge&logo=tensorflow" alt="MoE Vision Pro"&gt;
&lt;/p&gt;

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Live Demo](#-live-demo)
- [Installation](#-installation)
- [Usage Guide](#-usage-guide)
- [Architecture Explained](#-architecture-explained)
- [Supported MoE Architectures](#-supported-moe-architectures)
- [Keyboard Shortcuts](#-keyboard-shortcuts)
- [Technology Stack](#-technology-stack)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## 🌟 Overview

**MoE Vision Pro Ultra** is an interactive, browser-based educational platform designed to demystify **Mixture of Experts (MoE)** — the sparse neural network architecture powering modern Large Language Models like **GPT-4**, **Mixtral 8x7B**, **Google Gemini**, and **Switch Transformers**.

Instead of reading dense research papers, you can **see, interact with, and experiment** with MoE concepts in real-time using:
- 🎮 **Interactive parameter controls**
- 🧊 **Real-time 3D visualizations** (Three.js)
- 📊 **Live training metrics dashboards**
- 💻 **Auto-generated production code** (PyTorch / TensorFlow / JAX)
- 🌍 **Full Urdu (RTL) + English bilingual support**

&gt; **No installation. No GPU. No backend.** Just open the HTML file in any modern browser.

---

## ✨ Key Features

### 🧊 3D Neural Network Visualization
- Real-time **Three.js** rendering of expert nodes
- Dynamic routing connections with animated particle flow
- Active experts glow; inactive ones fade
- Auto-rotating camera with smooth transitions

### 📡 Live Training Monitor
Real-time calculation of critical MoE training metrics:
- **Load Balancing Loss** — prevents expert collapse
- **Router Z-Loss** — stabilizes router logits
- **Expert Utilization** — active capacity percentage
- **FLOPs Counter** — billions of operations per forward pass

### 🎛️ Advanced Control Panel
| Parameter | Range | Description |
|-----------|-------|-------------|
| **N (Total Experts)** | 2 – 16 | Number of expert networks |
| **Top-K** | 1 – 8 | How many experts activate per token |
| **Input Value (x)** | 0.0 – 20.0 | Simulated input token embedding |
| **Temperature (T)** | 0.1 – 5.0 | Softmax temperature for gating |
| **Capacity Factor** | 0.5 – 3.0 | Token capacity per expert |
| **Load Balance Weight** | 0.0 – 0.1 | Auxiliary loss coefficient |
| **Animation Speed** | 0.5x – 3.0x | Visualization playback speed |

### 🏗️ Architecture Explorer
Compare 4 major MoE architectures side-by-side:
1. **Switch Transformer** (Google — Top-1 routing)
2. **BASE Layers** (Balanced joint training)
3. **Hash Layers** (Router-free O(1) routing)
4. **Expert Choice** (Token → Expert reverse routing)

Each includes:
- Detailed explanation
- Architecture-specific stats
- Syntax-highlighted **PyTorch** code with copy button

### 💻 Code Generator
Generate production-ready MoE layer code for:
- **PyTorch** (`nn.Module`)
- **TensorFlow/Keras** (`keras.layers.Layer`)
- **JAX/Flax** (`nn.Module`)

Code dynamically injects your current N, K, and configuration values.

### 📊 Interactive Charts
- **Gate Score Distribution** (Doughnut chart)
- **Expert Utilization Heatmap** (Bar chart with active/inactive coloring)

### 🌍 Bilingual & Accessible
- Complete **Urdu (Nastaliq)** interface with RTL layout
- **English** technical terms preserved for clarity
- Designed for South Asian AI learners and educators

### 🎯 Additional Tools
- 🌓 **Dark / Light theme toggle**
- 📥 **Export results to JSON**
- 🖥️ **Fullscreen mode**
- ⌨️ **Keyboard shortcuts**
- 🔊 **Voice narration** (Web Speech API)
- 📱 **PWA-ready** (works offline)

---

## 🚀 Live Demo

🔗 **Try it now:** [https://gotrendwise-com.github.io/MoE-Interactive-Simulator-](https://gotrendwise-com.github.io/MoE-Interactive-Simulator-)

Or simply download `moe_vision_pro_ultra.html` and open it in your browser.

---

## 📥 Installation

Since this is a **fully self-contained static web application**, there is no build step or server required.

### Option 1: Direct Download
```bash
# Clone the repository
git clone https://github.com/gotrendwise-com/MoE-Interactive-Simulator-.git

# Open the file
cd MoE-Interactive-Simulator-
open moe_vision_pro_ultra.html        # macOS
xdg-open moe_vision_pro_ultra.html    # Linux
start moe_vision_pro_ultra.html       # Windows

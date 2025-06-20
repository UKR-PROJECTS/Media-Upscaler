# 🚀 Anime‑Media‑Upscaler v2.0.0

![License: MIT](https://img.shields.io/badge/License-MIT-green) ![Language: Python](https://img.shields.io/badge/Language-Python-blue) ![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen)

<p align="center">
  <img src="src/favicon.ico" alt="App Icon" width="64" height="64" />
</p>

Anime‑Media‑Upscaler is a powerful, open‑source desktop application built with PyQt6, leveraging Real‑ESRGAN AI models and FFmpeg to batch upscale your favorite anime images and videos with ease 

---

## ✨ What’s New in v2.0.0

- ✅ **Video Upscaling** support via frame‑by‑frame Real‑ESRGAN + FFmpeg reassembly  
- ✅ **Multi‑threaded** batch processing with real‑time progress bars  
- ✅ **Advanced Settings** dialog: model selection, GPU toggle, tile size, FPS & quality  
- ✅ **Comprehensive Logging** system with save/load capability  
- ✅ **Drag‑and‑Drop** interface enhancements  

---

## 🛠️ All Features

- **Image Upscaling**: JPG/PNG/BMP/TIFF/WebP → 2×/3×/4× scales  
- **Video Upscaling**: MP4/AVI/MKV/MOV/WMV/FLV → upscaled frames + original audio  
- **Batch Queue**: enqueue multiple files for sequential processing  
- **Model Manager**: choose from anime‑optimized & general SR Real‑ESRGAN variants  
- **GPU Acceleration**: CUDA/OpenCL support for faster upscaling  
- **Advanced Settings**: tile size, output format (jpg/png/webp), FPS, CRF quality  
- **Auto‑Folder**: outputs organized into timestamped sessions  
- **Drag‑and‑Drop**: intuitive file/folder addition  
- **Logging**: timestamped logs, clear & save to file  

---

## 🗂️ Folder Structure

```

Anime-Media-Upscaler/
├── LICENSE                  # MIT License
├── README.md                # This file
├── requirements.txt         # Python dependencies
├── src/                         # Source directory
│    ├── build.bat                # Convert main.py into exe
│    ├── main.py                  # Application entry point
│    ├── favicon.ico              # App icon
│    ├── bin/                     # External executables
│    │   ├── ffmpeg.exe           # FFmpeg binary
│    │   └── realesrgan-ncnn-vulkan.exe  # Real‑ESRGAN engine
│    └── models/                  # Pre‑downloaded .param & .bin files
│        └── \*.param  \*.bin
├── example/                 # Sample inputs & outputs
│   ├── pikachu.jpg
│   └── pikachu_upscaled_x4.jpg
└── screenshots/             # UI previews
    └── screenshot.png

````

---

## 📋 Requirements

- **Python 3.8+**  
- **pip** package manager  
- **CUDA‑enabled GPU** (optional, for acceleration)  
- **Real‑ESRGAN** & **FFmpeg** binaries in `bin/` or system PATH  

Install dependencies:

```bash
pip install -r requirements.txt
````

> Or manually:
>
> ```bash
> pip install PyQt6 colorlog
> ```

---

## ⚙️ Installation

1. **Clone** the repository

   ```bash
   git clone https://github.com/UKR-PROJECTS/Anime-Media-Upscaler.git
   cd Anime-Media-Upscaler
   ```
2. **Ensure** `bin/ffmpeg` and `bin/realesrgan-ncnn-vulkan` are present or in PATH
3. **Install** Python dependencies

   ```bash
   pip install -r requirements.txt
   ```

---

## ▶️ Usage

1. **Run** the app:

   ```bash
   python main.py
   ```
2. **Add Files**: drag‑and‑drop or click **Add Files** / **Add Folder**
3. **Select Output Folder** and configure quick or advanced settings
4. **Start Upscaling** and monitor **Overall** & **Current** progress bars
5. **Save Logs** or **Open Output** once complete

---

## 🖼️ Example Inputs & Outputs

<p align="center">
  <img src="example/pikachu.jpg" alt="Original Pikachu" width="300" />
  <img src="example/pikachu_upscaled_x4.jpg" alt="Upscaled Pikachu ×4" width="300" />
</p>

## 📸 Screenshot

![Interface](screenshots/screenshot.png)

---

## 🤝 How to Contribute

1. **Fork** the repo
2. **Create** a branch:

   ```bash
   git checkout -b feature/YourFeature
   ```
3. **Commit** your improvements
4. **Push** & **Open** a Pull Request

---

## 🙏 Acknowledgments

* [Real‑ESRGAN](https://github.com/xinntao/Real-ESRGAN) for super‑resolution models
* [PyQt6](https://pypi.org/project/PyQt6/) for the GUI framework
* [FFmpeg](https://ffmpeg.org/) for high‑quality video processing

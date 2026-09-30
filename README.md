# Hi, I'm Isilsolme 👋

I build small, focused tools — firmware for microcontrollers, computer-vision experiments,
and plugins for the open-source clients I use every day.

- 🔧 **Embedded** — ESP32-S3, PlatformIO, Arduino / ESP-IDF, serial protocol parsing, FreeRTOS
- 👁 **Machine vision & ML** — OpenCV pipelines, PyTorch semantic segmentation
- 🧩 **DSH ecosystem** — plugins for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness), published on npm
- 🎧 **Open-source clients** — third-party music sources, Electron internals, `asar` tooling

---

## 🧩 DSH Plugins

| Plugin | What it does |
| --- | --- |
| [**dsh-anthropic-fonts**](https://github.com/Isilsolme/dsh-anthropic-fonts) | Switches the DSH Web UI to Anthropic Sans / Serif / Mono, with Source Han fallback for CJK · [![npm](https://img.shields.io/npm/v/dsh-anthropic-fonts?label=npm)](https://www.npmjs.com/package/dsh-anthropic-fonts) |
| [**dsh-splash-launcher**](https://github.com/Isilsolme/dsh-splash-launcher) | One-click DSH launcher for Windows: plays a splash animation immediately, boots `dsh web`, reveals the GUI when ready · [![npm](https://img.shields.io/npm/v/dsh-splash-launcher?label=npm)](https://www.npmjs.com/package/dsh-splash-launcher) |

`dsh-anthropic-fonts` is listed in [awesome-dsh-plugin](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin).

```sh
dsh plugin --profile web add dsh-anthropic-fonts
dsh plugin --profile web add dsh-splash-launcher
```

I care about the boring parts of plugin engineering: per-release compatibility matrices
that only claim `compatible` after an actual smoke test in a throwaway `DSH_HOME`,
uninstall that leaves nothing behind, and a minimal permission surface.

## 👁 Computer Vision & ML

- Classical OpenCV work — grayscale transforms and CLAHE, linear / non-linear filtering,
  Canny and Otsu binarization, contours and morphology
- Feature detection and matching — SIFT + FLANN + RANSAC homography, HOG + SVM
  pedestrian detection, Hough lines and circles
- PyTorch semantic segmentation with UNet / MiniUNet, trained on Oxford-IIIT Pet
  with a Dice + BCE objective

## 🔧 Embedded

- ESP32-S3 firmware built with PlatformIO
- Serial protocol work: frame parsing, framing and validation, device handshakes,
  and controlling read cycles from the firmware side
- FreeRTOS task structuring for hardware that has to keep responding while it works

## 🎧 Open-Source Clients

- Third-party music source plugins for open-source desktop players
- Electron app internals: `asar` containers, patched network layers, CDP-driven
  end-to-end debugging

---

📫 Reach me at **duanhaohong@163.com**

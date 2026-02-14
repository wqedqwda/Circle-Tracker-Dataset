# Circle-Tracker: Dataset Samples

This repository contains **representative sample sequences** from the dataset used in the paper:
**"Circle-Tracker: Geometry-Constrained Stereo Multi-Object Tracking Under Severe Occlusion and Nonlinear Motion"** (Submitted to IEEE Transactions on Instrumentation and Measurement).

## ⚠️ Important Note
This is a **subset** of the full dataset. The provided sequences primarily demonstrate **high-speed motion** and **nonlinear rotation** with clear visibility.

**To reproduce the "Severe Occlusion" experiments described in the paper, we recommend applying synthetic occlusion (e.g., random masking) on these clean frames.** This ensures precise ground truth availability for quantitative evaluation.

## 📂 Content Overview
The samples include **raw uncompressed images** and corresponding annotations, organized in a flat structure:

* **Format**: Images (`.bmp`) and Annotations (`.json`) are stored together.
* **Image Type**: **Raw BMP (Lossless)** to preserve edge details for sub-pixel localization.
* **Annotation Type**: **Labelme JSON** (with `rotation` shape type for Oriented Bounding Boxes).

### Scenarios Covered
* **High-Speed Motion**: Structural vibration simulation.
* **Large-Angle Rotation**: Perspective deformation of circular markers.
* **Clean Baseline**: Ideal for simulating synthetic occlusion constraints.

## 🛠️ File Structure
```text
/
├── dataset/
│   ├── seq_01_0001.bmp      # Raw Lossless Image
│   ├── seq_01_0001.json     # Labelme OBB Annotation
│   ├── seq_01_0002.bmp
│   ├── seq_01_0002.json
│   ├── ...
└── README.md


@article{tao2026circle,
  title={Circle-Tracker: Geometry-Constrained Stereo Multi-Object Tracking Under Severe Occlusion and Nonlinear Motion},
  author={Tao, Jiang and et al.},
  journal={IEEE Transactions on Instrumentation and Measurement (Under Review)},
  year={2026}
}

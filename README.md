# 🚗 Hybrid Seat Belt Detection System

This project implements a **hybrid template matching system** that combines:
- 🧬 **Genetic Algorithm (GA)** for scale, rotation, and location optimization
- 🧠 **PQ-HOG + ILI (Sibiryakov's method)** for robust and fast descriptor matching (optional)

### 📦 Folder Structure
├── 05_hybrid_matching.ipynb # Main implementation file
├── preprocessed_data/ # Folder with test images (cropped ROIs)
├── results/ # Output folder for matched results

from hybrid_seatbelt_matching import hybrid_detect_batch

hybrid_detect_batch(
    image_folder="test_images",
    template_path="templates/template.jpg",
    output_path="results"
)


📄 Credits
Genetic Algorithm matching from original seat belt detection paper

PQ-HOG concept from Sibiryakov's "Fast Template Matching" method

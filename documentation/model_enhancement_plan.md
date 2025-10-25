## 1. Dataset Integration
Currently, the model was trained on two separate datasets — one for vehicles and people, and another for animals.  
Future work should focus on merging them into a single dataset that includes **all classes together**.  
This will help the model learn better contextual relationships when multiple object types appear in the same frame.

---

## 2. Dataset Diversity
To improve robustness, future datasets should include drone images captured under **diverse conditions**, such as:
- Different altitudes and angles  
- Varying lighting (morning, noon, evening)  
- Mixed terrains and environments  

This variation reduces overfitting and ensures the model performs consistently across real-world scenarios.

---

## 3. Model Enhancements
- Experiment with larger YOLOv8 variants (e.g., **YOLOv8m**, **YOLOv8l**) for better accuracy.  
- Use **data augmentations** such as rotation, brightness adjustments, and Mosaic augmentation to increase training diversity.  
- Fine-tune hyperparameters (learning rate, momentum) for additional performance gains.

---

## 4. Deployment Optimization
When deploying the model on drones:
- Apply **model quantization** or **pruning** to reduce memory usage and accelerate inference.  
- Integrate an **object tracking algorithm** (e.g., SORT, ByteTrack) for smoother, frame-by-frame counting.  
These steps can make real-time detection more efficient on limited onboard hardware.

---

## 5. Continuous Learning
Introduce a **feedback-based retraining loop** where:
- New drone captures and misdetected examples are periodically added back into the dataset.  
- The model is retrained on this expanded dataset to improve accuracy over time.  

This process supports long-term adaptability and continuous improvement of detection reliability.

---

**Document:** `model_enhancement_plan.md`  
**Project:** Drone Vision Detection — Aroha Submission

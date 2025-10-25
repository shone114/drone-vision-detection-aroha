# Calculation Sheet

| **Parameter**           | **Value**                        | **Units**         | **Notes**                  |
|--------------------------|----------------------------------|------------------|----------------------------|
| **Model**                | YOLOv8 (trained on aerial dataset) | —                |                            |
| **Image size**           | 640 × 640                        | px               |                            |
| **Batch size**           | 1(inference) , 16(training)      | —                |                            |
| **Avg inference time**   | ≈ 49 ms per image                | —                | From FPS ≈ 20              |
| **Avg FPS**              | 20.43                            | frames / sec     |                            |
| **Avg objects / frame**  | 15.09                            | objects          |                            |
| **Peak VRAM usage**      | 0.96 GB / 15.36 GB               | GB               | Tesla T4 GPU               |
| **Peak RAM usage**       | —                                | GB               | (CPU not measured)         |
| **Objects / sec**        | ≈ 308                            | objects / sec    |                            |
| **Objects / min**        | ≈ 18,480                         | objects / min    |                            |
| **Objects / hr**         | ≈ 1.1 million                    | objects / hour   |                            |

---

###  Notes
- These values were measured on a **Tesla T4 GPU** during inference.  
- Average FPS and inference time were computed from 20 test images.  
- RAM usage (CPU) was not recorded, as the focus was on GPU performance.  
- Object counts are based on the model’s detections from sample drone imagery.

---

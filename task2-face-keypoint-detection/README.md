# Face Keypoint Detection (Task 2)

This project implements a deep learning system to predict **68 facial landmark coordinates** from face images.

---

## Method

Two convolutional neural network backbones were compared:

- ResNet-18
- ResNet-34

Both models were pretrained on **ImageNet** and fine-tuned for the keypoint detection task.

Key techniques used:

- Transfer learning
- Fully connected regression head
- WingLoss for improved sensitivity to small errors
- Learning rate scheduling
- Early stopping

---

## Evaluation Metrics

Model performance was evaluated using:

- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Mean Euclidean Distance Error (MEDE)

---

## Results

| Model | MSE | MAE | MEDE |
|------|------|------|------|
| ResNet-18 | 43.998 | 4.916 | 7.692 |
| ResNet-34 | 27.488 | 3.908 | 6.165 |

ResNet-34 achieves better performance and reduces the average error by about **20%**.

---

## Files

face_keypoint_detection.ipynb  
Main notebook containing the experiment.

face_results.csv  
Evaluation results generated from the experiments.
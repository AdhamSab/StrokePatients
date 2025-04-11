# 🧠 Stroke Pain Detection App

A Streamlit-based app for automatically assessing pain intensity in stroke patients using facial asymmetry and deep learning.

This project uses three steps:
1. **Detect the affected side** of a stroke patient's face using a Keras-based CNN model.
2. **Crop the unaffected half** of the face.
3. Use a PyTorch model to **predict the pain intensity (PSPI score)** from the expressive half.

---

## 🚀 How to Use This App

Simply upload a **full-face image** of a stroke patient and let the model:
- Detect the affected side
- Crop the unaffected side
- Predict the patient's pain intensity (PSPI)

✅ You can access the live app here:  
[🔗 Launch App →](https://huggingface.co/spaces/AdhamQQ/StrokePatientsModel)


## 💾 Models Used

These models are automatically downloaded on first run:

| Model                             | Description                            | Link                                                                 |
|----------------------------------|----------------------------------------|----------------------------------------------------------------------|
| `cnn_stroke_model.keras`         | Detects the affected side of the face  | [Download](https://huggingface.co/AdhamQQ/cnn_stroke_model/resolve/main/cnn_stroke_model.keras)         |
| `right_side_pain_model.pth`      | Predicts pain intensity (PSPI score)   | [Download](https://huggingface.co/AdhamQQ/cnn_stroke_model/resolve/main/right_side_pain_model.pth)      |

---

## 🧠 Project Goals

This app is part of a larger system to:
- Automatically detect which side of a stroke patient's face is impaired
- Use the **expressive side** to analyze pain using PSPI (Prkachin and Solomon Pain Intensity) scores

---

## ✨ Credits

using:
- Streamlit
- TensorFlow/Keras
- PyTorch
- Hugging Face Hub

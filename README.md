# GPS_SPOOFING_DETECTION_PAPER
 🚗 SafeRoute: GPS Spoofing Detection in Autonomous Vehicles

This project aims to improve the **safety and security of autonomous vehicles (AVs)** by detecting GPS spoofing attacks using machine learning. The goal is to prevent attackers from manipulating GPS signals and causing accidents or wrong turns.

---

## 📌 Why This Project?

Autonomous vehicles rely heavily on **GPS data** for location and navigation. However, attackers can send fake GPS signals (called **spoofing**) that confuse the vehicle’s real location. This project proposes a method to detect such spoofing attacks **early and accurately**.

---

## 💡 What We Did

- ✅ Analyzed common **GPS spoofing attack patterns**.
- ✅ Preprocessed two real-world datasets: **AV-GPS** and **UAV-GPS**.
- ✅ Applied an **autoencoder-based feature selection** to reduce redundancy and keep important features.
- ✅ Built a **hybrid ML model** using:
  - RNN-LSTM (to understand time-based patterns)
  - Random Forest classifier (for final decision)
- ✅ Achieved **up to 99.98% accuracy** in detecting GPS spoofing.

---

## 🔧 How the Model Works

1. **Autoencoder** removes unnecessary and duplicate features from raw GPS data.
2. The cleaned data is passed to a **RNN-LSTM network** to detect movement trends.
3. The final output is classified as "attack" or "safe" using a **Random Forest** model.

---

## 📊 Performance Summary

| Dataset       | Accuracy | F1 Score |
|---------------|----------|----------|
| AV-GPS        | 99.86%   | 0.95     |
| UAV Dataset   | 99.98%   | 0.99     |

✔️ **Improved accuracy and generalization** compared to previous models  
✔️ **Low false alarm rate**  
✔️ **Fast detection time (6.8s)**

---

## 🧪 Sample Results

- Detected spoofed signals injected with positional offsets.
- Demonstrated successful classification across **two different datasets**.
- Used standard metrics: Precision, Recall, F1-Score.

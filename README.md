# DC Motor Sound Analysis and Predictive Maintenance

## 📋 Overview

This repository contains a comprehensive framework for **predictive maintenance of DC motors** through acoustic signal analysis. The project implements both **classical signal processing techniques** and **state-of-the-art deep neural networks** to detect motor anomalies, diagnose faults, and predict maintenance needs before failures occur.

By analyzing the acoustic signatures of DC motors, this system can identify:
- Motor bearing degradation
- Propeller faults
- Winding faults
- Performance anomalies
- Optimal maintenance scheduling

  The dataset is obtained from Kaggle:
  https://www.kaggle.com/datasets/amirberenji/brushless-dc-motor-sound-dataset-for-pdm/data

## 🎯 Key Features

- ✅ **Dual Approach**: Classical methods and deep learning models for comparison
- ✅ **Sound-Based Detection**: Non-invasive acoustic signal analysis
- ✅ **Real-time Analysis**: Immediate fault detection capabilities
- ✅ **Comprehensive Datasets**: Diverse motor conditions and fault scenarios
- ✅ **Feature Engineering**: Advanced signal processing techniques (FFT, MFCC, spectrograms)
- ✅ **Multiple ML Models**: Classical classifiers and deep neural networks
- ✅ **Reproducible Results**: Well-documented Jupyter notebooks with detailed explanations

## 📁 Repository Structure

```
DC-motor-sound-analysis-and-Predictive-maintenance/
│
├── BLDC_Classical_Method.ipynb      # Classical ML approach (FFT, feature extraction, traditional classifiers)
├── BLDC_Deep_NN.ipynb               # Deep learning approach (CNN, autoencoders, neural networks)
├── Dataset/                         # Motor sound recordings and labels
│   ├── normal_operation/            # Healthy motor acoustic data
│   ├── bearing_fault/               # Bearing damage recordings
│   ├── Propeller_fault/             # Misalignment fault data
├── Images/                          # Visualizations and results
└── README.md                        # This file
```

## 🔬 Methodology

### 1. **Classical Signal Processing Approach** (BLDC_Classical_Method.ipynb)
   - **Signal Processing**: FFT, spectral analysis, time-domain features
   - **Feature Extraction**: Energy, entropy, peak frequency, harmonic analysis
   - **Algorithms**: Random Forest, SVM, Decision Trees, Naive Bayes
   - **Advantages**: Interpretable, computationally efficient, domain knowledge driven

### 2. **Deep Learning Approach** (BLDC_Deep_NN.ipynb)
   - **Model Architecture**: Convolutional Neural Networks (CNN), Autoencoders
   - **Input Representation**: Spectrograms, mel-frequency cepstral coefficients (MFCC)
   - **Advantages**: Automatic feature learning, superior pattern recognition

## 🚀 Getting Started

### Prerequisites
```bash
python >= 3.7
jupyter
numpy
pandas
scipy
scikit-learn
matplotlib
librosa
tensorflow (for deep learning notebook)
```

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/PGuruPrasaath/DC-motor-sound-analysis-and-Predictive-maintenance.git
   cd DC-motor-sound-analysis-and-Predictive-maintenance
   ```

2. **Create virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install numpy pandas scipy scikit-learn matplotlib librosa jupyter tensorflow
   ```

4. **Launch Jupyter**:
   ```bash
   jupyter notebook
   ```

## 📊 Usage

### Classical Method
Open `BLDC_Classical_Method.ipynb` to:
- Load and preprocess acoustic data
- Extract hand-crafted features
- Train traditional machine learning classifiers
- Evaluate model performance with detailed metrics
- Visualize frequency spectra and feature importance

### Deep Learning Method
Open `BLDC_Deep_NN.ipynb` to:
- Build and train deep neural networks
- Implement CNN-based acoustic classification
- Use transfer learning approaches
- Compare performance with classical methods
- Generate predictions on new motor recordings

## 🔍 Fault Detection Capabilities

| Fault Type | Description |
|---|---|
| **Normal Operation** | Healthy motor baseline |
| **Bearing Fault** | Degradation, friction noise |
| **Propeller Fault** | Structural misalignment |

## 💡 Key Insights

- **Acoustic Signatures**: Each fault type produces distinct acoustic patterns
- **Early Warning System**: Detectable changes occur weeks before catastrophic failure
- **Non-invasive Monitoring**: No need for additional sensors beyond microphone
- **Generalization**: Models trained on one motor type can transfer to similar motors

## 🛠️ Customization

### Using Your Own Data
1. Record motor acoustic data (16+ kHz sampling rate recommended)
2. Organize files in the `Dataset/` folder by condition
3. Update file paths in notebooks
4. Re-run feature extraction and model training

### Adjusting Models
- Modify feature extraction parameters in classical notebooks
- Adjust neural network architecture in deep learning notebook
- Tune hyperparameters for your specific use case

## 📚 References & Theory

- **Signal Processing**: Welch's method, Short-Time Fourier Transform (STFT)
- **Feature Engineering**: Time-domain, frequency-domain, and time-frequency features
- **Machine Learning**: Scikit-learn documentation, classical classifiers
- **Deep Learning**: CNN architectures, attention mechanisms, autoencoders

## 🤝 Contributing

Contributions are welcome! Areas for improvement:
- Add more motor fault scenarios
- Implement real-time monitoring dashboard
- Deploy as REST API service
- Add transfer learning experiments
- Optimize model inference speed

Please fork the repository and submit pull requests!

## 📝 License

This project is licensed under the MIT License.

## 📧 Contact & Support

**Author**: PGuruPrasaath

For questions, suggestions, or collaborations, please open an issue on GitHub.

---

**Last Updated**: 2026-03-24 21:46:22

⭐ **If this project helped you, consider starring it!**

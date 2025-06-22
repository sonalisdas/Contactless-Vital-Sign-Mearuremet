Contactless Vital Sign Measurement Using Thermal Imaging

🔍 Overview

This project focuses on a non-invasive, AI-powered system for measuring vital signs like respiratory rate and fever detection using thermal imaging. Inspired by the need for safer neonatal care and remote health monitoring, this system eliminates physical contact, making it ideal for infection-prone or high-risk environments.

🧠 Problem Statement

Traditional vital sign monitoring methods in neonatal or pandemic settings involve contact-based sensors that can cause discomfort or increase the risk of infection. The challenge was to build a contactless, accurate, and low-cost system to monitor breathing rate and detect fever using thermal cameras only, without relying on RGB data.

🛠️ Tech Stack

Programming Language: Python

Libraries: OpenCV, NumPy, SciPy, Scikit-learn, Matplotlib

ML Models: Random Forest, Gradient Boosting (Ensemble)

Hardware Used: Thermal Camera (FLIR Thermal-compatible)

Environment: Jupyter Notebook

⚙️ Methodology

Thermal Video Acquisition

Captured thermal videos of the subject's face/chest using a low-resolution thermal camera.

Preprocessing

Applied Gaussian filters and image thresholding

Stabilized thermal frames to reduce motion artifacts

Fever Detection

Extracted temperature values from facial regions

Compared with a calibrated threshold to classify fever presence

Breathing Rate Estimation

Analyzed pixel intensity fluctuations in the nasal/thoracic region

Performed FFT (Fast Fourier Transform) to detect periodic breathing patterns

Trained an ensemble ML model (Random Forest + Gradient Boosting) on extracted features to predict breaths per minute (BPM)

✅ Results

Fever detection: Achieved ~98% accuracy in binary classification (fever/no fever)

Breathing rate prediction: Achieved 91% accuracy using ensemble learning

Real-time capable with optimized frame processing

🏆 Achievements

Secured ₹2.5L seed grant from Christ University under the Student Innovation Fund

Recognized under Public Health Innovation category

Demonstrated during university exhibitions and presented to healthcare tech mentors

🌍 Impact & Future Scope

This project lays the groundwork for smart ICU monitoring, home quarantine kits, and infant monitoring systems in resource-constrained environments. Future developments include:

Integrating heart rate prediction

Deploying on edge devices (like Raspberry Pi with thermal camera)

Real-time dashboard with alert mechanisms


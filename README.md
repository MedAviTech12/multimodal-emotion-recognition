# multimodal-emotion-recognition
A multimodal emotion recognition framework integrating EEG, thermal imaging, and digital facial images for affective computing and healthcare applications.

# Multimodal Emotion Recognition using EEG, Thermal Imaging, and Digital Facial Images

This project presents a multimodal emotion recognition framework that integrates electroencephalography (EEG) signals, thermal facial imaging, and digital facial images for emotion classification.

The study investigates the relationship between neural activity, physiological responses, and facial expressions by combining multiple data modalities into a unified emotion recognition system. The framework incorporates data acquisition, preprocessing, feature extraction, multimodal fusion, correlation analysis, and machine learning-based classification.

Data were collected from 50 participants exposed to emotion-inducing stimuli representing six emotional states: Happy, Sad, Neutral, Anger, Fear, and Surprise. The project evaluates both traditional machine learning and deep learning approaches to improve emotion recognition performance through multimodal fusion.

The work demonstrates the potential of combining neurophysiological and imaging modalities for affective computing, healthcare applications, mental health monitoring, and intelligent human-computer interaction systems.

## Key Features

* Multimodal Emotion Recognition Framework
* EEG, Thermal, and Digital Facial Data Integration
* Six-Class Emotion Classification
* Feature-Level, Decision-Level, and Hybrid Fusion
* Correlation Analysis Across Modalities
* Machine Learning and Deep Learning Models
* Real-World Emotion Dataset Collection
* Healthcare and Affective Computing Applications

## Project Overview

Traditional facial emotion recognition systems rely primarily on visible facial expressions and often suffer from challenges such as lighting variations, facial occlusions, and subtle emotional expressions. This project addresses these limitations by integrating three complementary modalities: EEG signals, thermal facial images, and digital facial images.

The proposed framework analyzes neural activity, physiological responses, and visual facial characteristics simultaneously to provide a more comprehensive representation of human emotions. By leveraging multimodal fusion techniques, the system improves emotion recognition robustness and classification performance compared to single-modality approaches.
## Dataset Description
<img width="494" height="377" alt="image" src="https://github.com/user-attachments/assets/4e278454-a8a0-4bf9-b786-7b51d7d957d4" />
<img width="463" height="280" alt="image" src="https://github.com/user-attachments/assets/73f12f63-4639-47fe-85de-b334d5315a2d" />
<img width="450" height="284" alt="image" src="https://github.com/user-attachments/assets/6199d90e-893c-4140-9e61-382f07269e27" />


### Participants

The study involved 50 healthy participants aged between 20 and 30 years. All participants provided informed consent prior to data collection. Ethical approval for the study was obtained from the Institutional Ethics Committee of SRM Hospital and Research Centre (SRMHRC), Kattankulathur, Tamil Nadu, India.

### Emotion Categories

Six emotional states were considered in this study:

* Happy
* Sad
* Neutral
* Anger
* Fear
* Surprise

These emotions were induced using carefully selected video stimuli designed to evoke specific emotional responses.

### Data Modalities

Three complementary data modalities were collected for each participant:

#### EEG Signals

Brain activity was recorded using a 16-channel EEG acquisition system following the international 10-20 electrode placement protocol. EEG signals provide direct neural indicators of emotional processing.

#### Thermal Facial Images

Thermal images were acquired using an infrared thermal camera to capture facial temperature variations associated with physiological responses to emotional stimuli.

#### Digital Facial Images

Visible-spectrum facial images were captured to record facial expressions and appearance-based emotional cues.

### Dataset Objective

The dataset was designed to investigate the relationships between neural activity, physiological responses, and facial expressions during emotional experiences. The multimodal nature of the dataset enables comprehensive emotion analysis and supports the development of robust emotion recognition systems.
## Experimental Setup

### Data Acquisition Environment

All experiments were conducted in a temperature-controlled laboratory environment maintained at approximately 21°C to ensure consistency during data collection and minimize external influences on physiological measurements.

Participants were seated approximately 2 meters from a projection screen displaying emotion-inducing video stimuli. The acquisition process was designed to ensure synchronized collection of EEG signals, thermal facial images, and digital facial images.

### Emotion Induction Protocol

Emotional responses were elicited using carefully selected video clips representing six emotional categories:

| Emotion  | Stimulus Type                         |
| -------- | ------------------------------------- |
| Happy    | Joyful and humorous video clips       |
| Sad      | Emotional and tragic scenes           |
| Anger    | Conflict and aggression-related clips |
| Fear     | Horror and suspense content           |
| Surprise | Unexpected visual events              |
| Neutral  | Calm and nature-based visuals         |

Each stimulus session lasted approximately 60 seconds and was designed to evoke measurable emotional responses across all modalities.

### EEG Acquisition System

EEG signals were recorded using a 16-channel acquisition system based on the international 10-20 electrode placement standard.

**Key Specifications**

* Sampling Rate: 100 Hz
* Band-Pass Filter Range: 0.5–50 Hz
* Recording Channels: Frontal, Central, and Occipital Regions
* Reference Electrodes: Fp1 and Fp2

The EEG recordings were synchronized with image acquisition systems to support multimodal analysis.

### Thermal Imaging System

Thermal facial images were captured using a FLIR A305SC infrared thermal camera.

**Key Specifications**

* Resolution: 320 × 240 pixels
* Spectral Range: 7.5–13 µm
* Temperature Sensitivity: ±0.05°C
* Frame Rate: 30 Hz

Thermal recordings captured facial heat distribution patterns associated with physiological responses to emotional stimuli.

### Digital Imaging System

Digital facial images were collected using a high-resolution DSLR camera under controlled lighting conditions.

**Key Specifications**

* Resolution: 1920 × 1080 pixels
* Frame Rate: 60 fps
* Controlled LED Illumination

The digital imaging setup captured facial expression changes corresponding to different emotional states.
## Data Preprocessing

Data preprocessing was performed separately for EEG signals, thermal facial images, and digital facial images to improve data quality and ensure reliable feature extraction. The preprocessing pipeline was designed to reduce noise, remove artifacts, and standardize inputs across all modalities.

### EEG Signal Preprocessing

The EEG signals were preprocessed to eliminate noise and improve signal quality prior to feature extraction.

#### Preprocessing Steps

* Band-pass filtering (0.5–50 Hz) to remove low-frequency drift and high-frequency noise.
* Removal of motion and environmental artifacts.
* Signal normalization to ensure consistency across participants.
* Segmentation of EEG recordings based on emotion-specific stimulus intervals.
* Extraction of frequency bands including Delta, Theta, Alpha, Beta, and Gamma.

#### Objective

The preprocessing stage enhanced neural signal quality and enabled reliable extraction of emotion-related brain activity patterns.

### Thermal Image Preprocessing

Thermal facial images were processed to improve temperature distribution analysis and highlight physiologically relevant regions.

#### Preprocessing Steps

* Conversion of thermal recordings into analyzable image frames.
* Noise reduction and image enhancement.
* Facial region detection and cropping.
* Temperature normalization across samples.
* Region-of-interest (ROI) extraction from key facial areas.

#### Objective

The preprocessing pipeline improved the visibility of temperature variations associated with emotional responses and physiological changes.

### Digital Facial Image Preprocessing

Digital facial images were standardized to reduce variations caused by lighting conditions and image acquisition differences.

#### Preprocessing Steps

* Face detection and alignment.
* Image resizing to a uniform resolution.
* Illumination normalization.
* Noise reduction and contrast enhancement.
* Facial region extraction for feature analysis.

#### Objective

The preprocessing stage ensured consistent facial representations and improved the robustness of facial feature extraction.

### Multimodal Data Preparation

After individual preprocessing, data from all three modalities were organized and synchronized for subsequent feature extraction, correlation analysis, and multimodal fusion. This ensured that neural, physiological, and visual information corresponding to the same emotional stimulus could be analyzed collectively.
## Feature Extraction

Feature extraction was performed independently for EEG signals, thermal facial images, and digital facial images to capture neural, physiological, and visual indicators of emotional responses. The extracted features served as the foundation for subsequent correlation analysis, multimodal fusion, and emotion classification.

### EEG Feature Extraction

EEG signals were analyzed in both the time and frequency domains to identify neural patterns associated with emotional states.

#### Extracted Features

* Delta Band Power (0.5–4 Hz)
* Theta Band Power (4–8 Hz)
* Alpha Band Power (8–13 Hz)
* Beta Band Power (13–30 Hz)
* Gamma Band Power (>30 Hz)
* Mean Signal Amplitude
* Standard Deviation
* Signal Energy
* Power Spectral Density (PSD)

#### Significance

Frequency-band analysis enabled the identification of emotion-related neural activity patterns, with Theta and Alpha bands showing strong associations with emotional processing.

### Thermal Image Feature Extraction

Thermal facial images were analyzed to quantify physiological changes reflected through facial temperature distributions.

#### Extracted Features

* Mean Facial Temperature
* Maximum Temperature
* Minimum Temperature
* Temperature Variance
* Thermal Entropy
* Regional Temperature Distribution
* Facial Heat Map Characteristics

#### Significance

Thermal features captured involuntary physiological responses to emotional stimuli and provided objective indicators of emotional arousal.

### Digital Facial Image Feature Extraction

Digital facial images were processed to extract appearance-based emotional cues.

#### Extracted Features

* Histogram of Oriented Gradients (HOG)
* Facial Landmark Measurements
* Texture Descriptors
* Facial Region Statistics
* Expression-Based Geometric Features

#### Significance

These features represented facial expression variations associated with different emotional states and provided complementary visual information for emotion recognition.

### Multimodal Feature Representation

The extracted features from EEG, thermal imaging, and digital facial imaging were combined to create a comprehensive representation of emotional responses.

This multimodal feature space enabled the integration of:

* Neural Activity (EEG)
* Physiological Responses (Thermal Imaging)
* Visual Facial Expressions (Digital Imaging)

The resulting feature set formed the basis for correlation analysis, feature-level fusion, decision-level fusion, and deep learning-based emotion classification.
## Correlation Analysis

Correlation analysis was performed to investigate the relationships between neural activity, physiological responses, and facial expressions across different emotional states. The objective was to determine whether changes observed in one modality were associated with corresponding changes in other modalities.

### Purpose of Correlation Analysis

The multimodal nature of emotional responses suggests that emotions are simultaneously reflected through:

* Brain activity (EEG signals)
* Physiological responses (Thermal Imaging)
* Facial expressions (Digital Facial Images)

Correlation analysis was conducted to evaluate the strength of these relationships and identify complementary patterns across modalities.

### EEG–Thermal Correlation

A detailed analysis was performed between EEG frequency-domain features and thermal imaging characteristics.

#### Example Investigation

* EEG Feature: Theta Band Power
* Thermal Feature: Thermal Entropy
* Emotion Class: Surprise

The analysis revealed a positive relationship between neural activation and thermal facial responses, indicating that emotionally arousing stimuli can simultaneously influence both brain activity and physiological temperature variations.

### Significance of Findings

The observed correlations support the hypothesis that emotions manifest through multiple interconnected physiological mechanisms rather than a single observable response.

Key observations include:

* Strong associations between neural and physiological responses during emotionally intense states.
* Improved understanding of multimodal emotional behavior.
* Evidence supporting the integration of EEG and thermal features for enhanced emotion recognition.
* Validation of multimodal fusion approaches for affective computing applications.

### Visualization and Analysis

Correlation matrices, scatter plots, and statistical analyses were generated to evaluate relationships between extracted features from different modalities.

These analyses provided valuable insights into how neural, physiological, and visual indicators interact during emotional experiences and contributed to the design of robust multimodal emotion recognition models.
## Multimodal Fusion

Multimodal fusion was implemented to combine information from EEG signals, thermal facial images, and digital facial images into a unified emotion recognition framework. The objective was to leverage the complementary strengths of each modality and improve classification performance compared to unimodal approaches.

### Feature-Level Fusion

Feature-level fusion was performed by combining extracted features from all three modalities into a single feature vector prior to classification.

#### Fusion Workflow

EEG Features
+
Thermal Features
+
Digital Image Features
↓
Combined Feature Vector
↓
Machine Learning Classification

#### Advantages

* Preserves detailed information from individual modalities.
* Enables the classifier to learn cross-modal relationships.
* Improves emotion discrimination capability.

### Decision-Level Fusion

Decision-level fusion was implemented by independently classifying each modality and combining their prediction outputs to generate a final emotion label.

#### Fusion Workflow

EEG Classifier Prediction
+
Thermal Classifier Prediction
+
Digital Image Classifier Prediction
↓
Decision Aggregation
↓
Final Emotion Prediction

#### Advantages

* Allows independent optimization of each modality.
* Improves robustness when one modality performs poorly.
* Reduces sensitivity to missing or noisy data.

### Hybrid Fusion Strategy

A hybrid fusion approach was also investigated to combine the strengths of both feature-level and decision-level fusion techniques.

The hybrid framework aimed to:

* Capture low-level feature interactions.
* Preserve modality-specific decision information.
* Improve overall classification accuracy.
* Enhance robustness across different emotional states.

### Importance of Multimodal Fusion

The fusion of neural, physiological, and facial expression information provides a more comprehensive representation of emotional responses than any individual modality.

The results demonstrate that multimodal fusion significantly improves emotion recognition performance and supports the development of reliable affective computing systems for healthcare, human-computer interaction, and mental health monitoring applications.
## Classification Models

To evaluate the effectiveness of multimodal emotion recognition, both traditional machine learning algorithms and deep learning architectures were implemented and compared.

### Machine Learning Models

Several supervised machine learning classifiers were trained using features extracted from EEG signals, thermal facial images, and digital facial images.

#### Decision Tree (DT)

The Decision Tree classifier demonstrated the highest overall performance among traditional machine learning approaches.

**Advantages**

* Interpretable decision-making process
* Efficient training and inference
* Strong performance on multimodal feature sets

#### k-Nearest Neighbors (k-NN)

The k-NN classifier was used as a distance-based learning approach for emotion classification.

**Advantages**

* Simple implementation
* Effective for non-linear decision boundaries
* Useful baseline classifier

#### Multi-Layer Perceptron (MLP)

A feedforward neural network was implemented to learn complex relationships within the multimodal feature space.

**Advantages**

* Ability to model non-linear patterns
* Improved generalization compared to traditional classifiers
* Suitable for high-dimensional multimodal data

### Deep Learning Models

Deep learning architectures were explored to automatically learn spatial and temporal representations from multimodal data.

#### VGG + CNN Architecture

The VGG-based convolutional neural network was used for image feature extraction and emotion classification.

**Strengths**

* Effective spatial feature extraction
* Strong performance on facial image data
* Robust visual pattern recognition

#### ResNet50 + LSTM Hybrid Architecture

A hybrid deep learning framework combining ResNet50 and Long Short-Term Memory (LSTM) networks was developed.

**Architecture Components**

* ResNet50 for extracting spatial features from digital and thermal images.
* LSTM for capturing temporal patterns in EEG signals.
* Integrated multimodal learning framework.

**Advantages**

* Simultaneous modeling of spatial and temporal information.
* Improved representation learning across modalities.
* Enhanced recognition of complex emotional states.

### Model Evaluation

The performance of all classifiers was evaluated using emotion classification accuracy and comparative analysis across individual and fused modalities.

The comparison enabled the identification of the most effective machine learning and deep learning approaches for multimodal emotion recognition.
## Results and Performance

The experimental evaluation demonstrated that multimodal emotion recognition significantly outperforms traditional single-modality approaches. By integrating EEG signals, thermal facial imaging, and digital facial images, the framework achieved highly accurate and robust emotion classification across six emotional states.

### Performance of Individual Modalities

| Modality              | Best Classifier | Accuracy |
| --------------------- | --------------- | -------- |
| EEG Signals           | Decision Tree   | 98.3%    |
| Thermal Imaging       | Decision Tree   | 98.3%    |
| Digital Facial Images | Decision Tree   | 95.0%    |

The results indicate that EEG and thermal imaging provide stronger emotion-related information than digital facial images alone. Physiological and neural responses proved to be more reliable indicators of emotional states, while facial expressions remained susceptible to environmental factors such as lighting conditions, facial occlusions, and voluntary expression control.

### Multimodal Fusion Performance

The integration of EEG, thermal, and digital image features produced the highest overall classification performance.

#### Key Findings

* Multimodal fusion improved classification accuracy by approximately 15–20% compared to single-modality systems.
* Combined neural, physiological, and visual information provided a more comprehensive representation of emotional responses.
* Feature-level and decision-level fusion significantly enhanced system robustness.

### Machine Learning Model Comparison

Among all traditional machine learning algorithms, the Decision Tree classifier consistently achieved the highest classification accuracy across individual modalities and fused datasets.

#### Performance Summary

* Decision Tree (DT): Best overall performance
* k-Nearest Neighbors (k-NN): Moderate performance
* Multi-Layer Perceptron (MLP): Competitive performance with higher computational complexity

### Deep Learning Model Evaluation

Two deep learning architectures were evaluated for multimodal emotion recognition.

| Model           | Accuracy           |
| --------------- | ------------------ |
| VGG + CNN       | Strong Performance |
| ResNet50 + LSTM | 95.0%              |

The hybrid ResNet50 + LSTM architecture achieved the highest deep learning performance by effectively combining:

* Spatial feature extraction from thermal and digital facial images.
* Temporal pattern analysis from EEG signals.

The model demonstrated superior performance for challenging emotional states such as Fear and Sadness by capturing both visual and neural information simultaneously.

### Key Contributions

* Demonstrated the effectiveness of multimodal emotion recognition.
* Validated the importance of EEG and thermal imaging for affective computing.
* Established strong correlations between neural activity and physiological responses.
* Achieved high classification accuracy using both machine learning and deep learning approaches.
* Provided a scalable framework for future emotion-aware healthcare and human-computer interaction systems.
## Applications

The proposed multimodal emotion recognition framework has potential applications across healthcare, affective computing, human-computer interaction, security, and rehabilitation. By combining neural, physiological, and facial expression data, the system provides a comprehensive understanding of human emotional states.

### Mental Health Monitoring

The integration of EEG and thermal imaging enables continuous assessment of emotional well-being and psychological states.

Potential applications include:

* Early detection of stress, anxiety, and depression.
* Emotion-aware biofeedback systems.
* Continuous emotional monitoring using wearable devices.
* Support for mental health interventions and therapy.

### Affective Computing

Emotion-aware systems can enhance interactions between humans and intelligent machines.

Potential applications include:

* Emotion-sensitive virtual assistants.
* Adaptive chatbots and conversational AI.
* Personalized learning platforms.
* Emotion-responsive gaming and virtual reality environments.

### Human-Computer Interaction (HCI)

Multimodal emotion recognition can improve user experience by enabling systems to respond dynamically to emotional states.

Potential applications include:

* Intelligent user interfaces.
* Adaptive educational technologies.
* Emotion-aware recommendation systems.
* Personalized digital experiences.

### Healthcare and Rehabilitation

Emotion recognition can support diagnosis, therapy, and rehabilitation programs.

Potential applications include:

* Post-stroke emotional rehabilitation.
* Autism Spectrum Disorder (ASD) therapy support.
* Cognitive and behavioral health assessment.
* Patient monitoring in clinical environments.

### Security and Surveillance

Physiological and neural indicators can provide additional insights beyond facial expressions alone.

Potential applications include:

* Behavioral analysis systems.
* Driver fatigue and stress monitoring.
* Emotion-aware security screening.
* Research on deception and stress detection.
## Future Scope

While the proposed framework demonstrates strong performance in multimodal emotion recognition, several opportunities exist for further improvement and real-world deployment.

### Potential Future Enhancements

* Development of real-time emotion recognition systems with low-latency processing.
* Integration with wearable EEG devices and smart healthcare platforms.
* Expansion of the dataset to include larger and more diverse participant populations.
* Investigation of cross-cultural and multilingual emotional expressions.
* Deployment on edge-computing platforms for portable emotion monitoring.
* Exploration of Transformer-based multimodal fusion architectures.
* Implementation of attention mechanisms for adaptive feature selection.
* Integration with mental health monitoring and rehabilitation systems.

### Long-Term Vision

The long-term objective is to develop scalable and real-time emotion-aware systems capable of supporting healthcare, education, rehabilitation, and human-computer interaction applications through intelligent analysis of neural, physiological, and visual emotional indicators.
## Documentation

The repository contains the following project resources:

* IEEE Conference Publication
* Final Project Report
* Project Presentation
* Experimental Results and Performance Analysis
* Correlation Analysis Outputs
* Feature Extraction Visualizations
* System Architecture and Workflow Diagrams

## Author

**Abhishek Kumar Jha**

Biomedical Engineering Graduate

### Areas of Interest

* Medical Artificial Intelligence
* Neuroengineering
* Medical Imaging
* Affective Computing
* Biomedical Signal Processing
* Intelligent Healthcare Systems

### Repository Purpose

This repository serves as a documentation and research showcase of the multimodal emotion recognition project, including methodology, experimental design, analysis, and results.

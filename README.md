# WLARM
This dataset is designed for research on WiFi-based sensing, including indoor localization, human activity recognition, and respiration monitoring. It is collected using USRP devices with WiFi CSI and organized to support training and evaluation of models under different environmental and spatial configurations.//
📂 Dataset Structure
├── 1.5m/           # CSI data collected at 1.5 meters between TX and RX
├── 2m/             # Data at 2.0 meters
├── 2.5m/
├── 3m/
├── 3.5m/
├── 4m/
├── corridor/       # Data collected in a narrow corridor
├── office/         # Data collected in an office environment
├── open_hall/      # Data collected in a large open hall
├── WLARM/          # Additional dataset for model comparison
Description
Each distance folder (1.5m, 2m, ..., 4m) contains CSI sequences collected at fixed transceiver distances under controlled motion and respiration states.
Each environment folder (corridor, office, open_hall) contains data collected in corresponding real-world indoor scenes, with transceiver distance fixed at 2 meters.
The WLARM folder contains a mixed dataset used specifically for evaluating cross-model performance and generalization benchmarks.
Notes
CSI is preprocessed using the APVF subcarrier selection method.

Respiration and motion labels are provided in sequence-level annotations.

Data collected using USRP2954 SDR platforms at 5.32 GHz, sampling rate: 100 Hz.

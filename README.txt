# 2.45 GHz LNA Simulation – Gain, Noise Figure & Equivalent Noise Temperature

This project models a narrowband 2.45 GHz Low Noise Amplifier (LNA) using Python.  
It simulates key RF performance metrics—Gain, Noise Figure (NF), and Equivalent Noise Temperature (Te)—using lightweight analytical models suitable for RF test-automation portfolios.

The notebook demonstrates:
- Creation of a frequency axis around 2.45 GHz  
- Gaussian-based gain modelling  
- NF modelling with ripple  
- Te calculation from NF  
- Visualizations (individual & combined plots)  
- Export of figures to the `/figures` folder  

---

## Features

### **1. LNA Gain Model**
- Peak gain: **20 dB** at **2.45 GHz**  
- Narrowband Gaussian model  
- Optional dynamic clipping for realism  

### **2. Noise Figure (NF) Model**
- Achieves **1.2 dB** at center  
- Small ±0.1 dB ripple to simulate measurable hardware behavior  

### **3. Equivalent Noise Temperature**
- Computed from NF using:  
  `Te = (10^(NF/10) − 1) * 290 K`  
- Typical simulated value near **92 K** at 2.45 GHz  

### **4. Combined Visualization**
You get:
- Gain (dB)  
- Noise Figure (dB)  
- Te (K)  
All on a single composite plot.

PNG images are automatically saved in:

figures/
combined_gain_nf_te.png
gain_db.png
noise_figure_db.png


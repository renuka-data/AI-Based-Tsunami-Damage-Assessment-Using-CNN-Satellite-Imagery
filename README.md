# AI-Based-Tsunami-Damage-Assessment-Using-CNN-Satellite-Imagery
This project develops an Artificial Intelligence system to automatically detect and localize disaster damage from satellite images captured before and after a tsunami event.
Using Deep Learning and Computer Vision techniques, the model learns terrain changes and identifies affected regions. The system also implements Explainable AI (Grad-CAM) to visually highlight the areas where destruction has occurred.

The goal is to support: Disaster response teams
                        Government agencies
                        Urban planning & recovery analysis
                        Environmental monitoring
Key Features: Satellite image preprocessing & pairing (pre vs post disaster)
              Spectral vegetation analysis (NDVI & EVI)
              Terrain change detection
              Deep Learning based damage prediction
              CNN-based image comparison model
              Explainable AI visualization using Grad-CAM
              Damage heatmap localization
              Each Before image has a corresponding After image of the same location.
Technologies Used: Python, TensorFlow / Keras, OpenCV, NumPy, Matplotlib, Raster based spectral analysis, Explainable AI (Grad-CAM)
Methodology: 1. Image Preprocessing => Image resizing, Pixel normalization, Pair matching (Before → After)
             2. Spectral Analysis => Vegetation indices were used to measure environmental damage, NDVI (Normalized Difference Vegetation Index), EVI (Enhanced Vegetation Index), Dectected Entities: vegetation loss, soil exposure, flooded terrain
             3. Deep Learning Model (CNN) => A Convolutional Neural Network compares the before and after images to learn structural terrain differences such as: collapsed buildings, shoreline changes, vegetation loss, debris spread, The model outputs a damage score.
             4. Explainable AI — Grad-CAM => Grad-CAM highlights which image regions influenced the model's decision.

Output: 🔴 Red → severe damage
        🟡 Yellow → moderate damage
        🔵 Blue → minimal/no damage

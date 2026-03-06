# first-cnn-mnist
CNN model for handwritten digit classification using TensorFlow
Image (28×28)
     ↓
Couche Conv2D      → détecte les contours
     ↓
Couche MaxPooling  → réduit la taille
     ↓
Couche Flatten     → transforme en vecteur 1D
     ↓
Couche Dense       → classifie 0 à 9

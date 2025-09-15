# aynpath-object_detection

## Overview
This repository provides the **TFLite object detection model** and **labels** used in the *Ayn-Path Mobile App* for real-time indoor object detection and navigation assistance.

## Usage
1. Place the `.tflite` model inside your `assets/models/` folder.  
2. Update `pubspec.yaml` to include the model:  

```yaml
flutter:
  assets:
    - assets/models/object_detection.tflite
```

## Notes/Limitations
* Make sure the input image size matches the model’s required dimensions (e.g., 300x300).
* Use the tflite_flutter_helper package for easier image preprocessing. For this project, I use the older version for all the dependencies due to the compatibility of my android device:
```yaml
dependencies:
  tflite_flutter: ^0.9.0
  tflite_flutter_helper: ^0.2.1
  image: ^3.2.0
```
    

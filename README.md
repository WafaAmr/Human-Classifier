# Human Classifier

A simple Python app to classify GAN-generated images. There are two models to choose from: a high-quality model (HQ) with **challenging** images and a low-quality model (LQ) with relatively more straightforward digits. Each model has a total of 10 classes, with each class containing 100 images.

![UI](./UI.jpg)
## Installation

```bash
pip install pillow
```
## Usage

* Clone this repository
  ```bash
  git clone https://github.com/WafaAmr/Human-Classifier.git
  ```
* Uncomment one of the models in the `human_classifier.py` file
  ```python
  5: # model = 'HQ'
  6: # model = 'LQ'
  ```
* Run the code
  ```bash
  python human_classifier.py
  ```
* Use the **the number keys** <kbd>0-9</kbd> or the GUI to classify the images. The <kbd>enter</kbd> key is mapped to the "Unknown" class. If you need some reference images, take a look at [the training Dataset](./reals.png).

* Each classification will be saved as a new line in the TXT file named `<MODEL>-labels.txt` in the top directory.

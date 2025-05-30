# Python DIY-GIF Generator ૮ ˶ᵔ ᵕ ᵔ˶ ა
<p align="center">
  <img src="cinnamonroll.gif" alt="Cinnamonroll GIF" width="250"/>
</p>

This simple project creates an animated GIF from a sequence of PNG images using the `imageio` library in Python. It's a simple and effective way to stitch multiple images into a smooth animation.


Tested and developed using ***Google Colab*** [![***Google Colab***](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gowthamee18/gif-diy/blob/main/gif_diy.ipynb)

## 📁 Files Included

- `1.png` to `5.png`: Input images (frames of the animation)
- `cinnamonroll.gif`: Output animated GIF
- `gif_diy.ipynb`: Colab notebook containing the code

## 🔧 Setup

In Colab or your Jupyter environment, install the required package:

```python
!pip3 install imageio
```

## ♡ How to Use ♡

1. Open [`gif_diy.ipynb`](https://colab.research.google.com/) in Google Colab.
2. Upload all the image files (`1.png` to `5.png`) to your Colab session.
3. Run the notebook cells.
4. The script reads the images and creates `cinnamonroll.gif`.

## 💡 How It Works

```python
import imageio.v3 as iio

filenames = ['1.png', '2.png', '3.png', '4.png', '5.png']
images = [iio.imread(fname) for fname in filenames]

iio.imwrite('cinnamonroll.gif', images, duration=200, loop=0)
```



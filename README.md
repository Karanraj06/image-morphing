# Image-Morphing

## File Structure

```
.
├── .gitignore
├── LICENSE
├── README.md
├── images
│   ├── image1.jpg
│   └── image2.jpg
├── input.txt
├── main.ipynb
├── requirements.txt
└── shape_predictor_68_face_landmarks.dat
```

## Usage

- Install the required python packages using

```
pip3 install -r requirements.txt
```

- Run the code with

```
python3 main.py
```

- The output gifs are saved as `output1.gif` and `output2.gif`

## Summary

This python program takes two images and produces a gif by gradually transforming one image into another. To create the morphed image, we use Delaunay triangulation to divide the image into small triangles. To create each frame of the gif, we compute the morphed triangle for all triangles in the image using a specific alpha value. In other words, we transform each small triangle in the image by a certain amount specified by the alpha value, and then use these transformed triangles to create the next frame of the gif.

The implementation details are explained within the code. The output of Part A is saved as `output1.gif`, while the output of Part B is saved as `output2.gif`.
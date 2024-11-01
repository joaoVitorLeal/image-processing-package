# image-processing-jvlc

## Description
The **image-processing-jvlc** package provides tools for image processing, including operations for adjustment and visualization. The package’s main functionalities include:

### Main Features
- **Histogram Matching**: Matches the histogram of an image to that of another image.
- **Structural Similarity**: Computes the structural similarity between two images, ideal for detailed comparisons.
- **Resize Image**: Resizes images to specified dimensions.

### Utilities
- **Read Image**: Loads an image from a file.
- **Save Image**: Saves the processed image to a file.
- **Plot Image**: Displays an image.
- **Plot Result**: Compares and displays images side-by-side.
- **Plot Histogram**: Shows the histogram of an image for pixel distribution analysis.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install **image-processing-jvlc**:

```bash
# With PyPi test
pip install -i https://test.pypi.org/simple/ image-processing-jvlc==0.0.1

# or

# Directly Pypi
pip install image-processing-jvlc
```

## Usage
- **Here’s an example of how to use the package to resize an image and display the result:**
```python
from image_processing_jvlc.processing import transformation
from image_processing_jvlc.utils import io, plot

# Load an image
image = io.read_image("path/to/image.jpg")

# Resize the image
resized_image = transformation.resize_image(image, (200, 200))

# Display the original and resized images
plot.plot_image(image, title="Original Image")
plot.plot_image(resized_image, title="Resized Image")

```

## Author
João Vitor Leal de Castro

## License
This project is licensed under the MIT license.

[MIT](https://choosealicense.com/licenses/mit/)

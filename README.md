# Download Images and Background Images

This project consists of a Javascript script that allows to download all the images and background images from a web page.

## Features

- Downloads all `<img>` tags in a page
- Downloads all images set as `background-image` in CSS
- Zips all images into a ZIP file for download
- Allows choosing between downloading only images, only background images or both

## How to Use

1. Copy the Javascript code and paste it into your browser console on the desired page
2. Execute the function `downloadImagesOrBackgroundImagesOrBoth()`
3. Choose between downloading img, background-images or both
4. A ZIP file called `downloaded_images.zip` will be generated with all images

## Considerations

- Images are named with a prefix `image_` or `background_image_` and a timestamp
- After downloading background images, a `data-downloaded` attribute is added to not download the same image again
- The code relies on the JSZip library to create the zip file with the images
- It was base64 encoded and decoded at runtime to facilitate executing in the console

## Credits

This code uses the [JSZip](https://stuk.github.io/jszip/) library to zip the images.

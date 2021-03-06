# Training Data Filtering
This is a GUI tool for manually filtering out images from [Matting Human Datasets](https://www.kaggle.com/laurentmih/aisegmentcom-matting-human-datasets). Results are saved to a local .csv file, and the progress will resume from where was left out last time.

Even though the dataset provides a large amount of images (34427), the quality of matting for most images are not very good, e.g. missing body parts, and scattered alpha values, which might suffocate the performance of a trained model. This tool aids user to mark down the good ones, and only use those for training purpose.
<p>
<img src="/screenshots/good_matting.png" width="40%" height="40%" />
<img src="/screenshots/bad_matting.png" width="40%" height="40%" />
</p>


# Usage
- Right arrow: Mark current image as 'bad', and move on to the next image.
- Left arrow: Go back to the previous image.
- Up arrow: Mark current image as 'good'.
- Down arrow: Mark current image as 'bad'.
- Esc: save and exit.

Each session the program will start from where was left out last time, and save the work when it exits. It also prints out the number of acculumated good images so far, so feel free to stop if you get enough images for training.

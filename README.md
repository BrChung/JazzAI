# JazzAI

Create jazz music with the power of AI

## Requirements

Install Python Dependencies

```
pip install -r requirements.txt
```

Install [FFmpeg](https://ffmpeg.org/)

On MacOS
```
brew install ffmpeg
```

## Train the Model

Use the Jupiter Notebook `trainer.ipynb` to begin train your model! The program will read midi files directly from a directory `default - midi/*.mid` and preprocess them into `notes.pkl`.

JazzAI uses TensorFlow and Keras to train the model and will save the best weights following every epoch.

## Generating the Jazz

Use the python script `generate.py` to generate a midi file from a trained weight. The program will ask for a weight file, enter the relative path to the weight file and the script will generate a `output.mid` file for you to listen to.

## Generating Video Animation

Use the python script `animate.py` to generate an mp4 from a midi file. Settings for the video output are found in `options.cfg`.

## References
Dataset:
https://bushgrafts.com/midi/

Git Repositories:
https://github.com/fatemetkl/music-generator-Tensorflow-
https://github.com/Conchylicultor/MusicGenerator
https://github.com/Simeonedef/music_gen_deep_learning
https://github.com/MajorThird/quick-midi-animation

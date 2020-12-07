# JazzAI

Create jazz music with the power of AI
Training Data From: https://bushgrafts.com/

## Requirements

Install Python Dependencies

```
pip install -r requirements.txt
pip install git+https://github.com/vishnubob/python-midi.git#egg=midi
```

Install FFmpeg

On MacOS
```
brew install ffmpeg
```

## Train the Model

Use the Jupiter Notebook `trainer.ipynb` to begin train your model! The program will read midi files directly from a directory `default - midi/*.mid` and preprocess them into `notes.pkl`.

JazzAI uses TensorFlow and Keras to train the model and will save the best weights following every epoch.

## Generating the Jazz

Use the python script `generate.py` to generate a mid file from a trained weight. The program will ask for a weight file, enter the relative path to the weight file and the script will generate a `output.mid` file for you to listen to.

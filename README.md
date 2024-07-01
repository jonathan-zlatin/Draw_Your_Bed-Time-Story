# Magical Drawing Adventure

![Game-start](project/src/assets/gameImg.png)

## Description
Magical Drawing Adventure is an interactive drawing application designed for children aged 4-8. This enchanting app combines the fun of drawing with the magic of AI-generated storytelling. Users draw three magical objects, which are then recognized by a machine learning model and incorporated into a unique, personalized fairy tale.

## Features
- Interactive drawing canvas with a magical theme
- AI-powered drawing recognition for 15 magical objects
- GPT-powered story generation based on the user's drawings
- Text-to-speech functionality for story narration
- Engaging user interface with sound effects and animations

## Technologies Used
- Python 3.9+
- PyQt5 for the graphical user interface
- TensorFlow for the machine learning model
- OpenAI GPT for story generation
- OpenCV for image processing

## Installation
1. Clone the repository:

git clone https://github.com/yourusername/magical-drawing-adventure.git

2. Navigate to the project directory:

cd Draw_Your_Bed_Time_Story

3. Install the required dependencies:

pip install -r requirements.txt

4. Set up your OpenAI API key in api_key.py:

API_KEY = "your_openai_api_key_here"

## Usage

Run the main application:
python QuickDrawApp.py

Draw a magical object on the canvas.
Click "Next Spell" to process your drawing.
Repeat steps 2-3 two more times.
Enjoy your personalized magical story!

## Model Training
To train the drawing recognition model:

Go to https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/simplified;tab=objects?prefix=&forceOnObjectsSortingFiltering=false
and download the labels you want to train on (npy ver.)

Ensure your QuickDraw dataset is in the data/ directory.
Run the training script:

pythons QD_loadData.py
python QD_trainer.py

## Project Structure

QuickDrawApp.py: Main application file
LoadData.py: Data loading and preprocessing
QD_trainer.py: Model training script
models/: Directory for saved models
data/: Directory for QuickDraw dataset
api_key.py: Configuration file for OpenAI API key

Contributing
Contributions to improve Magical Drawing Adventure are welcome! Please feel free to submit a Pull Request.

Google QuickDraw for the dataset
OpenAI for the GPT API
The PyQt and TensorFlow communities for their excellent tools and documentation

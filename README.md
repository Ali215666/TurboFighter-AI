# TurboFighter AI

AI-powered Street Fighter II Turbo bot that learns controller behavior from gameplay data and predicts button inputs in real time.

## Project Overview

This project combines emulator game-state data with supervised learning:

1. Gameplay states are recorded in GameState.csv.
2. A neural network is trained using trainingcode.py.
3. The trained model is saved as game_model.h5.
4. During live play, bot.py loads the model and predicts button actions for Player 1.

## Repository Contents

- bot.py: Real-time bot inference logic.
- trainingcode.py: Data preprocessing, model training, and evaluation.
- GameState.csv: Recorded gameplay state/action dataset.
- game_model.h5: Trained TensorFlow model used by the bot.

## Requirements

- Python 3.10 (recommended for TensorFlow compatibility)
- BizHawk emulator
- Street Fighter II Turbo ROM

## Python Dependencies

Install dependencies with:

pip install pandas matplotlib numpy tensorflow scikit-learn keyboard

## How Training Works

trainingcode.py performs data cleaning, normalization, model training, evaluation, and saves game_model.h5.

Run training:

python trainingcode.py

## How to Run the Bot

1. Open BizHawk (EmuHawk.exe).
2. Load the Street Fighter II Turbo ROM.
3. Open Tools -> Tool Box.
4. Start your Python integration that instantiates Bot from bot.py.
5. Activate the bot from the BizHawk tooling UI.

## Gameplay Screenshots

Screenshots section prepared; images will be referenced in the next documentation update.

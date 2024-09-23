# BERT Sentiment Analyzer

This project is a web application that performs sentiment analysis using a pre-trained BERT model. The frontend is built with React and Vite, while the backend is powered by Flask. The application allows users to input text and receive sentiment analysis results indicating whether the text is negative, neutral, or positive.

## Prerequisites

- Node.js and npm installed
- Python 3.x installed
- pip (Python package installer) installed

## Setup and Installation

### Backend

1. Navigate to the [`backend`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FWeb%20Development%2FProjects%2FBERT%20Testing%2Fbackend%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%2208853fac-bf0d-47a7-a12a-e5fecfabbf59%22%5D "d:\Web Development\Projects\BERT Testing\backend") directory:

    ```sh
    cd backend
    ```

2. Install the required Python packages:

    ```sh
    pip install -r requirements.txt
    ```

3. Run the Flask server:

    ```sh
    python server.py
    ```

### Frontend

1. Navigate to the [`frontend`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FWeb%20Development%2FProjects%2FBERT%20Testing%2Ffrontend%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%2208853fac-bf0d-47a7-a12a-e5fecfabbf59%22%5D "d:\Web Development\Projects\BERT Testing\frontend") directory:

    ```sh
    cd frontend
    ```

2. Install the required npm packages:

    ```sh
    npm install
    ```

3. Start the development server:

    ```sh
    npm run dev
    ```

## Usage

1. Open your web browser and navigate to the IP shown in the CLI.
2. Enter text into the input field and submit it to receive sentiment analysis results.

## Running with GPU

If you want to run the backend using GPU for faster performance, make sure that the CUDA toolkit is installed on your machine. You can follow the instructions at [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) to install it.

After installing the CUDA toolkit, you need to install the appropriate version of PyTorch that supports CUDA. Visit [PyTorch Get Started](https://pytorch.org/get-started/locally/) and follow the instructions to install PyTorch with CUDA support.

You should uninstall the regular version of torch before installing the GPU version to avoid any conflicts:

```sh
pip uninstall torch
```

## Project Details

- **Backend**: The backend is implemented using Flask. It loads a pre-trained BERT model for sentiment analysis and provides an API endpoint to analyze the sentiment of the input text.
- **Frontend**: The frontend is built with React, Vite, and Tailwind CSS. It provides a user interface for inputting text and displaying sentiment analysis results.
- **Model**: The sentiment analysis model used is `cardiffnlp/twitter-roberta-base-sentiment`, a RoBERTa model fine-tuned on Twitter data for sentiment classification.

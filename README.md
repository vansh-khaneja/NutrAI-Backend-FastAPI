# NutrAI Searcher - AI that reveals a product's nutrients with a single photo click
This repository guides to develop a Multimodal FastAPI application that leverages the [CLIP](https://openai.com/index/clip/) model for analyzing ```images``` or ```text```. The app performs semantic search to identify and retrieve nutritional information by querying a vector database, making it a powerful tool for multimodal data processing. Theis fastapi app is connected with web frontend-end written in Next.js for a better user interaction.

![Alt Text - description of the image](https://github.com/vansh-khaneja/NutrAI-Searcher-FastAPI/blob/main/sample.png?raw=true)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Execution](#execution)
- [Contributions](#contributions)

## Introduction

In this project, we used OpenAI ```CLIP``` model to create images embeddings and compare them with the already created text embeddings present in the Qdrant database and give the respective nutirents. The [FastAPI](https://fastapi.tiangolo.com/) model takes the image file as request and after processing give the nutrients as the response.

## Features

- Fast and efficient 
- Best for Diet freaks 
- Text and Image multimodal searching
- Easily intgrable with frontend with FastAPI

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/vansh-khaneja/NutrAI-Searcher-FastAPI
    cd NutrAI-Searcher-FastAPI
    ```

2. Set up the Python environment and install dependencies:

    ```sh
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. Set up Qdrant:

    Login to [Qdrant Cloud](https://cloud.qdrant.io/) to get the api_key and url.
   
   ```sh
    qdrant_client = QdrantClient(
    url="https://xxxxxx-xxxxx-xxxxx-xxxx-xxxxxxxxx.us-east.aws.cloud.qdrant.io:6333",
    api_key="<your-api-key>",
    )
    ```


4. Execute the ```main.py``` file by running this command in terminal.

```sh
    python main.py
```

## Execution
1.Create a .env file and create a variable ```OPENAI_API_KEY``` storing your API key.


2.Download the dataset for this project [here](https://run.unl.pt/bitstream/10362/135618/1/TEGI0570.pdf) or you can try with your own dataset. Just change the path of the PDF here.



3.Execute the ```main.py``` file by running this command in terminal.

```sh
    python main.py
```

## Contribution


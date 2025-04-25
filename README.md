# Animated-Image Generator Tool

This project is a **Streamlit application** that allows users to generate images in a **comic book style** using the **Stable Diffusion** model. The app takes a user-provided description, enhances it with comic book style prompts, and generates an image using the Stable Diffusion model.

## Features
- **Text-to-Image** generation in **comic book style**.
- Utilizes **Stable Diffusion** via Hugging Face's `diffusers` library.
- Deployed with **Streamlit** for easy web-based interaction.
- Supports both **CUDA** (for GPU acceleration) and **CPU** inference (however execution on CPU is very slow).
  
## Prerequisites

Ensure you have the following installed:
- Python 3.7 or later
- `pip` for package management

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com//Gauravendra-Chaudhary/AIGT.git
    cd stable-diffusion-assignment
    ```

2. **Install required Python libraries**:
    ```bash
    pip install -r requirements.txt
    ```

3. **(Optional) Set up GPU**: 
   If you have a GPU available, ensure that **CUDA** is properly installed to take advantage of faster image generation.

## Running the Application

1. **Run the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

2. **Enter a description**: The application will prompt you to enter a description for the image. For example:
    ```
    A superhero flying through the sky
    ```

3. **Generate the image**: Once you click the "Generate Image" button, the app will process your input and display a comic book-style image.

## Files

- **`app.py`**: Contains the core Streamlit application logic and the function to generate images using Stable Diffusion. This includes:
    - Text input for user description
    - Image generation function that loads the Stable Diffusion model from `diffusers` and applies a comic book style to the generated images.
  
- **`requirements.txt`**: Lists all the dependencies required for this project, including:
    - `torch` for deep learning model operations
    - `diffusers` for accessing pre-trained Stable Diffusion models
    - `streamlit` for building and deploying the web app
    - `Pillow` for image handling

- **`deploy_streamlit_app_on_google_colab_ngrok.ipynb`**: A Jupyter notebook that provides a tutorial on how to deploy the Streamlit app on Google Colab using **ngrok** for tunneling. This is useful if you want to run the application on Colab and share it easily.

## Usage Example

Here’s a basic usage of the application:

1. Run the app using `streamlit run app.py`.
2. Input the prompt: `A robot fighting a dragon`.
3. Wait while the image is generated.
4. View the final image in the app interface.

## Deployment

You can deploy this app in various ways:
- **Locally**: By running the command `streamlit run app.py`.
- **On Google Colab**: By following the steps in `deploy_streamlit_app_on_google_colab_ngrok.ipynb` to run the app on Google Colab with ngrok tunneling.

### Thank you !!

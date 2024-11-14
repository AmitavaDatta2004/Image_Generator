Here's a README for your project:

---

# Image Generation App

This project is a web application that leverages OpenAI's image generation API to create AI-generated images based on user prompts. The application is built with Flask and allows users to input a prompt and receive generated images in response.

## Features
- Simple web interface to enter prompts for image generation.
- Generates 5 AI-generated images (256x256 pixels) based on the input prompt.
- Uses OpenAI API for generating images.
- JSON response with image data for easy integration and handling.

## Prerequisites
1. Python 3.x
2. Flask
3. OpenAI API Key
4. dotenv

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/AmitavaDatta2004/Image_Generator.git
   ```

2. **Install Dependencies**
   Install the necessary Python packages:
   ```bash
   pip install flask openai python-dotenv
   ```

3. **API Key Setup**
   Create a `.env` file in the project directory and add your OpenAI API key:
   ```plaintext
   OPENAI_API_KEY=your_openai_api_key
   ```

## Usage

1. **Run the Application**
   Start the Flask app by running:
   ```bash
   python app.py
   ```

2. **Access the Web Interface**
   Open your browser and navigate to:
   ```
   http://0.0.0.0:8080
   ```

3. **Generate Images**
   - Use the input field on the homepage to enter a prompt for generating images.
   - The app will return 5 images in a JSON format for you to view.

## API Endpoints

- **`GET /generateimages/<prompt>`**  
  Generates images based on the specified prompt.

  **Request Parameters:**
  - `prompt`: The text prompt to generate images from.

  **Response:**
  - JSON with generated image data.

## File Structure

```
.
├── app.py               # Main Flask application
├── .env                 # Environment variables (API Key)
├── requirements.txt     # Project dependencies
└── templates
    └── index.html       # HTML file for the web interface
```

## License
This project is licensed under the MIT License.

---

### Notes
Make sure to replace `your_openai_api_key` in the `.env` file with your actual OpenAI API key before running the app.
AI-image-prediction
An AI Image Prediction API is an intelligent software interface that uses Artificial Intelligence (AI) and Machine Learning, espFlux Dev Image Generator A modern, beautiful web application for generating AI images using the Flux Dev model via HuggingFace Inference API.

Features ✨ Clean, modern UI with gradient design 🎨 Real-time image generation using Flux Dev model ⚡ No local GPU required - uses HuggingFace's free inference API 📱 Fully responsive design 🎯 Customizable parameters (width, height, steps) 💾 Download generated images 🔄 Settings persistence with localStorageecially Deep Learning, to identify, classify, and predict information from images automatically. This API acts as a bridge between a trained AI model and external applications such as websites, mobile apps

Setup Instructions:

Install Dependencies pip install flask flask-cors requests python-dotenv
Get HuggingFace Token Go to HuggingFace Settings Create a new access token (with "read" access) Copy your token
Configure Environment Create a .env file in the project root:
HF_TOKEN=your_huggingface_token_here 4. Run the Application python app.py The server will start at: http://localhost:5000

Usage Open your browser and navigate to http://localhost:5000 Enter a detailed prompt describing the image you want Adjust parameters if needed: Width/Height: Image dimensions (256-2048px) Steps: Number of inference steps (1-50, higher = better quality but slower) Click "Generate Image" Wait for the AI to create your image Download or create a new image! Example Prompts "A futuristic cityscape at sunset with flying cars, neon lights reflecting on wet streets, cyberpunk style" "A serene mountain landscape with a crystal clear lake reflection, autumn colors, golden hour" "A magical forest with glowing mushrooms and fireflies at night, fantasy art style" "An astronaut exploring a colorful alien planet with multiple moons in the sky" Technologies Used Backend: Flask (Python) Frontend: Vanilla JavaScript, HTML5, CSS3 AI Model: FLUX.1-dev by Black Forest Labs API: HuggingFace Inference API Icons: Font Awesome 6.5 Fonts: Google Fonts (Inter) API Endpoints GET / - Serve the main application POST /generate - Generate image from prompt GET /health - Health check endpoint

Notes: First generation may take longer as the model loads on HuggingFace servers The free tier has rate limits - wait a few seconds between requests if needed For faster generation, consider using a paid HuggingFace plan or running locally with GPU Troubleshooting Model loading error: Wait 20-30 seconds and try again Token error: Make sure your HF_TOKEN is valid and has model access Timeout: Reduce the number of steps or image dimensions CORS errors: Make sure flask-cors is installed

License: MIT License - Feel free to use and modify for your projects!

CREDITS: Flux Dev Model: Black Forest Labs UI Design: Custom modern gradient design Icons: Font Awesome

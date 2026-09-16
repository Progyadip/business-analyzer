# VentureScan

AI-powered business idea and market analysis with Flask and Gemini.

## Run locally

1. Create a virtual environment and install dependencies:

	```bash
	python -m venv .venv
	source .venv/bin/activate
	pip install -r requirements.txt
	```

2. Create a `.env` file and add your Gemini API key:

	```text
	GEMINI_API_KEY=your-key-here
	```

3. Start the app:

	```bash
	python app.py
	```

Open `http://localhost:5000` in your browser.

## Deploy for free

The app is ready for a free public [Hugging Face Space](https://huggingface.co/spaces):

1. Create a new Space and choose **Docker** with the free CPU hardware.
2. Copy the files from this repository into the Space, or import this GitHub repository if that option is available.
3. In the Space settings, add a secret named `GEMINI_API_KEY`.
4. Wait for the Docker build to finish. The Space URL is the public website.

The Docker image listens on port `7860`, and the API key remains server-side in the Space secret. Do not commit `.env` or an API key.
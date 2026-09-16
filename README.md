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

## Deploy publicly

This repository includes a `render.yaml` blueprint for deployment on Render:

1. Sign in to [Render](https://render.com) and choose **New > Blueprint**.
2. Connect the `Progyadip/business-analyzer` GitHub repository.
3. Deploy the blueprint.
4. In the Render service settings, set the private `GEMINI_API_KEY` environment variable.

Render will build and start the Flask app automatically. The public URL will be shown on the service page, and future pushes to `main` will redeploy it.
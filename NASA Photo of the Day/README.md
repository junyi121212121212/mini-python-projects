# NASA Photo of the Day

Explore the cosmos with NASA's Astronomy Picture of the Day! This interactive tool lets you select any date and view stunning astronomical images with detailed explanations, plus audio narration powered by text-to-speech.

## Features

- Browse NASA's Astronomy Picture of the Day by selecting any date
- View high-quality astronomical images and videos
- Read detailed scientific explanations for each image
- Listen to audio narration of the descriptions using Google Text-to-Speech
- Automatic image downloading and local storage
- Interactive date selection interface

## Requirements

- Python 3.x
- Jupyter Notebook
- NASA API key (free - takes about 2 minutes to get!)

Install dependencies:
```bash
pip install nasapy gtts playsound python-dotenv
```

## Setup

### Getting Your NASA API Key (2 minutes)

1. Visit the [NASA API website](https://api.nasa.gov/)
2. Click "Get Started" or "Generate API Key"
3. Fill out the simple form with your name and email
4. You'll receive your API key instantly!
5. Copy your API key and paste it in the `.env` file:
   ```
   NASA_API_KEY=your_api_key_here
   ```

That's it! No waiting, no approval process - just instant access to NASA's amazing data.

## Usage

1. Make sure you've added your NASA API key to the `.env` file
2. Open `NASA_photo_of_the_day.ipynb` in Jupyter Notebook
3. Run the notebook cells to start the application
4. Select a date to view that day's astronomical image
5. Type `a` to hear the audio explanation of the image

## How It Works

The tool connects to NASA's APOD (Astronomy Picture of the Day) API to fetch:
- High-resolution images or videos
- Scientific titles and descriptions
- Copyright and credit information
- Publication dates

Images are automatically saved to the `Astro_Images` folder, and audio explanations are generated using Google's Text-to-Speech service.

---

Discover the universe one day at a time!

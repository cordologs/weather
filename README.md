# Weather Dashboard

A real-time weather dashboard for Ambient Weather WS-2902 weather stations. This web application displays live weather sensor data and historical charts using the Ambient Weather API.

## Prerequisites

You need an Ambient Weather station and API access:

1. **Weather Station**: Compatible Ambient Weather station (WS-2902, etc.)
2. **Ambient Weather Account**: Register at [ambientweather.net](https://ambientweather.net)
3. **API Credentials**: Obtain API and Application keys from your account

## Getting API Credentials

1. Log into your Ambient Weather account at [ambientweather.net](https://ambientweather.net)
2. Go to **Account** → **API Keys**
3. Generate a new **API Key** and **Application Key**
4. Note your weather station's **MAC address** from your device list

## Quick Start

### Option 1: Use URL Parameters (Easiest)

Access the dashboard directly with your credentials in the URL:

```
https://yourusername.github.io/weather/?apiKey=YOUR_API_KEY&appKey=YOUR_APP_KEY&mac=YOUR_MAC_ADDRESS
```

### Option 2: Use Login Form

1. Visit the dashboard URL
2. Enter your credentials in the login form:
   - **API Key**: Your Ambient Weather API key
   - **Application Key**: Your Ambient Weather application key
   - **Device MAC Address**: Your weather station's MAC address (format: XX:XX:XX:XX:XX:XX)

## GitHub Pages Deployment

### 1. Fork or Clone This Repository

```bash
git clone https://github.com/yourusername/weather.git
cd weather
```

### 2. Push to Your GitHub Repository

```bash
git remote set-url origin https://github.com/yourusername/weather.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

Your dashboard will be available at: `https://yourusername.github.io/weather/`

## Local Development

Since this is a client-side application with CDN dependencies, no build process is required:

```bash
# Simply open the file in a browser
open index.html

# Or serve with a local server
python -m http.server 8000
# Then visit http://localhost:8000
```

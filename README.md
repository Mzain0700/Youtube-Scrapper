
# YouTube Scraper

This YouTube scraper is a Python-based tool designed to fetch data about videos from specific YouTube channels using the YouTube Data API. It retrieves details like video titles, descriptions, publish dates, view counts, and more, organizing the information into a structured format.

## Features

- **Channel Video Information:** Fetches a list of videos from a specified YouTube channel.
- **Video Details:** Retrieves metadata such as video title, description, publish date, and view count.
- **Data Export:** Saves the collected data to a CSV file for easy analysis.
- **Comments scrap:** Also scrapp comment from videos scrapp above in csv form.

## Requirements

- Python 3.6+
- YouTube Data API key

## Libraries Used

- `googleapiclient.discovery`: Used to interact with the YouTube Data API.
- `pandas`: For data handling and manipulation.
- `csv`: For exporting the data to CSV files.

## Setup

1. **Clone or download the repository:**

   ```bash
   git clone https://github.com/yourusername/youtube-scraper.git
   cd youtube-scraper
   ```

2. **Install the required Python libraries:**

   Install the required libraries using pip:
   ```bash
   pip install google-api-python-client pandas
   ```

3. **Obtain a YouTube Data API Key:**

   - Go to the [Google Cloud Console](https://console.cloud.google.com/).
   - Create a new project (if you don't have one already).
   - Enable the "YouTube Data API v3" for your project.
   - Create an API key in the credentials section and save it.

4. **Set up the API Key in the code:**

   In the code, you will see a placeholder for the API key:
   ```python
   api_service_name = "youtube"
   api_version = "v3"
   DEVELOPER_KEY = "YOUR_API_KEY_HERE"
   ```

   Replace `YOUR_API_KEY_HERE` with the API key you generated from the Google Cloud Console.

   or Simply Save api in variable created in code "api_key"

## Usage

1. **Running the Notebook:**

   Open the Jupyter notebook `Youtube_scrapper.ipynb` and run the cells step-by-step. Make sure you start by setting up the API key and the service client.

2. **Fetching Channel Video Data:**

   The notebook includes a function to retrieve video details from a specified YouTube channel. To specify the channel, update the variable in the code:
   ```python
   channel_name = "Your_Channel_name"
   ```

3. **Saving Data to CSV:**

   The video data retrieved will be saved automatically to a CSV file named `Youtube_name.csv`. You can modify the filename in the code if required.

## Output

The output of this scraper includes:
- **Video Title**
- **Video Description**
- **Published Date**
- **View Count**

The data is organized and saved in a CSV file format for easy analysis and further processing.

## Limitations

- **API Quota:** Be aware of the quota limitations imposed by the YouTube Data API. Excessive requests may lead to quota exhaustion.
- **Data Accuracy:** Data fetched is dependent on the information available via the YouTube API and may vary over time.

## Troubleshooting

- **Quota Exceeded:** If you receive an error related to quota limits, you may need to reduce the frequency of your requests or request a higher quota from Google.
- **Invalid API Key:** Ensure that the API key is correct and that you have enabled the YouTube Data API v3.

## Contributing

If you'd like to contribute to the project, please fork the repository and use a feature branch. Pull requests are warmly welcome.


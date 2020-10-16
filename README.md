# Google Personal Data
***
Want to explore the data associated with your Google account?

Google has a data export tool. But the data is housed inside HTML files. This project:
- Converts your Search history into a CSV for your own EDA, model building, and miscellaneous use.
- Clusters your Google Searches into a specified number of topics and the words that comprise each

## Instructions:
1. Visit [Google Takeout](https://takeout.google.com/), and request a copy of your data
2. Install required libraries
3. Change `path` to your Google HTML file
4. Change `OUTPUT_FILE` to your desired CSV name
5. Run

## Features Generated From Google Data
- Log type 
- Query (raw)
- Date
- URL
- Location (coordinates)
- Day
- Desktop/Mobile
- Site
- Location (address)
- Query (cleaned for topic modeling)

\* Note: Only searches have location data

## What
- `ProcessGoogleData` class: creates the CSV from Google's HTML
- `GenerateFeatures` class: builds additional useful features
- `ModelData` class: creates topic NMF or LDA topic models from the Google Search queries*

\* Only tested on Google search since I rarely use the others.

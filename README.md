# Osmose per Country 

This is a front end interface that allows fetching data on gaps in the OSM data through the OSMOSE API on a country level.
Visit the website [here](https://open-energy-transition.github.io/osmose_per_country/): 

## How It Works

1. **Input Parameters:**  
   Fill out the form with the following:
   - **Country:** The name of the country for which data is to be retrieved. Some states and province names are also supported. A list of all supported regions can be found in the [Osmose Countries API](https://osmose.openstreetmap.fr/api/0.3/countries). To get all regions from a country at once, you can use a wildcard character (\*). For example, nigeria\* will give you all regions of Nigeria.
   - **Issue Type (item):** The specific issue type code.
   - **Class:** The classification code for the issues.

2. **Data Fetching:**  
   When the form is submitted, JavaScript constructs an API URL and fetches data from the Osmose API. The fetched data is filtered and converted into a GeoJSON FeatureCollection. Once data is processed, the app automatically downloads the file named using the country parameter.

## Installation

1. **Clone or Download the Repository:**
   ```bash
   git clone https://github.com/yourusername/osmose-api-data-fetcher.git
   ```
2. Ensure the repository includes:
   - `index.html`
   - `styles.css`
   - `logo.png` 

3. **Run Locally:**  
   Open `index.html` in your browser to test the application.

## Useful Links

- [Osmose API Documentation](https://wiki.openstreetmap.org/wiki/Osmose/api/0.3)
- [Osmose Countries API](https://osmose.openstreetmap.fr/api/0.3/countries)
- [Osmose Issue Types Documentation](https://wiki.openstreetmap.org/wiki/Osmose/issues)

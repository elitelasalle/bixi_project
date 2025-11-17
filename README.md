# BIXI Station Finder

Web app project for finding BIXI bike stations in Montreal and checking live availability.

## Team
**Elite Team** - LaSalle College Montreal  
Professor: Mohamed Zeroug

## Project Goal
Build a simple web application where users can search for BIXI stations by name and view:
- Station location on an interactive map
- Real-time bike availability
- Number of available docks
- Last update timestamp

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript
- **Map Library**: Leaflet.js
- **Map Tiles**: MapTiler (OpenStreetMap)
- **Data Source**: BIXI Open Data API (GBFS format)

## APIs Used
The app fetches data from BIXI's public feeds:
- `station_information.json` - Station names, locations, capacity
- `station_status.json` - Live bike/dock availability
- `vehicle_types.json` - Bike types (optional)

API endpoints are documented in `BixiData.txt`

## How to Run
1. Clone the repo
2. Open `osm.html` in a browser, or run a local server:
   ```bash
   python3 -m http.server 8000
   ```
3. Navigate to `http://localhost:8000/osm.html`

## Current Status
- ✅ Basic map setup with Leaflet
- ✅ MapTiler API configured
- ✅  Station search functionality
- 🚧 Live data integration (in progress)
- 🚧 Station popup with availability info (in progress)

## Next Steps
- Add search input with autocomplete
- Fetch and combine BIXI API data
- Display searched station on map with live info
- Error handling and loading states

## Notes
- MapTiler API key is already configured in `osm.html`
- Each team member should work on their assigned part
- Test your changes before pushing to main

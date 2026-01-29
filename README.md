# Myanmar Earthquake Map (August 20-21, 2025)

An interactive web-based visualization of earthquake events that occurred in Myanmar on August 20-21, 2025. This project uses Leaflet.js to display earthquake locations, magnitudes, and affected regions on an interactive map.

## Overview

This project visualizes seismic activity in the Ayeyarwady Region of Myanmar, specifically two significant earthquake events that occurred in succession. The interactive map allows users to explore earthquake locations, view magnitude information, and understand the geographic context of these seismic events.

## Earthquake Events

The map displays the following earthquake events:

1. **Event 1 (August 20, 2025)**
   - **Magnitude:** 4.8
   - **Location:** Approximately 23 miles SE of Pyapon
   - **Coordinates:** 16.07°N, 95.94°E
   - **Marker Color:** Blue
   - **Depth Indicator:** Radius 14.4 units

2. **Event 2 (August 21, 2025)**
   - **Magnitude:** 5.1
   - **Location:** Approximately 28 miles SE of Kungyangon
   - **Coordinates:** 16.08°N, 96.22°E
   - **Marker Color:** Orange
   - **Depth Indicator:** Radius 15.3 units

## Features

- **Interactive Map:** Pan and zoom to explore the affected region
- **Color-Coded Markers:** 
  - Blue markers indicate magnitude 4.0-4.9 earthquakes
  - Orange markers indicate magnitude 5.0-5.9 earthquakes
- **Popup Information:** Click on any marker to view detailed information about the earthquake
- **Geographic Context:** Includes Myanmar's administrative boundaries (red outline)
- **OpenStreetMap Integration:** High-quality base map with detailed geographic features
- **Responsive Design:** Works on desktop and mobile devices

## Technology Stack

This project is built using the following technologies:

- **[Leaflet.js](https://leafletjs.com/) (v1.9.3):** JavaScript library for interactive maps
- **[jQuery](https://jquery.com/) (v3.7.1):** JavaScript library for DOM manipulation
- **[Bootstrap](https://getbootstrap.com/) (v5.2.2):** CSS framework for responsive design
- **[Leaflet.awesome-markers](https://github.com/lvoogdt/Leaflet.awesome-markers) (v2.0.2):** Plugin for custom map markers
- **[Font Awesome](https://fontawesome.com/) (v6.2.0):** Icon library
- **[OpenStreetMap](https://www.openstreetmap.org/):** Base map tile provider
- **[Folium](https://python-visualization.github.io/folium/):** Python library used to generate the map (likely used in data processing)

## Installation and Usage

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for loading external libraries and map tiles)

### Running the Map

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mrtinkooo/myanmar-quake-20250820-20250821.git
   cd myanmar-quake-20250820-20250821
   ```

2. **Open the map:**
   - Simply open `index.html` in your web browser
   - Or use a local web server:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Python 2
     python -m SimpleHTTPServer 8000
     
     # Node.js (with http-server package)
     npx http-server
     ```
   - Then navigate to `http://localhost:8000` in your browser

3. **Interact with the map:**
   - Click and drag to pan the map
   - Use the scroll wheel or +/- buttons to zoom in/out
   - Click on earthquake markers to view detailed information

## Data Sources

The earthquake data displayed in this visualization comes from seismological monitoring systems that track seismic activity in Southeast Asia. The data includes:

- Earthquake magnitude (Richter scale)
- Geographic coordinates (latitude/longitude)
- Approximate location descriptions (distance and direction from known cities)
- Event timestamps

## Map Configuration

The map is centered on Myanmar with the following default settings:

- **Center Point:** 16.075°N, 96.08°E
- **Initial Zoom Level:** 6
- **Coordinate Reference System:** EPSG:3857 (Web Mercator)
- **Tile Layer:** OpenStreetMap standard tiles
- **Max Zoom:** 19 levels
- **Attribution:** © OpenStreetMap contributors

## Color Coding System

The earthquake markers use a color-coding system based on magnitude:

- **Blue:** Magnitude 4.0 - 4.9 (Light to moderate earthquakes)
- **Orange:** Magnitude 5.0 - 5.9 (Moderate earthquakes)
- **Red:** Magnitude 6.0+ (Strong to major earthquakes) - Not present in this dataset

The marker size also scales with magnitude, providing a visual indicator of earthquake intensity.

## Browser Compatibility

This map is compatible with all modern web browsers that support:
- HTML5
- CSS3
- JavaScript ES5+
- SVG rendering

Tested browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Project Structure

```
myanmar-quake-20250820-20250821/
├── index.html          # Main HTML file with embedded map and data
├── README.md           # This documentation file
├── CONTRIBUTING.md     # Contribution guidelines
└── LICENSE             # MIT License and attributions
```

## Contributing

Contributions are welcome! If you'd like to improve this visualization or add additional earthquake data:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## Possible Enhancements

Future improvements could include:

- **Real-time Data:** Integration with live earthquake feeds
- **Historical Data:** Display of historical earthquake patterns
- **Timeline Control:** Slider to view earthquakes over time
- **Data Export:** Ability to download earthquake data in various formats
- **Statistics Panel:** Show aggregated statistics about the events
- **Mobile App:** Native mobile application for iOS and Android
- **Alert System:** Notification system for new earthquake events
- **Depth Visualization:** Better representation of earthquake depth
- **Magnitude Scale:** Visual scale/legend for earthquake magnitudes
- **Search Functionality:** Search for earthquakes by location or magnitude

## Safety Information

If you experience an earthquake:

1. **DROP:** Drop down onto your hands and knees
2. **COVER:** Cover your head and neck under a sturdy table or desk
3. **HOLD ON:** Hold on until shaking stops

For more earthquake safety information, visit your local disaster preparedness organization.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

The map data is provided by OpenStreetMap contributors under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/).

## Acknowledgments

- OpenStreetMap contributors for map tile data
- Leaflet.js community for the excellent mapping library
- Seismological monitoring organizations for earthquake data
- Bootstrap team for the responsive design framework

## Contact

For questions, issues, or suggestions, please open an issue on the [GitHub repository](https://github.com/mrtinkooo/myanmar-quake-20250820-20250821/issues).

## Disclaimer

This visualization is for informational and educational purposes only. For official earthquake information and emergency alerts, please consult:

- Myanmar Department of Meteorology and Hydrology
- USGS Earthquake Hazards Program
- Your local emergency management agency

**Note:** Always follow official guidance from local authorities during seismic events.
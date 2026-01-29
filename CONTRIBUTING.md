# Contributing to Myanmar Earthquake Map

Thank you for your interest in contributing to this project! This document provides guidelines and information for contributors.

## How to Contribute

We welcome contributions in several forms:

### 1. Reporting Issues

If you find a bug or have a suggestion:

1. Check the [issue tracker](https://github.com/mrtinkooo/myanmar-quake-20250820-20250821/issues) to see if it's already reported
2. If not, create a new issue with a clear description
3. Include:
   - Browser and version
   - Steps to reproduce (for bugs)
   - Expected vs. actual behavior
   - Screenshots if applicable

### 2. Suggesting Enhancements

We're always looking to improve! If you have ideas for new features:

1. Open an issue with the "enhancement" label
2. Describe the feature and its benefits
3. Provide examples or mockups if possible
4. Explain any technical considerations

### 3. Code Contributions

#### Getting Started

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/myanmar-quake-20250820-20250821.git
   cd myanmar-quake-20250820-20250821
   ```

3. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

#### Making Changes

1. **Code Style**
   - Use consistent indentation (4 spaces)
   - Follow existing code patterns
   - Add comments for complex logic
   - Keep functions small and focused

2. **Testing**
   - Test your changes in multiple browsers
   - Verify the map displays correctly
   - Check that markers and popups work
   - Ensure mobile responsiveness

3. **Documentation**
   - Update README.md if adding features
   - Add inline comments for new code
   - Update this CONTRIBUTING.md if needed

#### Submitting Changes

1. **Commit your changes**
   ```bash
   git add .
   git commit -m "Brief description of changes"
   ```

2. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

3. **Create a Pull Request**
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Select your fork and branch
   - Provide a clear description of changes
   - Reference any related issues

## Development Guidelines

### Project Structure

```
myanmar-quake-20250820-20250821/
├── index.html          # Main map visualization file
├── README.md           # Project documentation
└── CONTRIBUTING.md     # This file
```

### Adding Earthquake Data

If you're adding new earthquake events:

1. **Data Format**
   - Latitude and longitude (decimal degrees)
   - Magnitude (Richter scale)
   - Location description
   - Date/time of event

2. **Marker Colors**
   - Blue: Magnitude 4.0-4.9
   - Orange: Magnitude 5.0-5.9
   - Red: Magnitude 6.0+

3. **Code Pattern**
   ```javascript
   // Add earthquake marker
   var circle_marker = L.circleMarker(
       [latitude, longitude],
       {
           color: "color-based-on-magnitude",
           radius: scaled-radius,
           // ... other options
       }
   ).addTo(map);
   
   // Add popup with information
   var popup = L.popup({maxWidth: "100%"});
   var html = $(`<div>Magnitude: X.X<br>Region: Description</div>`)[0];
   popup.setContent(html);
   circle_marker.bindPopup(popup);
   ```

### Enhancing the Visualization

Ideas for improvements:

1. **Timeline Feature**
   - Add a slider to view events chronologically
   - Animate marker appearance

2. **Data Layers**
   - Toggle different types of seismic events
   - Show/hide specific magnitude ranges

3. **Statistics Panel**
   - Display summary statistics
   - Show frequency charts

4. **Export Functionality**
   - Allow data export to CSV/JSON
   - Generate printable reports

5. **Real-time Updates**
   - Connect to earthquake data APIs
   - Auto-refresh with new events

## Code of Conduct

### Our Standards

- Be respectful and inclusive
- Accept constructive criticism gracefully
- Focus on what's best for the community
- Show empathy towards others

### Unacceptable Behavior

- Harassment or discrimination
- Trolling or insulting comments
- Publishing others' private information
- Unprofessional conduct

### Enforcement

Violations may result in:
- Warning
- Temporary ban
- Permanent ban

Report issues to the repository maintainers.

## Questions?

If you have questions:

1. Check existing issues and documentation
2. Open a new issue with the "question" label
3. Provide context and what you've already tried

## Recognition

Contributors will be recognized in:
- Git commit history
- Release notes (for significant contributions)
- Project acknowledgments

Thank you for contributing to earthquake awareness and education!

## License

By contributing, you agree that your contributions will be licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Additional Resources

### Earthquake Data Sources

- [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/)
- [European-Mediterranean Seismological Centre](https://www.emsc-csem.org/)
- [Myanmar Department of Meteorology and Hydrology](http://www.dmh.gov.mm/)

### Technical Documentation

- [Leaflet.js Documentation](https://leafletjs.com/reference.html)
- [Leaflet Tutorial](https://leafletjs.com/examples.html)
- [GeoJSON Specification](https://geojson.org/)
- [Web Mercator Projection](https://en.wikipedia.org/wiki/Web_Mercator_projection)

### Testing Tools

- [Can I Use](https://caniuse.com/) - Browser compatibility
- [Chrome DevTools](https://developer.chrome.com/docs/devtools/) - Debugging
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) - Performance testing

---

**Last Updated:** January 2026

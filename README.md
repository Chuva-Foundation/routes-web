# Routes Web App Documentation

The `Routes Web` app is a React application that provides a graphical user interface for visualizing and interacting with bus route data on a map. The app utilizes the Mapbox API for map rendering and includes features for displaying bus routes, adding markers, calculating routes, and managing route visibility.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Components](#components)
- [Functions](#functions)
- [License](#license)

## Prerequisites
Before you begin, make sure you have the following:

- [Node.js](https://nodejs.org/) installed on your machine.
- A valid Mapbox API access token. You can obtain one by signing up at [Mapbox](https://www.mapbox.com/).

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/routes-web-app.git
   ```
2. Navigate to the project directory:
   ```sh
   cd routes-web-app
   ```
3. Install dependencies using npm:
   ```sh
   npm install
   ```
4. Replace `"YOUR_MAPBOX_ACCESS_TOKEN"` with your actual Mapbox API access token in the `App.js` file.

## Getting Started
To start the app, run the following command:
```sh
npm start
```

The app will be accessible at `http://localhost:3000` in your web browser.

## Usage
The `Routes Web` app provides the following features:

### 1. Display Bus Routes
- Click on individual route options to toggle the visibility of bus routes on the map.

### 2. Show All Routes
- Click the "Show All" button to display all available bus routes on the map.

### 3. Remove All Routes
- Click the "Remove All" button to remove all currently displayed bus routes from the map.

### 4. Calculate Route
- Click the "Calculate Route" button to calculate and display a route between two selected map points.

### 5. Add Markers
- Click on the map to add markers. A maximum of two markers can be added, which represent the origin and destination points for route calculation.

### 6. View Geoposition
- The current longitude, latitude, and zoom level are displayed in the sidebar.

## Components
The app consists of the following main components:

- `MapContainer`: Renders the map using the Mapbox API.
- `Options`: Displays options for toggling route visibility, showing all routes, and removing all routes.
- `App`: The main component that integrates the map, options, and functionalities.

## Functions
The app includes several functions for handling various functionalities:

- `handleVisibleLines()`: Adds visible bus routes to the map based on user selection.
- `showAll()`: Displays all available bus routes on the map.
- `show(id)`: Toggles the visibility of a specific bus route on the map.
- `calculateRoute()`: Calculates and displays a route between the selected origin and destination points.
- `remove(id)`: Removes a specific bus route from the map.
- `removeRoute()`: Removes the calculated route from the map.
- `removeAll()`: Removes all currently displayed bus routes from the map.
- `removeSubstring(originalString)`: Removes a specified substring from a string.

## License
This app is released under the MIT License. See the [LICENSE](/LICENSE) file for details.

---

This documentation provides an overview of the `Routes Web` app and its features. For detailed implementation and customization, please refer to the source code and comments in the `App.js` file. If you encounter any issues or need further assistance, please feel free to reach out to the project maintainers or the community.

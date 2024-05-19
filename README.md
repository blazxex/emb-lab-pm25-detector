# Air Pollution Dashboard

This website is part of the final project for the 2110366 Embedded Systems Lab in Computer Engineering at Chulalongkorn University. We utilize the WHO AQI guidelines as a reference for determining hazardous air quality levels. Please note that the data on this site may include mock data for educational purposes.

## Project Overview

This interface displays data collected from GPS, PM2.5, and CO2 sensors connected to an STM32-based NodeMCU. The data is transmitted via NETPIE for visualization here.

## Features

- **Real-Time Data Visualization**: Display real-time data from PM2.5 and CO2 sensors.
- **Location-Based Data**: Use GPS data to show location-specific air quality information.
- **WHO AQI Guidelines**: Reference WHO AQI guidelines to provide context on air quality levels.
- **Educational Mock Data**: Some data may be mocked for educational purposes.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/blazxex/emb-lab-pm25-detector
    cd emb-lab-pm25-detector
    cd project-frontend
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Create a `.env` file** in the `project-frontend` directory with the following environment variables:
    ```env
    VITE_NET_USER_TOKEN_KEY=your_netpie_key
    VITE_GEO_API=your_OpenCage_API_key
    VITE_GOOGLE_MAPS_API_KEY=your_gooogle_map_API_KEY
    ```

4. **Run the development server**:
    ```bash
    npm run dev
    ```

## Usage

### Location Data

Your location data will be used solely for displaying relevant data and will not be collected or stored on our servers.

### Transmitted Data

- **GPS**: Provides the geographical location for data relevance.
- **PM2.5**: Measures particulate matter in the air.
- **CO2**: Measures carbon dioxide levels in the air.

### Data Transmission

The data is transmitted via NETPIE, an IoT platform, to this Vue.js interface for visualization.

## Project Structure

- `src/`: Contains the source code for the Vue.js application.
  - `components/`: Vue components.
  - `assets/`: Static assets.
- `public/`: Public assets.
- `README.md`: Project documentation.

---

This project was developed as part of the 2110366 Embedded Systems Lab in Computer Engineering at Chulalongkorn University.

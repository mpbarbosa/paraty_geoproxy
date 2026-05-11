# paraty_geoproxy
A  geolocation proxy server developed in TypeScript and Node.js.
## Features
- **Geolocation Proxying**: Intercept and modify geolocation requests to provide custom location data.
- **Configurable Location Data**: Easily configure the location data that the proxy will return for geolocation requests.
- **Cross-Platform**: Runs on any platform that supports Node.js.
- **Lightweight**: Minimal dependencies and efficient performance.
- **Cache Support**: Optionally cache geolocation responses for improved performance.
- **Logging**: Detailed logging of geolocation requests and responses for debugging and monitoring purposes.
- **API Integration**: Integrate with external APIs to fetch real-time location data if needed.
- **Security**: Implement security measures to protect against unauthorized access and ensure data integrity.
- **Access the Geolocation Services**: Easily access and utilize the geolocation services provided by the proxy.
- **Supported Providers**: Main geolocation providers like Google Maps, OpenStreetMap, and Mapbox are supported.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/mpbarbosa/paraty_geoproxy.git
cd paraty_geoproxy
```

2. Install dependencies:

```bash
npm install
```

3. Build the project:

```bash
npm run build
```

4. Start the proxy server:

```bash
npm start
```
## Configuration
The proxy server can be configured using a `config.json` file located in the root directory. Here is an example configuration:
```json
{
  "port": 8080,
  "locationData": {
    "latitude": 37.7749,
    "longitude": -122.4194,
    "accuracy": 100
  },
  "cacheEnabled": true,
  "cacheDuration": 3600,
  "loggingEnabled": true,
  "externalApi": {
    "enabled": false,
    "url": "https://api.example.com/geolocation"
  }
}
```
- `port`: The port on which the proxy server will listen for requests.
- `locationData`: The custom location data that the proxy will return for geolocation requests.
- `cacheEnabled`: Enable or disable caching of geolocation responses.
- `cacheDuration`: The duration (in seconds) for which cached responses will be stored.
- `loggingEnabled`: Enable or disable logging of geolocation requests and responses.
- `externalApi`: Configuration for integrating with an external API to fetch real-time location data.       
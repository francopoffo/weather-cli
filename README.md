# Weather CLI App

This is a simple command-line interface (CLI) application that fetches and displays the weather forecast for a given location.

## Installation

1. Clone this repository:
   
```bash
git clone <repository_url>
```

2. Navigate to the project directory:
   
```bash
cd <project_directory>
```

3. Build the application:

```bash
go build
```

4. Set up your Weather API key:

   - Sign up on [WeatherAPI](https://www.weatherapi.com/) to get your API key.
   - Create a file named `.env` in the project directory.
   - Add your Weather API key to the `.env` file:

     ```env
     WEATHER_API_KEY=your_weather_api_key
     ```

## Usage

Run the application from the command line with the following command:

```bash
./weather-cli [location]
```

Replace `[location]` with the name of the location for which you want to check the weather. If no location is provided, the default location is set to "Blumenau".

Example:

```bash
./weather-cli London
```

## Dependencies

- `github.com/fatih/color`: For colorizing output.
- `github.com/joho/godotenv`: For loading environment variables from a `.env` file.

## Notes

- This application uses the WeatherAPI to fetch weather data.
- It displays the current weather condition and temperature, along with a forecast for the day.
- The forecast includes the temperature, chance of rain, and weather condition for each hour.
- Hours that have already passed are skipped.
- Output colors are used to highlight hours with a high chance of rain.

Feel free to modify and extend this application according to your needs!

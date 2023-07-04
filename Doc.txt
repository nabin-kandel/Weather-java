
# WeatherApp Documentation🤡

## Introduction💤💤💤
The WeatherApp is a Java application that allows users to retrieve the current temperature for a specified location using the OpenWeatherMap API. The application provides a simple graphical user interface (GUI) for entering the location and displaying the temperature information.

## Features🍀🍀🍀
- Enter a location to get the current temperature
- Display the temperature in Celsius along with the weather condition

## Prerequisites👻
Before running the WeatherApp, ensure that you have the following:
- Java Development Kit (JDK) installed on your system
- Internet connectivity to access the OpenWeatherMap API

## Installation🤖🤖🤖
To install and run the WeatherApp, follow these steps:

1. Download the WeatherApp.java source code file.
2. Open a command prompt or terminal and navigate to the directory containing the WeatherApp.java file.
3. Compile the source code by executing the following command:
   ```
   javac WeatherApp.java
   ```
4. Run the application using the following command:
   ```
   java WeatherApp
   ```

## User Interface🤩🤩🤩
Upon launching the WeatherApp, a GUI window will appear with the following elements:

- Location Label: A label indicating the "Location" field.
- Location Field: A text field where users can enter the desired location.
- Temperature Label: A label indicating the "Temperature" field.
- Temperature Field: A non-editable text field that displays the current temperature in Celsius.
- Get Weather Button: A button that triggers the retrieval of the weather information.

## Usage🛟🛥
To use the WeatherApp, follow these steps:

1. Launch the application by executing the `java WeatherApp` command.
2. Enter the desired location in the "Location" text field.
3. Click the "Get Weather" button to retrieve the current temperature for the specified location.
4. The temperature will be displayed in the "Temperature" field along with the weather condition.

## Implementation Details🧐🧐🧐🧐🧐
The WeatherApp utilizes the following key components:

- `JFrame`: The main window that contains the application's GUI elements.
- `JPanel`: A panel that holds the labels, text fields, and button.
- `JLabel`: Labels used to indicate the purpose of the text fields.
- `JTextField`: Text fields for entering the location and displaying the temperature.
- `JButton`: A button to trigger the retrieval of weather information.
- `ActionListener`: An event listener that handles the button click event.
- `HttpURLConnection`: A class for creating an HTTP connection to the OpenWeatherMap API.
- `InputStream`: A stream to read the response from the API.
- `SwingUtilities`: A utility class for invoking the GUI creation on the event dispatch thread.

The application follows the Model-View-Controller (MVC) pattern, where the `WeatherApp` class serves as the controller, handling user interactions, and coordinating with the model (API) and view (GUI).

To retrieve the weather information, the application performs the following steps:
1. Constructs the API URL with the specified location and API key.
2. Opens an HTTP connection to the API.
3. Retrieves the response from the API and extracts the temperature and weather condition.
4. Converts the temperature from Kelvin to Celsius.
5. Updates the GUI with the retrieved temperature and weather condition.

In case of an error during the retrieval process, an exception message will be displayed in a dialog box.

## Limitations🫣🫣🫣
- The WeatherApp relies on the availability and reliability of the OpenWeatherMap API. If the API is unreachable or returns unexpected data, the application's functionality may be affected.
- The application only displays the current temperature and weather condition. Additional features like hourly or extended forecasts are not implemented in this version.

## Conclusion🟢🟢
The WeatherApp is a simple Java application that allows users to get the current Weather condition.

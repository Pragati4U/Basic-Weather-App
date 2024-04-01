# Basic-Weather-App
The basic weather app implemented using Python and Tkinter is a simple graphical user interface (GUI) application that allows users to input a city name and retrieve the current weather information for that city. Here's a breakdown of its components and functionality:

GUI Setup: The app's GUI is created using Tkinter, a standard GUI toolkit for Python. The window size is set to 400x400 pixels, and the window is made non-resizable.

User Input Field: There's an entry widget where users can input the name of the city for which they want to check the weather.

Button: A button labeled "Check Weather" is provided for users to trigger the weather information retrieval process.

Weather Display Area: Below the button, a label "The Weather is:" is displayed, followed by a text widget where the weather information will be displayed.

Weather Retrieval Function: The showWeather() function is responsible for fetching the weather information from the OpenWeatherMap API based on the city name entered by the user. It constructs the API URL, sends a request using the requests module, and processes the JSON response to extract relevant weather data.

Time Formatting Function: The time_format_for_location() function converts the UTC timestamp to local time based on the timezone offset provided by the API response.

Error Handling: If the API request is successful (status code 200), the weather information is displayed in the text widget. If the city name is not found or there's an error in the API response, an appropriate error message is displayed.

API Key: The OpenWeatherMap API key is stored in the api_key variable. It's essential to replace this with your actual API key obtained from the OpenWeatherMap website.

Dependencies: The code utilizes the requests module for making HTTP requests to the API. If you haven't already installed it, you need to install it using pip.

Overall, this weather app provides a simple way for users to check the current weather for any city of their choice using a basic graphical interface. It serves as a starting point for more advanced weather apps with additional features like forecast display, unit conversion, and error handling improvements.

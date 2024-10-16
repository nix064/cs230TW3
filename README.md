CS230 Teamwork 3:

Andhika: Tester

Jack: Project Leader

Nic: Coder

Seamus: Reviewer


This assignment is to take weather_data.txt and format it for the user.

for the sample output the program must:
1. Ask the user if they would like to see temps in F or C
2. Print the formatted weather data
  ex. Oct 01, 2024 68.0°F, Cloudy
      ...
      Oct 30, 2024 69.0°F, Sunny
3. print a tempurature bar chart:
  ex.
Oct 01, 2024: Cloudy Temp: 68.0°F | XXXXXXXXXXXXX
Oct 02, 2024: Sunny Temp: 70.0°F  | XXXXXXXXXXXXXX
Oct 03, 2024: Rainy Temp: 65.0°F  | XXXXXXXXXXXXX
Oct 04, 2024: Sunny Temp: 72.0°F  | XXXXXXXXXXXXXX
Oct 05, 2024: Rainy Temp: 66.0°F  | XXXXXXXXXXXXX
Oct 06, 2024: Sunny Temp: 69.0°F  | XXXXXXXXXXXXX
Oct 07, 2024: Cloudy Temp: 67.0°F | XXXXXXXXXXXXX
Oct 08, 2024: Sunny Temp: 71.0°F  | XXXXXXXXXXXXXX
....
Oct 30, 2024: Sunny Temp: 69.0°F  | XXXXXXXXXXXXX
4. print available weather forecasts:
   ex. Available Weather Forecasts: Partly Cloudy, Rainy, Sunny, Cloudy
Enter a weather forecast to get statistics: partly cloudy
Number of days with Partly Cloudy weather: 2
Dates with this forecast:
- 2024-10-19
- 2024-10-23

5. Monthly Weather Summary:
ex. 
Highest Temperature: 72.0°F
Number of days with highest temperature: 4
Dates with highest temperature:
- 2024-10-04
- 2024-10-12
- 2024-10-20
- 2024-10-28
Average Precipitation: 0.11 inches


Notes:

read_weather_data:
Reads the data from weather_data.txt into an appropriate data structure. 
Hint: think list of lists or list of tuples.

get_temp_unit:
asks the user whether to display temperatures as F (Fahrenheit) or C (Celsius). 
User can enter F or C (upper or lower), and if the entry is invalid defaults to F.

Would you like to see temperatures in Fahrenheit (F) or Celsius (C)? c

simlulate_weather:
Displays the day, temperature, and condition, nicely formatted. (After you get it working, look 
up the datetime module and write a function format_date to format the date as MMM DD YYYY format.) 
Sample output:

Oct 01, 2024 20.0°C, Cloudy
Oct 02, 2024 21.1°C, Sunny
Oct 03, 2024 18.3°C, Rainy
Oct 04, 2024 22.2°C, Sunny

create_temperature_chart: 
Displays the formatted date, weather forecast, temperature, and a 
simulated bar chart composed of X’s, with one X for every 5 degrees. Here are some sample lines:

Temperature Bar Chart:
Oct 01, 2024: Cloudy Temp: 20.0°C | XXXX
Oct 02, 2024: Sunny Temp: 21.1°C | XXXX
Oct 03, 2024: Rainy Temp: 18.3°C | XXX

weather_forecast_stats: 
Determines the available weather forecast types from the data itself 
(do not hardcode this value), and then displays them. Asks the user to enter one of the weather 
forecast types (Cloudy, Sunny, etc.), and displays the number of days with this forecast and the 
dates (formatted as either MMM DD, YYYY or as below). Ignore upper/lower case of user input value.

Available Weather Forecasts: Rainy, Cloudy, Sunny, Partly Cloudy
Enter a weather forecast to get statistics: Cloudy
Number of days with Cloudy weather: 6
Dates with this forecast:
- 2024-10-01
- 2024-10-07
- 2024-10-11
- 2024-10-15
- 2024-10-20
- 2024-10-27

monthly_weather_summary: 
Displays the highest temperature, the number of days with that 
temperature, and the dates with that temperature. Displays the average precipitation.

Monthly Weather Summary:
Highest Temperature: 22.2°C
Number of days with highest temperature: 4
Dates with highest temperature:
- 2024-10-04
- 2024-10-12
- 2024-10-20
- 2024-10-28

Average Precipitation: 0.11 inches

ftoc( f_temp): 
Converts an F temperature to C.

format_date (d): 
Given a string representing a date, return a string formatting the date as MMM DD YYYY. 
For example, formatdate('10-01-2024') would return 'Oct 01 2024'
calculate_average_precipitation(weather_data) : returns the month’s average precipitation

Typing the Degree Symbol:

Typing the degree symbol (°) can vary depending on your operating system and keyboard.
· On Windows: Hold down the Alt key and type 0176 on the numeric keypad.
· On Windows: Open the Character Map application (charmap), find and select the degree symbol (°), click “Copy” 
and then paste it where you need it.
· On Mac: Using the Keyboard: Press Option + Shift + 8.





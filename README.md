## My-Weather-App
### Description
MyWeatherApp is a simple Java-based web application that retrieves real-time weather information for any city using the [OpenWeatherMap API](https://openweathermap.org/). It displays weather conditions such as temperature, humidity, wind speed, and the general weather condition.

---
### Demo video 


https://github.com/user-attachments/assets/6f58bc76-8aa9-4944-81f1-1ae3de7730c2


---

### Features
- Fetches current weather data using the OpenWeatherMap API.
- Displays temperature, humidity, wind speed, and weather conditions.
- User-friendly interface to input the city name.
- Provides real-time weather updates for cities around the world.

---

## Technology Stack
- **Java** (Jakarta EE 5.0)
- **JSP** for dynamic page rendering.
- **Servlets** for handling HTTP requests and API integration.
- **Gson** for parsing JSON data from the OpenWeatherMap API.
- **HTML/CSS** for the front-end design.

---

### Prerequisites
1. **Eclipse IDE** with Jakarta EE support.
2. **Java JDK 17+** (or any compatible version).
3. **Tomcat Server** for deployment.
4. **Maven** for dependency management (optional).
5. **OpenWeatherMap API Key** (Sign up [here](https://openweathermap.org/appid)).

### Steps to Run Locally:
1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/TusharTalmale/My-Weather-App.git
    ```

2. Import the project into Eclipse:
    - Open Eclipse, go to **File** > **Import** > **Maven** > **Existing Maven Projects**.
    - Browse to the project directory and click **Finish**.

3. Add necessary external JARs **Gson** if not using Maven.

4. Update your OpenWeatherMap API key in the servlet:
    ```java
    String apiKey = "your-api-key-here";
    ```

5. Deploy the project on a local Tomcat server and start the server.

6. Open a browser and go to:
    ```bash
    http://localhost:8080/MyWeatherApp/
    ```

---

## How It Works
1. The user inputs a city name in the search box.
2. The app sends a POST request to the backend servlet.
3. The servlet calls the OpenWeatherMap API using the provided city name.
4. The API returns weather data in JSON format, which is parsed using **Gson**.
5. The parsed data is displayed on the webpage, showing temperature, humidity, wind speed, and weather condition.

---
### Dependencies
If using Maven, add the following dependencies to your pom.xml:

xml
```
<dependencies>
    <!-- Gson for JSON parsing -->
    <dependency>
        <groupId>com.google.code.gson</groupId>
        <artifactId>gson</artifactId>
        <version>2.8.5</version>
    </dependency>
</dependencies>
```
---
### Author
##### Tushar Talmale - https://github.com/TusharTalmale

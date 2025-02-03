Title: Currency Converter
Description: A Spring Boot application that integrates with a public API to provide real-time currency conversion functionality.
Features: -Fetch the exchange rates for the given base currency. 
          -Convert an amount from one currency to another using the fetched exchange rates.
Technologies Used: -Java 17
                   -Spring Boot
                   -Maven
                   -IDE(preffered Eclipse)
Requirement: -java 17
             -Maven 3.9.9
Installation: -Clone the repository -  bash
                                       git clone https://github.com/JoyalThomas1199/currency-converter.git
                                       cd currency-converter

You need to login to https://openexchangerates.org/account
Then create a new api key using this URL: https://openexchangerates.org/account/app-ids to generate the application key to use in this application.
Copy the application code which is generated from the website - This is used to fetch the realtime currency values - which is required for this application apis.



Build the project: mvn clean package -Dcurrency.api.key=<API KEY GENERATED>
run the jar: java -jar -Dcurrency.api.key=<API KEY GENERATED> target\currencyconverter-0.0.1-SNAPSHOT.jar
Applicattion will be up and running here: http://localhost:8080/api/rates?base=USD

API Documentations can be find here: http://localhost:8080/swagger-ui/index.html
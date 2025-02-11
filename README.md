This project contains a collection of Postman tests for the OpenWeatherMap API. The tests are designed to validate the functionality, edge cases, and error handling of the API.

**Purpose of the Tests**

The purpose of these tests is to:

Validate the correctness of the OpenWeatherMap API responses.

Ensure proper error handling for invalid inputs.

Test various API endpoints, including current weather, forecasts, and geolocation-based queries.

Automate API testing using Postman's scripting capabilities.

**APIs Tested**

The following OpenWeatherMap API endpoints are tested:

**Current Weather Data**

Endpoint: /weather

Parameters: q (city name), id (city ID), lat/lon (geographic coordinates), units, lang, etc.

**Error Scenarios**

Invalid API key.

Invalid city name.

Missing required parameters.

**Rate Limiting**

Testing the API's rate limit handling.

How to Import and Run the Tests in Postman
**Step 1: Import the Collection**

Download the Postman collection JSON file from this repository.

Open Postman.

Click on the Import button in the top-left corner.

Select the downloaded JSON file to import the collection.

**Step 2: Set Up Environment Variables**

In Postman, create a new environment (e.g., OpenWeatherMap).

Add the following variables:

api_key: Your OpenWeatherMap API key.

city: Default city name (e.g., London).

invalid_city: Invalid city name (e.g., InvalidCityName).

invalid_api_key: Invalid API key (e.g., INVALID_API_KEY).

**Step 3: Run the Tests**

Select the imported collection in Postman.

Choose the environment you created (OpenWeatherMap).

Click the Runner button at the top of Postman.

Select the collection and click Run.

View the test results in the Postman console.

# 11 Prompt Engineering: Weather Forecast

## Description

This project is a Weather Forecast API that retrieves a five-day weather forecast for a given city and presents it in the style of a sports announcer. The purpose of this project is to enhance prompt engineering skills by integrating the OpenAI API to generate creative and engaging weather reports.

The application follows a simple workflow:  
- A user submits a city name through a `POST` request.  
- The backend fetches real-time weather data.  
- The OpenAI API is used to transform this data into a lively sports announcer-style forecast.  
- The formatted response is returned as a JSON object.  

This project is an optional challenge designed to reinforce skills in API integration, Express.js, and working with environment variables. Users can modify the prompt style to receive weather forecasts in different tones, such as those of a cartoon character or a historical figure. The project also emphasizes the importance of securing API keys and testing API endpoints using Insomnia.

## Table of Contents

- [Usage](#usage)
- [Instructions](#instructions)
- [Key Features](#key-features)
- [Sample Input](#sample-input)
- [Sample Output](#sample-output)
- [Technology Stack](#technology-stack)
- [Additional Resources](#additional-resources)

## Usage

To start the application, follow these steps:

1. Install dependencies:
```bash
npm install
```

2. Set up your .env file with your OpenAI API key

3. Run the server:
```bash
npm start
```

4. Use Insomnia or Postman to send a `POST` request to:

```bash
http://localhost:3000/forecast
```

With the following JSON body:

```json
{
  "location": "Sacramento CA"
}
```

5. Receive a five-day weather forecast styled as a sports announcer’s report.

## Instructions

1. Clone the repository and navigate to the project directory.

2. Install all necessary dependencies using npm install.

3. Create a .env file and add your OpenAI API key.

4. Start the application using npm start.

5. Open Insomnia or Postman and send a request to test the API.

6. Modify the OpenAI prompt in the code if you'd like to change the forecast style.

## Key Features

* Fetches a five-day weather forecast based on a user-provided city.

* Uses the OpenAI API to transform weather data into an engaging sports announcer-style report.

* Allows users to customize the forecast style.

* Provides JSON-formatted responses for easy integration with front-end applications.

* Secures API keys using an .env file.

* Enables API testing through Insomnia or Postman.

## Sample Input

```json
{
  "location": "Sacramento CA"
}
```

## Sample Output

```json
{
  "result": {
    "day1": "And here we go, folks! Day one in Sacramento is looking like a scorcher with a high of 95 degrees and clear skies. It's going to be a hot one out there!",
    "day2": "Moving on to day two, we've got a slight cool down with a high of 90 degrees and a chance of some afternoon showers. It's going to be a nail-biter to see if the rain holds off for the big game!",
    "day3": "Day three is shaping up to be a beautiful day in Sacramento with a high of 85 degrees and sunny skies. Perfect weather for a day out on the golf course or a picnic in the park!",
    "day4": "As we head into day four, temperatures are on the rise again with a high of 92 degrees and mostly sunny conditions. It's going to be a real sizzler out there on the field!",
    "day5": "And finally, on day five, we're looking at a high of 88 degrees with a mix of sun and clouds. It's going to be a thrilling end to the week as we see if the weather holds up for the big championship game!"
  }
}
```

## Technology Stack

* **Node.js & Express.js:** Handles API requests and responses.

* **OpenAI API:** Generates creative weather forecasts based on provided weather data.

* **dotenv:** Manages environment variables securely.

* **Insomnia/Postman:** Used for testing API endpoints.

## Additional Resources

* Learn how to set up an OpenAI API key: Full-Stack Blog: [OpenAI Account Setup Guide](https://coding-boot-camp.github.io/full-stack/ai/openai-account-setup-guide)

* OpenAI API Documentation: [OpenAI API Docs](https://platform.openai.com/docs/overview)


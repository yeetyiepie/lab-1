# FastAPI Factorial API

## Objectives
- Introduce FastAPI as a technology stack for developing APIs
- Review Python as a programming language for API development
- Create, run, and test APIs created using FastAPI
- Practice logic building and technical expertise through coding

## Instructions
1. Create an API that will fulfill the following requirements:
   - Written in FastAPI
   - Endpoint Name: `/factorial/{starting_number}`
   - Endpoint should execute the following logic:
     - Compute the factorial of the inputted value in the endpoint
     - If the value inputted is 0, the endpoint should return `{ "result": false }`
     - Implement the code using a while loop
2. Turn in the GitHub repository link of the code, together with dependencies needed to run the application in Google Classroom

## Features
- Computes the factorial of a positive integer.
- Returns an error response if the input is 0.
- Uses FastAPI for efficient and easy API handling.

## Requirements
- Python 3.7+
- FastAPI
- Uvicorn

## Installation

1. Clone this repository:
   ```sh
   git clone (GIT URL)
   cd factorial-api
   ```

2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   ```

3. Install dependencies:
   ```sh
   pip install fastapi uvicorn
   ```

## Running the API
Start the FastAPI server using Uvicorn:
```sh
uvicorn main:app --reload
```

## Usage
Make a GET request to the following endpoint to get the factorial of a number:
```sh
GET http://127.0.0.1:8000/factorial/{starting_number}
```

### Example Request:
```sh
GET http://127.0.0.1:8000/factorial/5
```

### Example Response:
```json
{
  "starting_number": 5,
  "factorial": 120
}
```

## API Documentation
Once the server is running, you can view the interactive API documentation at:
- Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

## License

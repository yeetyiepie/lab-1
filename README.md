# FastAPI Factorial API

This is a simple FastAPI application that calculates the factorial of a given number.

## Features
- Calculates the factorial of a given number.
- Returns a JSON response.
- Built with FastAPI.

## Requirements

Ensure you have the following installed:
- Python 3.7+
- FastAPI
- Uvicorn

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/fastapi-factorial.git
   cd fastapi-factorial
   ```

2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
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

Send a GET request to:
```
http://127.0.0.1:8000/factorial/{starting_number}
```
Replace `{starting_number}` with the number whose factorial you want to calculate.

### Example Request:
```
GET http://127.0.0.1:8000/factorial/5
```

### Example Response:
```json
{
  "starting_number": 5,
  "factorial": 120
}
```

If `starting_number` is `0`, the API will return:
```json
{
  "return": false
}
```

## License

This project is licensed under the MIT License. See `LICENSE` for more details.


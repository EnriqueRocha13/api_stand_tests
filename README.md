# Python API Testing Project

## Description
This project provides automated API testing for user creation endpoints using Python and pytest. It includes comprehensive test cases covering positive and negative scenarios.

## Features
- Automated user creation endpoint testing
- Positive and negative test case validation
- Response code and payload verification
- User data persistence validation
- Easy to extend and maintain

## Requirements
- Python 3.6+
- pytest
- requests

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/EnriqueRocha13/api_stand_tests.git
   cd api_stand_tests
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Run the tests using pytest:
```bash
pytest create_user_test.py -v
```

## Project Structure
```
api_stand_tests/
├── configuration.py          # API configuration and endpoints
├── data.py                   # Test data and headers
├── sender_stand_request.py   # API request functions
├── create_user_test.py       # User creation test cases
├── test_main.py              # Main test execution
└── README.md
```

## Test Cases
The project includes 10 comprehensive test cases:

### Positive Tests
1. Create user with 2-letter first name
2. Create user with 15-letter first name

### Negative Tests
3. Create user with 1-letter first name (error expected)
4. Create user with 16-letter first name (error expected)
5. Create user with spaces in first name (error expected)
6. Create user with special characters (error expected)
7. Create user with numbers in first name (error expected)
8. Create user without firstName parameter (error expected)
9. Create user with empty firstName (error expected)
10. Create user with numeric type for firstName (error expected)

## Configuration
Edit `configuration.py` to update API endpoints:
- `URL_SERVICE`: Base API URL
- `CREATE_USER_PATH`: User creation endpoint
- `USERS_TABLE_PATH`: Users database path

## Contributing
Feel free to submit pull requests and issues. All contributions are welcome!
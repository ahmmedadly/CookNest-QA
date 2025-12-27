# Food Planner API Testing (TheMealDB)

This repository contains API testing artifacts for the **Food Planner Android application**.
The APIs under test are provided by **TheMealDB public API**.

## Tools Used
- Postman
- Postman Collection Runner
- Git & GitHub

## API Details
- **Base URL:** https://www.themealdb.com/api/json/v1/1
- **Protocol:** REST
- **Method:** GET
- **Authentication:** Not required (public API)

## Tested Endpoints
- Get random meal
- Search meal by name
- Get meal categories
- Filter meals by category
- Filter meals by country
- Get meal details by ID
- Invalid meal ID (negative test)

##  Project Structure
api-testing/
├── test-cases/
│ └── food_planner_api_test_cases.md
├── postman/
│ └── food_planner_postman_collection.json
├── test-summary-report.md
└── README.md

##  How to Run the Tests
1. Import the Postman collection.
2. Ensure the collection variable `base_url` is set.
3. Run the collection using **Postman Collection Runner**.
4. Review test results and assertions.

##  Notes
- During testing, some requests initially failed due to **trailing spaces in query parameters**.
- After correcting parameter formatting, all endpoints returned valid JSON responses.



# Food Planner API Test Cases

## API Provider: TheMealDB
Base URL: https://www.themealdb.com/api/json/v1/1  
Method: GET  
Tool: Postman  

---

## TC_API_001 – Get random meal

**Endpoint:** /random.php  

**Steps:**
1. Send GET request

**Expected Result:**
- Status code 200
- Response contains meal object
- Meal has id, name, image, and instructions

---

## TC_API_002 – Search meal by name

**Endpoint:** /search.php?s=Arrabiata  

**Expected Result:**
- Status code 200
- Meal list returned
- Meal name contains "Arrabiata"

---

## TC_API_003 – Get categories list

**Endpoint:** /categories.php  

**Expected Result:**
- Status code 200
- Categories list is returned
- Each category has id, name, and description

---

## TC_API_004 – Filter meals by category

**Endpoint:** /filter.php?c=Seafood  

**Expected Result:**
- Status code 200
- Meals list returned
- Each meal belongs to Seafood category

---

## TC_API_005 – Filter meals by country

**Endpoint:** /filter.php?a=Canadian  

**Expected Result:**
- Status code 200
- Meals list returned
- Each meal belongs to Canadian cuisine

---

## TC_API_006 – Get meal details by ID

**Endpoint:** /lookup.php?i=52772  

**Expected Result:**
- Status code 200
- Meal details returned
- Ingredients, measurements, and instructions present

---

## TC_API_007 – Invalid meal ID

**Endpoint:** /lookup.php?i=999999  

**Expected Result:**
- Status code 200
- meals field is null or empty


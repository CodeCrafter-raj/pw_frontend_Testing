# pw_frontend_Testing Assignment


# JMeter Performance Testing Report

This project contains a collection of performance/load tests created using Apache JMeter. The tests simulate user traffic on various endpoints to analyze how the server responds under load.

---

## 📁 Test Scenarios

### ✅ 1. API Load Testing using Reqres.in (https://reqres.in/)
#### ➤ GET Request
- **Description:** Simulates fetching user data.
- **Number of Threads (Users):** 50  
- **Ramp-Up Period:** 5 seconds  
- **HTTP Method:** GET  
- **Endpoint:** `/api/users?page=2`  
- **Purpose:** Measure response time and behavior under concurrent load.

#### ➤ POST Request
- **Description:** Simulates user registration or login.
- **Number of Threads (Users):** 50  
- **Ramp-Up Period:** 5 seconds  
- **HTTP Method:** POST  
- **Endpoint:** `/api/users`  
- **Payload:** JSON body with user data  
- **Purpose:** Test how the system handles POST operations under load.

---

### ✅ 2. Website Load Testing using SimpliLearn (https://www.simplilearn.com)
#### ➤ Pages Tested:
1. **Home Page**  
2. **Resource Section**  
3. **Corporate Section**

- **Number of Threads (Users):** 50 per request  
- **Ramp-Up Period:** 5 seconds for each  
- **HTTP Method:** GET  
- **Purpose:** Test how the SimpliLearn site performs under concurrent user load for major user-facing pages.

---

## 📊 Result Output

- **All results were saved as `.csv` files** for further analysis.
- The `View Results Tree` and `View Results Table` listeners were used during testing for debugging and validation.

---

## 🧪 Tools Used

- **Apache JMeter**
- **Localhost and Public Test APIs (reqres.in)**
- **SimpliLearn Website**

---

## 🔍 Notes

- Proper headers like `Content-Type: application/json` were added using **HTTP Header Manager**.
- Tests simulate realistic user traffic patterns and provide insight into application behavior under load.

---

---

## 📌 How to Run

1. Open `.jmx` file in JMeter.
2. Configure thread settings if needed.
3. Click on **Start** to run the test.
4. View live results in listeners or examine the `.csv` output.

---

Feel free to customize or extend this setup for more advanced test scenarios like authentication, session tracking, or distributed load testing.


---


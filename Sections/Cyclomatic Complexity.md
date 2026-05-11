# 6. Cyclomatic Complexity

There are 2 decision statements:

## 6.1 Decision Statement 1

* `IF username == "admin" AND password == "admin123"`

## 6.2 Decision Statement 2

* `ELSE IF username == "user" AND password == "user123"`


## 6.3 Cyclomatic Complexity Calculation

* **Formula:**
    * `V(G) = Number of decisions + 1`

* **Substitution:**
    * `V(G) = 2 + 1`

* **Final Result:**
    * `V(G) = 3`

* **Cyclomatic Complexity:**
    * `3`


## 6.4 Independent Paths

There are three independent paths:

## 6.4.1 Path 1

* **Purpose:** Admin login successful.
* **Steps:**
    * Start
    * Display `"Enter Username"`
    * Input username
    * Display `"Enter Password"`
    * Input password
    * Check admin condition = `TRUE`
    * Display `"Welcome, Administrator."`
    * Call `LoadAdminDashboard`
    * End

---

## 6.4.2 Path 2

* **Purpose:** User login successful.
* **Steps:**
    * Start
    * Display `"Enter Username"`
    * Input username
    * Display `"Enter Password"`
    * Input password
    * Check admin condition = `FALSE`
    * Check user condition = `TRUE`
    * Display `"Welcome, User."`
    * Call `LoadUserDashboard`
    * End

---

## 6.4.3 Path 3

* **Purpose:** Invalid credentials.
* **Steps:**
    * Start
    * Display `"Enter Username"`
    * Input username
    * Display `"Enter Password"`
    * Input password
    * Check admin condition = `FALSE`
    * Check user condition = `FALSE`
    * Display `"Error: Invalid Credentials."`
    * Call `ShowLoginScreen`
    * End

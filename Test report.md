# Software Testing – Timetable, Room & Lab Allocation

## 📌 Testing Overview

As a member of the **Software Testing Team**, I performed manual testing on the **Timetable, Room & Lab Allocation System** to verify that the implemented features work according to the specified project requirements.

The testing covered two main areas:

* **Manual Frontend Testing**
* **Manual API Testing using Swagger UI**

The testing focused on system behavior, data validation, conflict detection, authorization, and the main scheduling workflow.

---

## 🧪 Testing Scope

### 1. Manual Frontend Testing

The Frontend was tested manually by interacting directly with the application interface as a real user.

The testing included:

* Login and system access
* Navigation between system pages
* Creating and managing Sections
* Selecting Courses, Student Groups, Lecturers, and Rooms
* Creating timetable allocations
* Testing scheduling conflicts
* Testing room capacity and requirements
* Testing Draft and Published Schedules
* Verifying the timetable displayed to students
* Testing search and filtering functionality
* Checking reports and displayed information
* Verifying validation messages and system responses

---

### 2. Manual API Testing

API testing was performed manually using **Swagger UI**.

The testing focused on:

* Sending valid and invalid requests
* Checking **HTTP Status Codes**
* Validating API responses
* Testing input validation
* Testing business logic
* Testing conflict detection
* Testing authorization and role-based access
* Verifying unauthorized operations
* Checking error handling

---

## 🛠️ Testing Tools

| Tool            | Purpose                                     |
| --------------- | ------------------------------------------- |
| **Swagger UI**  | Manual API testing and response validation  |
| **Web Browser** | Manual Frontend testing                     |
| **GitHub**      | Reviewing repositories and project progress |

---

## 🖥️ Manual Frontend Testing

The Frontend was tested through direct interaction with the application.

### Main Tested Areas

| Area               | Testing Activity                                        |
| ------------------ | ------------------------------------------------------- |
| Login              | Verify user login and system access                     |
| Sections           | Create and validate Section data                        |
| Allocations        | Assign Sections to Rooms, Lecturers, and Time Slots     |
| Conflict Detection | Verify that scheduling conflicts are rejected           |
| Rooms              | Verify Capacity, Type, and Equipment requirements       |
| Draft Schedule     | Verify Draft behavior                                   |
| Publishing         | Verify schedule publishing                              |
| Student View       | Verify that students see the latest published timetable |
| Search & Filters   | Verify search and filtering results                     |
| Reports            | Verify displayed reports and timetable information      |

---

## 🔌 Manual API Testing Using Swagger

**Swagger UI** was used to manually execute and validate API requests.

### Testing Process

1. Open the Swagger API Documentation.
2. Select the required endpoint.
3. Click **Try it out**.
4. Enter the required request data.
5. Click **Execute**.
6. Check the **HTTP Status Code**.
7. Check the **Response Body**.
8. Compare the Actual Result with the Expected Result.

### API Testing Areas

| Testing Area        | What Was Verified                           |
| ------------------- | ------------------------------------------- |
| Request Validation  | Required and valid input data               |
| Response Validation | Response body and returned data             |
| Status Codes        | Successful and rejected requests            |
| Business Logic      | Scheduling rules                            |
| Conflict Detection  | Room, Lecturer, and Student Group conflicts |
| Authorization       | Access based on user roles                  |
| Error Handling      | Invalid and unauthorized operations         |

---

## 🚨 Conflict Testing

Several scheduling conflict conditions were tested manually:

* **Room Conflict**
* **Lecturer Conflict**
* **Student Group Conflict**
* **Capacity Conflict**
* **Equipment/Type Conflict**
* **Room Closure/Maintenance Conflict**
* **Duration Conflict**
* **Overlapping Time Slots**

The purpose was to verify that the system prevents invalid allocations and provides appropriate validation or conflict feedback.

---

## 🔐 Authorization Testing

Role-based access was also tested through the API.

The testing included verifying that:

* Students cannot publish schedules.
* Department Coordinators cannot publish schedules.
* Facilities Managers cannot publish official schedules.
* Users cannot access data outside their permitted scope.
* Unauthorized users cannot access **Audit Logs**.

For unauthorized operations, the expected response was:

`HTTP 403 Forbidden`

---

## 📊 Test Results

The manual tests performed showed that the tested scenarios produced the expected results.

| Testing Type               | Result   |
| -------------------------- | -------- |
| Manual Frontend Testing    | ✅ Passed |
| Manual API Testing         | ✅ Passed |
| Conflict Validation        | ✅ Passed |
| Authorization Testing      | ✅ Passed |
| Input & Validation Testing | ✅ Passed |

### Overall Testing Status

**✅ PASS**

---

## 📝 Conclusion

Manual testing was performed on both the **Frontend Layer** and the **API Layer** of the Timetable, Room & Lab Allocation System.

The Frontend was tested through direct interaction with the user interface, while the APIs were tested manually using **Swagger UI**.

The testing covered:

* Main system functions
* Data validation
* Scheduling conflicts
* Authorization
* Error handling
* Scheduling workflow

The tested scenarios produced the expected results, and the system successfully handled the valid and invalid cases that were tested.

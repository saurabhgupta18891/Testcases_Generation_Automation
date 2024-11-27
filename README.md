# Automated API Test Case Generator and Executor

This application automates the process of generating, executing, and evaluating test cases for APIs. It supports both JSON and XML-based APIs and integrates with OpenAI to generate test cases dynamically based on API specifications and functional requirements.

---

## Features

### 1. **Test Case Generation**
- Generates test cases dynamically for both JSON and XML APIs.
- Supports:
  - **Positive Test Cases**: Validate correct input scenarios.
  - **Negative Test Cases**: Validate error-handling and edge cases.
  - **Business Logic Test Cases**: Verify domain-specific constraints.
  - **Logical Relationship Test Cases**: Ensure inter-parameter consistency.
  - **Remove Mandatory Field Tests**: Evaluate API behavior when required fields are missing.

### 2. **Test Case Execution**
- Executes generated test cases against API endpoints.
- Supports both `POST` and `GET` methods.
- Validates:
  - Status codes.
  - JSON response structure and content.
  - XML response equivalence using canonicalization.

### 3. **Authentication Support**
- Static Token Authentication.
- Basic Authentication (dynamic token generation).
- Supports JSON, XML, and form-urlencoded content types.

### 4. **Integration with MongoDB**
- Stores API definitions, test cases, and execution results.
- Real-time status updates for test execution.

### 5. **Error Logging and Intermediate Data Updates**
- Detailed logging for troubleshooting.
- Intermediate statistics are calculated and updated during execution.

---

## Setup and Installation

### Prerequisites
- Python 3.8 or later.
- MongoDB instance (local or cloud).
- OpenAI API key.
- Required Python packages (specified in `requirements.txt`).

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/api-test-generator.git
   cd api-test-generator

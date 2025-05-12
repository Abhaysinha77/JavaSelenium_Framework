# JavaSelenium_Framework

A robust, scalable, and maintainable UI automation framework built using **Java**, **Selenium WebDriver**, and **TestNG**. Designed for cross-browser testing, data-driven execution, and seamless integration with CI/CD pipelines.

---

## 🚀 Features

- ✅ Modular framework with Page Object Model (POM)
- ✅ Cross-browser testing support (Chrome, Firefox, Edge)
- ✅ Data-driven testing using Excel/JSON/Properties
- ✅ TestNG-based test orchestration
- ✅ Centralized configuration and reusable utilities
- ✅ Detailed test reports (Extent or Allure integration)
- ✅ Screenshots on failure
- ✅ Headless test execution
- ✅ Docker-ready for isolated test environments
- ✅ Easily integrable with Jenkins/GitLab CI

---

## 📂 Project Structure

JavaSelenium_Framework/
├── src/
│ ├── main/
│ │ └── java/
│ │ └── framework/
│ │ ├── base/ # Base classes (e.g., WebDriver setup)
│ │ ├── pages/ # Page Object classes
│ │ ├── utils/ # Utility classes (e.g., Excel, waits, config)
│ └── test/
│ └── java/
│ └── tests/ # Test classes
├── testng.xml # Test suite configuration
├── config.properties # Test config (browser, baseURL, etc.)
├── Dockerfile # For Dockerized test execution
├── pom.xml # Maven dependencies
└── README.md

yaml
---

## ⚙️ Technologies Used

- Java 11+
- Selenium WebDriver
- TestNG
- Maven
- Extent Reports / Allure
- Apache POI (Excel support)
- Log4j (logging)
- WebDriverManager (automatic driver management)
- Docker (optional containerized execution)

---

## 🧪 How to Run Tests

### 🔹 Run Locally
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/JavaSelenium_Framework.git
   cd JavaSelenium_Framework
Install dependencies

bash
mvn clean install
Run the test suite

bash
mvn test
🔹 Run in Headless Mode
Update your config.properties:

properties
browser=chrome
headless=true
Or modify the WebDriver setup to check a headless flag and enable it dynamically.

🔹 Run with Docker
Ensure Docker is installed and running

Build the Docker image

bash
docker build -t java-selenium-framework .
Run the tests inside a container

bash
docker run --rm java-selenium-framework
💡 Use headless mode in Docker to avoid GUI dependency:

properties
headless=true
📘 Configuration
config.properties – Set browser type, base URL, timeouts, and environment variables

testng.xml – Control test execution flow, suites, test groups, parallelism

📦 CI/CD Integration
This framework is easily integrable with:

Jenkins Pipelines
GitHub Actions
GitLab CI
CircleCI
Supports:
Headless mode
Docker execution
Report publishing

🤝 Contributing
Contributions are welcome! Please fork the repo, create a new branch, and submit a pull request.

📄 License
This project is licensed under the MIT License.

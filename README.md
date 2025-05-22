Here's a **professional `README.md`** file based on your provided Selenium + TestNG Java project that automates a local HTML form:

---

````markdown
# Web Form Automation with Selenium and TestNG

This project automates the testing of a local HTML form using **Selenium WebDriver** and **TestNG**. It dynamically fills out input fields with random data, simulates scrolling behavior, and submits user inputs such as email, password, gender, hobbies, and file uploads.

---

## 📁 Project Structure

```text
CodingAuto.htmlCoding/
│
├── AppTest.java          # Main automation logic using Selenium
├── TestDataAuto.java     # Utility class that generates random test data
└── index.html            # (Local HTML form for automation testing)
````

---

## 🚀 Features

* Scroll to and from sections on the page using JavaScript Executor.
* Auto-fills input fields with:

  * Random names
  * Random email/password/date/phone number
  * Gender selection (randomized)
  * Hobbies selection (multi-checkbox)
  * File upload via absolute file path
* Logs field behavior (e.g., number of hobby checkboxes)

---

## 🔧 Technologies Used

* **Java 8+**
* **Selenium WebDriver**
* **TestNG**
* **ChromeDriver**
* **Maven** (recommended for dependency management)

---

## ⚙️ Setup Instructions

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/form-auto-selenium.git
   cd form-auto-selenium
   ```

2. **Install Dependencies:**
   Make sure to include dependencies in `pom.xml` (if using Maven):

   ```xml
   <dependencies>
     <dependency>
       <groupId>org.seleniumhq.selenium</groupId>
       <artifactId>selenium-java</artifactId>
       <version>4.1.2</version>
     </dependency>
     <dependency>
       <groupId>org.testng</groupId>
       <artifactId>testng</artifactId>
       <version>7.4.0</version>
       <scope>test</scope>
     </dependency>
   </dependencies>
   ```

3. **Start a Local Server** (if you're using `index.html` locally):
   You can run a basic server using VS Code Live Server or:

   ```bash
   npx serve .
   ```

4. **Run the Tests:**

   * From IDE (e.g., Eclipse or IntelliJ) via `TestNG Suite`
   * Or via terminal:

     ```bash
     mvn test
     ```

---

## 🧪 Test Cases

| Test Name                 | Description                                               | Status                       |
| ------------------------- | --------------------------------------------------------- | ---------------------------- |
| `ScrollT()`               | Scrolls down and up the page using JS                     | Disabled (`enabled = false`) |
| `FillingTheInputFields()` | Fills out and submits the form using randomized test data | ✅ Enabled                    |

---

## 🗂️ Data Source: `TestDataAuto.java`

This class contains:

* Arrays of test values (emails, names, passwords, dates, phone numbers)
* A random generator to select values at runtime
* Absolute path to test file for file upload field

---

## 📌 Notes

* Ensure `chromedriver` is available in your system `PATH`.
* Test assumes the form exists locally at: `http://127.0.0.1:5500/index.html#media-section`
* Update file path in `TestDataAuto.java` if your directory is different.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Mousa AbuKhaled**
Feel free to reach out via [LinkedIn](https://linkedin.com) or [GitHub](https://github.com)

```

---

Let me know if you want:
- A version in Arabic
- Screenshots or badges added
- GitHub Actions CI setup included

Would you like me to generate a `LICENSE` file or `pom.xml` too?
```


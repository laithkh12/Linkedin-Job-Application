# 🚀 LinkedIn Job Application Bot

![selenium-logo](https://upload.wikimedia.org/wikipedia/commons/d/d5/Selenium_Logo.png)

A Python-based automation script that uses **Selenium WebDriver** to automate job applications on LinkedIn. This tool simplifies the application process by automatically filling in required fields and submitting applications.

---

## 📋 Features

- Automatically logs in to LinkedIn.
- Navigates to job postings for specified keywords and locations.
- Fills in phone number details if required.
- Skips complex applications or those requiring additional steps.
- Keeps the browser open for debugging in case of errors.

---

## ⚙️ Prerequisites

Before you start, ensure you have the following:

1. **Python 3.7+**
2. **Google Chrome Browser**
3. **ChromeDriver** compatible with your Chrome version.
4. Install required Python libraries:
   ```bash
   pip install selenium
    ```
---
## 🚀 How to Use
1. Clone this repository or copy the script into your working directory.
2. Update the **ACCOUNT_EMAIL**, **ACCOUNT_PASSWORD**, and **PHONE** variables with your LinkedIn login credentials and phone number.
3. Run the script
4. Solve the CAPTCHA manually when prompted and press Enter.
---
## 📂 Script Workflow
1. Reject Cookies:
  - Automatically rejects cookies when the LinkedIn page loads.
2. Log In
  - Signs in to your LinkedIn account using the provided credentials.
3. Retrieve Job Listings
  - Gathers all job listings based on the search criteria in the URL.
4. Automate Applications
  - Opens each job listing.
  - Clicks the "Apply" button.
  - Fills in the phone number if missing.
  - Submits or skips complex applications.
5. Handle Errors
  - Skips listings with missing or complex forms using the abort_application function.
---
## 🖋️ Example Configuration
Update these variables in the script:
```python
ACCOUNT_EMAIL = "your_email@example.com"
ACCOUNT_PASSWORD = "your_password"
PHONE = "123-456-7890"
```
---
## ⚠️ Important Notes
- This script is designed for personal use. Ensure compliance with LinkedIn's terms of service.
- CAPTCHA must be solved manually when prompted.
- The job search criteria can be modified by updating the LinkedIn URL in the script:
```python
driver.get("https://www.linkedin.com/jobs/search/?currentJobId=3977068347&keywords=python&location=israel%2C%20Israel%2C%20Israel%20Israel")
```
---
## 🛠 Troubleshooting
- **Browser Not Opening**? Check if the chromedriver executable is installed and added to your system's PATH.
-  **Errors During Login**? Ensure your credentials are correct and try updating them in the script.
-  **Form Issues**? If the bot skips too many applications, ensure the CSS selectors match LinkedIn's current HTML structure.
---
## 🤝 Contributing
Contributions are welcome! Feel free to submit a pull request or suggest improvements.
---
## 📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
---
## 🌟 Acknowledgments
- Powered by Selenium WebDriver.
- Inspired by the need to simplify repetitive tasks.

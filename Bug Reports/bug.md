# 🐞 Bug Report for Login Page Testing

## 📝 Overview

During the manual testing of the login functionality on **app.vwo.com**, a variety of test cases were executed to ensure the robustness of the login system. The testing focused on validating both successful logins with valid credentials and error handling for invalid inputs. Over **30+ test cases** were tested, with most cases passing successfully. However, a few bugs were encountered and are documented below.

## 🐛 Bugs Identified

| 🆔 **Bug ID** | 📝 **Description** | ⚠️ **Severity** | 🔄 **Steps to Reproduce** | ✅ **Expected Result** | ❌ **Actual Result** | 📌 **Status** |
|---------------|--------------------|-----------------|---------------------------|------------------------|----------------------|---------------|
| 001           | Login page freezes when submitting blank credentials after an invalid attempt | 🔴 High      | 1. Enter invalid username and password<br>2. Submit<br>3. Leave fields blank<br>4. Submit again | Error message should be displayed | Page becomes unresponsive | 🟠 Open |
| 002           | Error message does not disappear after a successful login attempt | 🟡 Medium    | 1. Enter invalid credentials<br>2. Submit<br>3. Enter valid credentials<br>4. Submit | Error message should disappear after a successful login | Error message remains on the screen | 🟠 Open |
| 003           | Special characters in username field cause page to break | 🔴 Critical  | 1. Enter special characters only in the username field<br>2. Submit | Error message should be displayed | Page breaks with server error | 🟠 Open |

## 📊 Summary of Test Cases

- **Total Test Cases Executed**: **30+**
- **Test Cases Passed**: **✅ 27**
- **Test Cases Failed**: **❌ 3**

## 🔍 Conclusion

The majority of test cases passed successfully, ensuring the login system is functioning as expected for typical user behavior. However, a few bugs were identified, particularly around edge cases like special characters in the username field and error handling. These need to be addressed to improve system stability.

📎 You can view the full test case report [here](https://1drv.ms/x/c/9b08bc18d9bc6fe0/ESc1STwX9wtAoNQe61aSNc4BZ1CMEikc1fX8RqhEhOyKjg).

---

**Note:** All critical bugs have been logged, and further testing will be performed after the fixes are implemented.

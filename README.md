# QuishGuard - QR Code Analyzer
QuishGuard is a web-based tool built using Flask and Selenium to analyze the safety of QR codes. The application decodes QR codes, checks URL reputations using the VirusTotal API, and performs behavior analysis of URLs in an isolated, headless browser environment.

### Features
QR Code Decoding: Upload a QR code image, and the application will extract and display the URL or data encoded in the QR code.
URL Safety Check: The application uses VirusTotal to check the URL’s reputation, providing the number of antivirus engines that flagged the URL as malicious.
Behavior Analysis: Using Selenium in headless mode, the application analyzes the behavior of the URL (e.g., redirects) in a controlled environment.

### Security
API Key Handling: The VirusTotal API key is stored in a separate config.py file, which is not included in the repository for security reasons.
Headless Browser: The application uses Selenium in headless mode to safely analyze URLs in an isolated environment.

### Future Work
- Real-time / Daily CVE Reporting, detailed views for CVE overview
- Phishing detection with machine learning, the user will input/copy a message, and a phishing confidence rate will be displayed

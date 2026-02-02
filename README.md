# SafePaste | Zero-Trust PII Redactor

**Stop feeding sensitive data to public LLMs.**

SafePaste is a client-side utility that automatically sanitizes text before you paste it into tools like ChatGPT, Claude, or DeepSeek. It runs 100% in the browser—no data is ever sent to a server.

## Live Demo
[**Click here to use SafePaste**](https://thelovearinze.github.io/safe-paste/)

## Why SafePaste?
Engineers and legal teams often need to analyze logs or contracts using AI. However, pasting raw data violates SOC2, GDPR, and PCI-DSS compliance because it exposes PII (Personally Identifiable Information) to third-party training data.

SafePaste acts as an "Air Gap" layer. It scrubs sensitive entities locally, ensuring **Data Isolation**.

## Capabilities
The engine uses regex pattern matching to identify and redact:
* **Network Logic:** IPv4 Addresses, MAC Addresses (Network Engineering focus)
* **Financial:** Credit Card Numbers (PCI-DSS compliant masking), Dollar Amounts
* **Identity:** Email Addresses, US Phone Numbers
* **Temporal:** Dates (MM/DD/YYYY)

## Security Architecture
* **Client-Side Only:** Built with vanilla HTML/JS. No backend. No API calls.
* **Zero External Dependencies:** No tracking scripts or analytics.
* **Open Source:** The code is transparent. What you see is what runs.

## Usage
1.  Open the [Live Demo](https://thelovearinze.github.io/safe-paste/).
2.  Paste your server logs, legal text, or emails into the **Input** box.
3.  Click **Redact PII & Logs**.
4.  Copy the sanitized text from the **Output** box.

## License
MIT License. Free to use for personal and commercial security workflows.

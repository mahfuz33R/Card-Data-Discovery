# Card Data Discovery Tool
"Automates the detection of unencrypted and unmasked cardholder data to support PCI DSS compliance with detailed Excel-based reporting and secure scanning capabilities."

**Version**: 2.0  

**Author**: Md Mahfuzur Rahman, CVA, CNSP, CPAv2 

**Email**: mahfuz33r@gmail.com 

**Website**: mahfuz33r.github.io (https://mahfuz33r.github.io)

![Card Data Discovery](/assets/Dashboard.png)

## Overview

The **Card Data Discovery Tool (CDD)** is a powerful and secure solution designed to assist financial institutions, banks, and enterprises in detecting unencrypted and unmasked cardholder data stored within their systems. The tool is built to simplify compliance with **PCI DSS (Payment Card Industry Data Security Standard)** by automating the discovery process and generating detailed reports in Excel format.


## **What is PCI DSS Compliance, and Why is It Important?**

### **What is PCI DSS?**
The **Payment Card Industry Data Security Standard (PCI DSS)** is a set of global security standards designed to ensure that all companies that process, store, or transmit credit card information maintain a secure environment. It was established by major credit card companies like Visa, MasterCard, and American Express to protect cardholder data and prevent fraud and data breaches.


### **Why is PCI DSS Compliance Necessary?**
- **Protects Sensitive Data**: Helps safeguard cardholder information from unauthorized access or theft.
- **Prevents Data Breaches**: Reduces the risk of costly data breaches that can damage an organization's reputation.
- **Regulatory Requirements**: Many industries are legally required to comply with PCI DSS standards to process card payments.
- **Avoid Penalties**: Non-compliance can result in fines, lawsuits, and loss of merchant privileges.


### **How Does the Card Data Discovery Tool Help Achieve Compliance?**
This tool addresses two critical requirements of PCI DSS compliance:
1. **Data Discovery**:
   - Scans connected drives and files to locate unencrypted or unmasked cardholder data.
   - Identifies sensitive data that should be encrypted or removed to meet PCI DSS requirements.

2. **Automated Reporting**:
   - Provides Excel-based output files (`valid_card_data.xlsx` and `invalid_card_data.xlsx`) with card data masked to ensure no sensitive information is leaked during the reporting process.
   - Helps organizations document and track their progress in securing cardholder data.

3. **Prevention of Non-Compliance Risks**:
   - By detecting and reporting card data stored in non-compliant formats, this tool allows businesses to take corrective actions and avoid penalties.
   - Validates detected card data using the **Luhn Algorithm**, reducing false positives and ensuring accurate reporting.

By using the **Card Data Discovery Tool**, organizations can efficiently scan their systems for sensitive cardholder data, generate detailed compliance reports, and take the necessary steps to secure their environments—bringing them closer to full PCI DSS compliance.


## Key Features

- **Automated Scanning**: Scans all connected drives for predefined patterns of card data (Visa, MasterCard, AMEX, Discover, etc.).
- **Excel-Based Reporting**: Outputs results in Excel format for easy review and reporting.
- **Card Masking**: Ensures detected card data is masked to maintain client privacy and avoid accidental data exposure.
- **File Filtering**: Limits scans to specific file types (e.g., `.txt`, `.docx`, `.xlsx`) for faster processing.
- **Validation with Luhn Algorithm**: Detects only valid card data to minimize false positives.
- **Compliance Support**: Assists in PCI DSS compliance by identifying sensitive data requiring encryption or removal.

## How It Works

1. **Drive Detection**: Automatically detects all connected drives and lists them for scanning.
2. **Pattern Matching**: Scans files for specific card data patterns using regex and validates results with the Luhn algorithm.
3. **Excel Reporting**: Generates detailed Excel reports:
   - `valid_card_data.xlsx` for detected valid card data.
   - `invalid_card_data.xlsx` for flagged false positives.
   - File paths and masked card data ensure sensitive information remains secure.
4. **Security First**: Operates in read-only mode to prevent modification of scanned files.

## Installation

1. **Download the Executable**: [Download Here](#).
2. **System Requirements**:
   - **OS**: Windows (with administrative privileges).
3. **Setup**:
   - Double-click the executable to launch.
   - Follow the on-screen instructions to begin scanning.

## Usage

1. Run the executable file with administrative privileges. You need user email and password. [**Feel Free to email me for a temporary Email and Password to test the tool**]
2. By default it will scan all the drives that are connected so you just need to wait with patience. 
3. Monitor the progress through the command-line interface.
4. Retrieve the output Excel files:
   - `card_data_discovery_output.txt`
   - `<IP>_client_data.xlsx`
   - `<IP>_masking_data.xlsx`

## Security Measures

- **Read-Only Access**: Ensures no data is modified during scanning.
- **Minimal Logging**: Logs only operational data like timestamps while avoiding storage of sensitive data.
- **Card Masking**: Detected card data is displayed in a masked format to prevent exposure.
- **Luhn Validation**: Ensures accuracy of detected data, reducing false positives.

## Troubleshooting

- **Permission Errors**: Ensure you run the tool as an administrator.
- **Unsupported Files**: Ensure scanned files are within supported formats (`.txt`, `.docx`, `.xlsx`, etc.).
- **Missing Dependencies**: Contact support if you encounter dependency errors during execution.

For additional support, feel free to contact me at **mahfuz33r@gmail.com **.

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or submit an issue in this repository.

## Contact

For questions, feedback, or collaboration, please reach out via:
- **Email**: mahfuz33r@gmail.com 
- **Website**: [mahfuz33r.github.io](https://mahfuz33r.github.io)

---

## Acknowledgments

This tool was developed to simplify compliance with PCI DSS standards and provide financial organizations with a reliable method for securing sensitive cardholder data.

**Let’s secure the digital future together!**

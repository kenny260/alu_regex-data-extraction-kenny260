              Regex Data Extraction Project

 Overview

This project uses Python and Regular Expressions (Regex) to extract structured data (like emails, URLs, phone numbers, and more) from unstructured text.  

 Extracted Data Types

- Email addresses  
- URLs  
- Phone numbers  
- Credit card numbers  
- Time (12h and 24h formats)  
- HTML tags  
- Hashtags  
- Currency amounts  

 Technologies Used

- Python 3  
- Regex (`re` module)  

  Repository Structure

 alu_regex-data-extraction-kenny260/
│
├── regex_extractor.py # Main Python script
├── README.md # Project documentation

   Setup Instructions

1.Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/alu_regex-data-extraction-kenny260.git
   cd alu_regex-data-extraction-kenny260

Make sure you have Python 3 installed.

 How to Run

Run the script in your terminal:

python3 regex_extractor.py

  Example Output

Emails: ['user@example.com', 'firstname.lastname@company.co.uk']
URLs: ['https://www.example.com', 'https://sub.example.org/page']
Phone Numbers: ['(123) 456-7890', '123-456-7890', '123.456.7890']
Credit Card Numbers: ['1234 5678 9012 3456', '1234-5678-9012-3456']
Hashtags: ['#example', '#ThisIsAHashtag']
24-Hour Times: ['14:30', '07:00']
12-Hour Times: ['2:30 PM', '12:15 AM']






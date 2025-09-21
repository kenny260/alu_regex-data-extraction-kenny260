🔍 Regex Data Extraction Project

This project shows how to use Regular Expressions (Regex) in Python to pull useful information out of messy text.
It was built as part of the ALU Regex Data Extraction Assignment.

What the Program Does

The script scans through a block of text and extracts:

📧 Email addresses

🌐 URLs (web links)

📞 Phone numbers

💳 Credit card numbers

🏷️ Hashtags

⏰ Time (24-hour and 12-hour formats)

🛠️ Tools Used

Python 3

Regex (re standard library)

📂 Repo Layout
alu_regex-data-extraction-{YourUsername}/
│
├── regex_extraction.py   # Main Python script
├── README.md             # Project documentation
└── sample_output.txt     # Example output from the program (optional)

▶️ How to Run It

Clone the repo to your computer:

git clone https://github.com/{YourUsername}/alu_regex-data-extraction-{YourUsername}.git
cd alu_regex-data-extraction-{YourUsername}


Run the Python script:

python regex_extraction.py


Check your terminal output. Example:

Emails: ['user@example.com', 'firstname.lastname@company.co.uk']
URLs: ['https://www.example.com', 'https://sub.example.org/page']
Phone Numbers: ['(123) 456-7890', '123-456-7890', '123.456.7890']
Credit Card Numbers: ['1234 5678 9012 3456', '1234-5678-9012-3456']
Hashtags: ['#example', '#ThisIsAHashtag']
24-Hour Times: ['14:30', '07:00']
12-Hour Times: ['2:30 PM', '12:15 AM']

✨ Features

✔️ Works with multiple data types (emails, URLs, phones, cards, hashtags, times)
✔️ Handles different formats (e.g., 24h & 12h time, phone separators)
✔️ Patterns are clear and reusable for learning purposes

⚡ Edge Case Handling

Prevents grabbing trailing punctuation in URLs

Accepts phone numbers with (), -, . or spaces

Recognizes both AM/PM and 24-hour times

📌 Example Regex Patterns

Email

\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[a-zA-Z]{2,}\b


Phone Number

\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}


Credit Card

\b(?:\d{4}[- ]?){3}\d{4}\b


Hashtags

#\w+


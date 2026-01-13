# website-status-checker 🌐

A simple Python script that checks the HTTP status of websites listed in a CSV file and prints their status codes with readable descriptions. Great for beginners learning CSV handling, HTTP requests, and status code handling in Python.

---

## 🎯 How It Works

- Reads a list of websites from `websites.csv`.  
- Sends an HTTP GET request to each website (with a real browser-like `User-Agent`).  
- Prints the URL along with the HTTP status code and its description (e.g., `200 OK`, `404 Not Found`).  
- Handles errors gracefully (e.g., if a site is unreachable).

Example output:
https://apple.com (200 OK) OK

https://facebook.com (200 OK) OK

https://this_website_is_not_real.com **Could not get information for website: "https://this_website_is_not_real.com"

https://newgrounds.com (200 OK) OK

https://linkedin.com (200 OK) OK

...

text

---

## 🐍 How to Run

1. Install the required packages:
   ```bash
   pip install requests fake-useragent
Make sure you have:

main.py (this script)

websites.csv in the same folder, with format:

text
1,"apple.com"
2,"facebook.com"
...
Run the script:

bash
python main.py
📂 Files
main.py – The main website status checker script.

websites.csv – CSV file containing the list of websites to check (format: id,"domain").

🌟 Why This Project?
Great for practicing:

Reading CSV files with csv.reader

Making HTTP requests with requests

Handling HTTP status codes using http.HTTPStatus

Using fake-useragent to avoid being blocked

Simple error handling and logging

Easy to extend (e.g., save results to a file, add timing, or add a GUI).

📜 License
This project is open source and available under the MIT License. Feel free to use, modify, and share it!







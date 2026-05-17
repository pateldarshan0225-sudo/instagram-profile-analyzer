# 📊 Instagram Profile Data Parser & Analyzer

A Python-based project that reads raw Instagram profile data from a text file, parses it into structured format, and performs basic analysis — finding top accounts by **posts**, **followers**, and **following**, along with listing all unique **account categories**.

---

## 📁 Project Structure

```
├── finaldata.txt       # Raw Instagram profile data (text format)
├── cob1.ipynb          # Parse and analyze Instagram profile data
└── README.md           # Project documentation
```

---

## 📓 Notebook Overview

### `cob1.ipynb` — Data Parser & Analyzer

- Reads raw Instagram profile data from `finaldata.txt`
- Splits data into individual profile chunks
- Parses each profile into structured fields:
  - Username
  - Posts count
  - Followers count
  - Following count
  - Name
  - Account Type
  - Bio
- Converts **K** (thousands) and **M** (millions) to actual numbers
- Finds account with **maximum posts**
- Finds account with **maximum followers**
- Finds account with **maximum following**
- Lists all unique **account categories**

---

## 📊 Data Format (Raw Text)

Each profile block in `finaldata.txt` looks like this:

```
username
120 posts
4.5K followers
300 following
Full Name
Account Type
Bio line here
```

---

## ✅ Analysis Results

| Metric | Result |
| --- | --- |
| 🏆 Maximum Posts | startuphub_blr |
| 👥 Maximum Followers | _anujsinghal |
| 👣 Maximum Following | bangalore_tech_bro |
| 🗂️ Total Account Categories | 34 |

---

## 🗂️ Account Categories Found (34)

```
Nonprofit organization, Tech Creator, Investor, Recruiter,
Blogger, Community, Cafe Explorer, Public Figure, Engineer,
Digital creator, Personal Blog, Backend Developer, Full-stack Dev,
Artist + Coder, Data Science, Cafe Nerd, Educator, Food & Drink,
Blog, Founder, Tech, Product Manager, Developer, Media,
Data Scientist, Design, Education, Entrepreneur, Software Engineer,
Frontend Dev, Comedy, Writer, Coder, Lifestyle
```

---

## ⚙️ How to Run

1. **Clone the repository**

```
git clone https://github.com/YourUsername/instagram-profile-analyzer.git
cd instagram-profile-analyzer
```

2. **Install Jupyter Notebook**

```
pip install notebook
```

3. **Launch Jupyter**

```
jupyter notebook
```

4. **Open and run:**
   - `cob1.ipynb` → Run all cells to parse and analyze data

---

## 🧠 Logic Used

| Feature | Logic |
| --- | --- |
| Data Parsing | Split by double newline, then by single newline |
| K/M Conversion | String replace + float multiplication |
| Max Posts/Followers/Following | Linear scan with comparison |
| Category Extraction | Python `set()` for unique values |

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Jupyter Notebook**
- **JSON** (for data serialization)
- No external libraries required (only built-in `json` module)

---

## 👨‍💻 Author

> Made by **pateldarshan0225-sudo (Darshan Patel)** as a data parsing and analysis project on Instagram profile data.

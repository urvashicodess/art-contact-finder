#Gallery Scraper

This Python script crawls a list of UK-based gallery websites and automatically extracts:

-  Gallery Name
-  Address
-  Email
-  Phone
-  Social Media Links
-  Checks if artist submissions are accepted

### Outputs
- `gallery_data.json`: Local backup of data
-  Google Sheet (auto-updated)

---

##  Requirements

- Python 3.x
- Virtual environment (`venv`)
- Google Sheets API credentials (`.json` file, not pushed to GitHub)

---

## How to Run

```bash
# Step 1: Clone the repo
git clone https://github.com/urvashicodess/gallery-scraper.git
cd gallery-scraper

# Step 2: Create virtual environment
python -m venv venv
venv\Scripts\activate       # On Windows
# source venv/bin/activate  # On Mac/Linux

# Step 3: Install dependencies
pip install -r requirements.txt

# Step 4: Add your Google Service Account JSON
Place your `.json` file (e.g., `gallery-leads-xxx.json`) in the root folder.

# Step 5: Run the scraper
python scraper.py


Now **Save the file**.

---

##  Step 2: Add a `.gitignore` File (If not already there)

This file prevents sensitive or unnecessary files from being pushed.

1. In VS Code, create a new file:


2. Paste this:

```gitignore
gallery-leads-*.json
__pycache__/
venv/
*.pyc
.DS_Store

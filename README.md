# Generate Newsletter

<div align="center">

### 📰 Automated Newsletter Generation | 🕷️ Web Scraping | 📧 HTML Newsletter

**Automated newsletter generation system that curates news articles and presents them in HTML format**

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Project Structure](#-project-structure)
- [Setup](#-setup)
- [Usage](#-usage)
- [Technologies Used](#-technologies-used)

---

## 🎯 Overview

The "Newsletter from Scratch" project is a comprehensive automation system designed to simplify the process of curating news articles from various sources and presenting them in a visually appealing HTML-based newsletter. By utilising modern web scraping techniques and advanced data transformation methods, this system ensures that end-users are always updated with the most relevant and recent news articles in their areas of interest.

---

## ✨ Features

- **🕷️ Automated Article Collection**: Scrapes news articles from various reputable sources using predefined search queries
- **📊 CSV Storage**: Stores scraped articles in structured CSV format for easy processing
- **📧 HTML Newsletter Generation**: Transforms articles into visually appealing HTML newsletters
- **🎨 Template-Based**: Uses customisable HTML templates for consistent formatting
- **🖼️ Image Integration**: Automatically includes related images in newsletters
- **📁 Archive Management**: Organises generated newsletters in a dedicated directory

---

## 🔄 How It Works

### Article Collection

The `main.py` script in the "Collect News Articles" directory:

1. Reads predefined search queries from `search querys.txt`
2. Uses the `gnews` library to scrape relevant news articles from various reputable sources
3. Ensures diversity and credibility in the news presented
4. Stores article details (title, author, URL, summary) in `scraped_articles.csv`

### Newsletter Generation

The `generate_html.py` script in the "Generate HTML document" directory:

1. Reads collected articles from `scraped_articles.csv`
2. Uses predefined templates from the "templates" directory to craft HTML documents
3. Fetches related images from the "images" directory to enhance visual presentation
4. Saves the final newsletter in the "newsletters" directory, ready for distribution

---

## 📁 Project Structure

```
Generate-Newsletter/
├── Collect News Articles/
│   ├── main.py                    # Article scraping script
│   ├── scraped_articles.csv      # Scraped articles data store
│   └── search querys.txt         # Search queries for article collection
│
├── Generate HTML document/
│   ├── generate_html.py          # Newsletter generation script
│   ├── data/                     # Supplementary data
│   ├── images/                   # Visual assets for newsletters
│   ├── newsletters/              # Archive of generated newsletters
│   └── templates/                # HTML templates
│       ├── article_img_template.html
│       ├── combined_newsletter_template.html
│       ├── footer_template_web.html
│       ├── header_template.html
│       └── section_header_template.html
│
└── README.md
```

---

## 🚀 Setup

### Prerequisites

- Python 3.x
- `gnews` library

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MatthewPaver/generate-newsletter.git
   cd generate-newsletter
   ```

2. **Install dependencies:**
   ```bash
   pip install gnews
   ```

3. **Configure search queries:**
   - Edit `Collect News Articles/search querys.txt` with your desired search terms
   - Each line represents a search query

---

## 📖 Usage

### Step 1: Collect News Articles

Navigate to the "Collect News Articles" directory and run:

```bash
python main.py
```

This will:
- Read search queries from `search querys.txt`
- Scrape articles using the gnews library
- Save results to `scraped_articles.csv`

### Step 2: Generate Newsletter

Navigate to the "Generate HTML document" directory and run:

```bash
python generate_html.py
```

This will:
- Read articles from `scraped_articles.csv`
- Apply HTML templates
- Include images from the images directory
- Generate the newsletter in the `newsletters/` directory

### Output

The generated newsletter will be saved in the `newsletters/` directory with a timestamp-based filename (e.g., `08-23_web.html`).

---

## 💻 Technologies Used

<div align="center">

**🐍 Python** **📰 gnews** **🌐 Web Scraping** **📧 HTML/CSS**

</div>

### Key Libraries

- **gnews** — News article scraping library
- **Python Standard Library** — CSV handling, file operations

---

## 📝 Notes

- **Search Queries**: Customise `search querys.txt` to target specific topics or keywords
- **Templates**: Modify HTML templates in the `templates/` directory to change newsletter appearance
- **Images**: Place related images in the `images/` directory for automatic inclusion
- **CSV Format**: The `scraped_articles.csv` file contains structured data for easy processing

---

## 🔧 Customisation

### Modifying Templates

Edit HTML templates in the `templates/` directory to customise:
- Newsletter layout and structure
- Header and footer design
- Article presentation format
- Styling and visual appearance

### Adding Search Queries

Add new search terms to `Collect News Articles/search querys.txt`, one per line, to expand article coverage.

---

## 📄 License

This project is provided for educational and demonstration purposes.

---

<div align="center">

**Automated Newsletter Generation System**

[⬆ Back to Top](#generate-newsletter)

</div>

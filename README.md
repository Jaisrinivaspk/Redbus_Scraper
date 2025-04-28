# Redbus Data Scraper

## 🚀 Project Overview
**Redbus Data Scraper** is a web scraping and data analysis project that extracts bus travel data from the Redbus website using Selenium. The data is stored in an SQL database and visualized using an interactive **Streamlit** application, allowing users to dynamically filter results based on pickup and drop-off locations, bus type, ratings, and more.

This project aims to automate and streamline data collection for travel aggregators, market researchers, and transport service providers.

---

## 🛠️ Tech Stack
- **Python**
- **Selenium** (for web scraping)
- **SQL** (for data storage)
- **Streamlit** (for UI development)
- **Pandas** (for data handling)

---

## 📦 Project Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/redbus-data-scraper.git
cd redbus-data-scraper
```

### 2. Create a Virtual Environment
```bash
python -m venv venv
```

Activate the environment:

- Windows:
  ```bash
  venv\Scripts\activate
  ```
- macOS/Linux:
  ```bash
  source venv/bin/activate
  ```

### 3. Install Required Libraries
```bash
pip install -r requirements.txt
```

---

## ⚙️ How to Run the Project

1. **Launch the Streamlit Application**  
   Start the UI by running:
   ```bash
   streamlit run ui.py
   ```

2. **Interact with the Application**  
   - Enter the **pickup** and **drop** locations.
   - View available buses, prices, timings, seat availability, and more.
   - Apply filters such as bus type, star ratings, price range, and availability.

---

## 📋 Features
- Automated scraping of bus routes, timings, star ratings, and ticket prices from Redbus.
- Structured storage of the data into a SQL database.
- Interactive Streamlit app for real-time dynamic filtering.
- Easy and user-friendly UI for exploring transport options.

---

## 📊 Database Schema

| Column Name     | Data Type | Description                     |
|-----------------|-----------|---------------------------------|
| id              | INT       | Primary Key (Auto-increment)    |
| route_name      | TEXT      | Bus Route information           |
| route_link      | TEXT      | Link to route details           |
| busname         | TEXT      | Name of the bus service         |
| bustype         | TEXT      | Bus Type (Sleeper/Seater/AC/Non-AC) |
| departing_time  | TIME      | Departure time                  |
| duration        | TEXT      | Duration of journey             |
| reaching_time   | TIME      | Arrival time                    |
| star_rating     | FLOAT     | Passenger rating                |
| price           | DECIMAL   | Ticket price                    |
| seats_available | INT       | Available seats                 |

---

## 📈 Business Use Cases
- Real-time bus schedule updates for travel aggregators.
- Market and competitor analysis based on travel data.
- Customer service enhancement by offering personalized options.
- Strategic planning based on travel trends.

---

## 🎯 Project Goals
- Scrape a minimum of 10 government and private buses.
- Design a clean and efficient SQL database.
- Build a user-friendly and interactive Streamlit application.
- Ensure high data accuracy and fast application performance.

---

## 📑 References
- [Selenium Documentation](https://www.selenium.dev/documentation/webdriver/elements/locators/)
- [Streamlit Documentation](https://docs.streamlit.io/get-started/installation)
- [Redbus Website](https://www.redbus.in/)

---


# Investors Dashboard Project

**Objective:**  
This project is an interactive, investor-focused dashboard providing insights into vehicle registrations in India. It allows users to explore trends across vehicle categories (2W, 3W, 4W) and manufacturers, and view Year-over-Year (YoY) and Quarter-over-Quarter (QoQ) growth.

---

## Tech Stack
- **Backend:** FastAPI, PostgreSQL
- **Frontend:** Streamlit
- **Data Collection:** Python Scraper
- **Data Format:** JSON / CSV

---

## Repository Structure

The project is divided into three repositories:

1. [Investor Dashboard Frontend](#https://github.com/akr-38/investor-dashboard-frontend) – Streamlit dashboard for visualizing the data  
2. [Investor Dashboard Backend](#https://github.com/akr-38/investor-dashboard-backend) – FastAPI APIs serving registration stats  
3. [Investor Dashboard Scraper and Storing](#https://github.com/akr-38/investor-dashboard-scraping-and-storing) – Data collection, cleaning, and DB setup  

---

## Setup Instructions (High-Level)

1. **Data Scraper & DB**  
   - Go to the Scraper repository-[Investor Dashboard Scraper and Storing](#https://github.com/akr-38/investor-dashboard-scraping-and-storing) and follow its README to set up and populate the database.  

2. **Backend & Frontend**  
   - You can set up the backend-[Investor Dashboard Backend](#https://github.com/akr-38/investor-dashboard-backend), frontend-[Investor Dashboard Frontend](#https://github.com/akr-38/investor-dashboard-frontend), or both.  
   - Each repository has its own README with setup instructions.  

---

## Project Description

### Phase 1: Data Scraping, Processing, and Storage
- Collects vehicle registration data from public Vahan Dashboard sources  
- Processes and aggregates data into broad categories (2W, 3W, 4W)  
- Stores data in PostgreSQL for backend access  

### Phase 2: Frontend Dashboard
- Standalone frontend fetches data via FastAPI backend  
- Users can filter by vehicle category, manufacturer, and date range  
- Displays interactive line charts and calculates YoY/QoQ growth  

---

## Architecture Diagram

          +----------------+
          |   Scraper      |
          |(Data Collection|
          | & Processing)  |
          +-------+--------+
                  |
                  v
          +----------------+
          |   Database     |
          +-------+--------+
                  ^
                  |
                  |
          +-------+--------+
          |   Backend      |
          | (APIs / Logic) |
          +-------+--------+
                  ^
                  |
                  v
          +----------------+
          |   Frontend     |
          | (Streamlit UI) |
          +----------------+

---

## Key Features
- Filter by vehicle category and manufacturer  
- Select date range (quarter-wise)  
- YoY and QoQ calculations  
- Interactive line charts to visualize trends  



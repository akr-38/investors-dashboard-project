

# Investor Dashboard Project

An interactive, investor-focused dashboard providing insights into the Indian automobile industry.

## 🚀 Objective

This project is an interactive dashboard that provides comprehensive insights into vehicle registration data in India from 2010 to 2025. It allows investors and analysts to:

* **Analyze Market Trends:** Visualize and understand market trends across the entire automobile industry.
* **Filter Data:** Drill down into specific segments, including vehicle categories (2W, 3W, 4W) and individual manufacturers.
* **Track Performance:** View key metrics like Year-over-Year (YoY) and Quarter-over-Quarter (QoQ) growth.

This project is designed to help users make informed decisions by providing a clear, data-driven perspective on the Indian automotive market.

***

## ⚙️ Tech Stack

This project is built using a modern, scalable tech stack across three distinct services.

* **Frontend:** `Streamlit`
* **Backend:** `FastAPI`, `Python`
* **Data Collection:** `Python Scrapping`, `Selenium`
* **Database:** `Supabase` (PostgreSQL)
* **Data Format:** `JSON`

***

## 📂 Repository Structure

The project is organized into three separate repositories, each with its own purpose and detailed setup instructions.

1.  **[Investor Dashboard Scraper and Storing](https://github.com/akr-38/investor-dashboard-scraping-and-storing)**
    * Handles data scraping from the Vahan Dashboard.
    * Performs data cleaning, processing, and aggregation.
    * Manages the database setup and populates the `Supabase` (PostgreSQL) database.

2.  **[Investor Dashboard Backend](https://github.com/akr-38/investor-dashboard-backend)**
    * Provides `FastAPI` endpoints for data access.
    * Serves the processed vehicle registration stats to the frontend.
    * Acts as the central business logic layer.

3.  **[Investor Dashboard Frontend](https://github.com/akr-38/investor-dashboard-frontend)**
    * A `Streamlit` application for data visualization.
    * Allows users to interact with filters (vehicle category, manufacturer, date range).
    * Displays key metrics and interactive charts.

***

## 🛠️ Getting Started

This main repository acts as a central hub. To run the full project, you will need to set up each of the three individual repositories in the correct order.

### Prerequisites

You must have Python 3.9+ installed and a `Supabase` project set up. You will need to configure your environment variables for the database connection (e.g., database URL, API keys).

### Setup Instructions

Follow these steps to get the entire project up and running:

1.  **Database Setup & Data Population**
    * Start by cloning and navigating to the `Scraper and Storing` repository.
    * Follow the detailed `README.md` within that repository to set up the database schema and scrape the necessary data. This will populate your `Supabase` instance.

2.  **Backend Server**
    * Next, clone and navigate to the `Backend` repository.
    * Follow its `README.md` to install dependencies and configure the environment variables to connect to your `Supabase` database.
    * Run the FastAPI server to ensure the APIs are functional and serving data correctly.

3.  **Frontend Dashboard**
    * Finally, clone and navigate to the `Frontend` repository.
    * Follow the setup instructions in its `README.md` to install the required libraries.
    * Configure the environment variables to point to your running `FastAPI` backend.
    * Start the Streamlit application to view the dashboard and interact with the data.

***

## 📊 Architecture Diagram

The project follows a standard three-tier architecture, where the data collection and storage are decoupled from the application logic and presentation layer.

<img width="512" height="279" alt="image" src="https://github.com/user-attachments/assets/e3b5a5ef-b36a-4174-8344-4040dc540fe0" />


***

## ✨ Features

* **Customizable Data Views:** Filter data by vehicle category (2W, 3W, 4W) and a wide range of manufacturers.
* **Time-Series Analysis:** Select a specific date range to analyze quarterly trends.
* **Interactive Visualizations:** Interactive line charts to visualize and compare trends over time.
* **Key Performance Indicators:** Automatic calculation of Year-over-Year (YoY) and Quarter-over-Quarter (QoQ) growth.

***

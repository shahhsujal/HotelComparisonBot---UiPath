# 🏨 Hotel Comparison Bot - UiPath

## 📌 Overview
Hotel Comparison Bot is a Robotic Process Automation (RPA) project built using **UiPath**. This bot automates the process of scraping hotel data from **Booking.com** and **Trivago**, applies user-defined filters like **maximum price** and **minimum rating**, merges the results, and exports the filtered hotel list into an Excel file.

This project showcases how web automation, data filtering, and Excel interaction can be seamlessly combined using UiPath workflows.

---

## ⚙️ Features
- 🌐 Automated web scraping from Booking.com and Trivago.
- 🧾 User input via Input Dialogs for price and rating preferences.
- 🧮 Dynamic filtering of data based on user-defined criteria.
- 📊 Merging filtered results from both platforms.
- 📁 Export to Excel for reporting and comparison.
- 💬 Confirmation and status messages after each major step.

---

## 📂 Project Structure

| File Name               | Description                                                |
|------------------------|------------------------------------------------------------|
| `Main.xaml`            | Orchestrates the entire bot flow, user inputs, and merging |
| `Scrape_Booking.xaml`  | Scrapes hotel data from Booking.com                        |
| `Scrape_Trivago.xaml`  | Scrapes hotel data from Trivago                            |
| `FilteredHotels.xlsx`  | Final Excel output after filtering and merging             |
| `HotelData.xlsx`       | Raw data output from each platform                         |

---

## 🧪 How It Works

1. **User Inputs**: Prompted to enter a **maximum price** and **minimum rating**.
2. **Web Scraping**:
   - Opens Booking.com and Trivago in Chrome.
   - Extracts hotel name, price, and rating using **Table Extraction**.
3. **Data Storage**: Writes data to `HotelData.xlsx`.
4. **Filtering Logic**:
   - Applies regex cleaning on prices and ratings.
   - Filters hotels that match user criteria.
5. **Merging**: Combines filtered results from both platforms.
6. **Export**: Writes the final list to `FilteredHotels.xlsx`.
7. **Notifications**: Displays message boxes confirming each step.

---

## 📦 Requirements
- UiPath Studio 2025.0.161 or higher
- Chrome browser with UiPath extension installed
- Excel installed (for viewing exports)

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/HotelComparisonBot-UiPath.git

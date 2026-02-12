# 🦠 COVID-19 Data Analysis Project

## 📌 Project Description
This project is developed using Python to fetch real-time COVID-19 data using a public API.  
It displays total confirmed cases, total deaths, and total recovered patients worldwide.

---

## 🎯 Aim
The aim of this project is to understand:
- API integration in Python
- JSON data handling
- Real-time data fetching

---

## 🛠 Technologies Used
- Python
- Requests Library
- JSON
- GitHub

---

## ⚙ How It Works
1. The program sends a request to the COVID-19 API.
2. The API returns data in JSON format.
3. Python extracts required values.
4. The program displays total cases, deaths, and recovered data.

---

## 💻 Source Code

```python
import requests

url = "https://disease.sh/v3/covid-19/all"
response = requests.get(url)
data = response.json()

print("Total Cases:", data["cases"])
print("Total Deaths:", data["deaths"])
print("Total Recovered:", data["recovered"])

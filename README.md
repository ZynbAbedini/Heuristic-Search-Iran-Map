# 🇮🇷 Iran Provinces Pathfinding (Search Algorithms)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)

> **Note:** For the Persian (Farsi) version of this README, please scroll down. 
> نسخه فارسی توضیحات در نیمه پایین صفحه قرار دارد.

## 🇬🇧 English Description

This project implements and compares various search algorithms (**BFS**, **DFS**, **A***, and **Weighted A***) to find the shortest path between Iranian provincial capitals based on real distance data. It serves as a practical exploration of Artificial Intelligence search strategies.

### 🚀 Features
* **Algorithms Implemented**: Breadth-First Search (BFS), Depth-First Search (DFS), A* Search, and Weighted A* Search.
* **Real-World Data**: Uses actual road distances and straight-line (Euclidean) distances for heuristic functions.
* **Performance Comparison**: Evaluates and compares execution time, path length, and the number of visited nodes.

### 🛠 Tech Stack
* **Language**: Python
* **Libraries**: `pandas` (for data manipulation), `heapq` (priority queue for A*), `collections` (deque for BFS).

### 📊 Performance Comparison (Sample)
Example route: **Tabriz → Bandar Abbas**

| Algorithm | w | Path Length (km) | Nodes Visited | Execution Time (s) |
| :--- | :---: | :---: | :---: | :---: |
| **A\*** | 1.0 | **2007** | 24 | 0.023 |
| **Weighted A\*** | 1.5 | 2058 | 7 | 0.010 |
| **BFS** | - | 2058 | 14 | 0.00006 |
| **DFS** | - | 5391 | 15 | 0.00005 |

### 📖 Analysis Summary
* **A\*** provides the optimal, shortest path because its heuristic is *admissible*.
* **Weighted A\*** significantly reduces the number of visited nodes (making it faster) but sacrifices perfect optimality.
* **DFS** is very fast and uses minimal memory but often results in extremely long, sub-optimal paths.

---
---

## 🇮🇷 توضیحات فارسی (Persian)

### مسیریابی استان‌های ایران (الگوریتم‌های جستجو)

این پروژه به زبان **پایتون** نوشته شده و به پیاده‌سازی و مقایسه الگوریتم‌های پایه و پیشرفته‌ی جستجو (**BFS**، **DFS**، **A*** و **Weighted A***) برای یافتن مسیر بین مراکز استان‌های ایران می‌پردازد. هدف این پروژه بررسی عملکرد الگوریتم‌های هوش مصنوعی روی داده‌های واقعی است.

### 🚀 ویژگی‌ها
* **الگوریتم‌های پیاده‌سازی شده**: جستجوی سطح‌اول، جستجوی عمق‌اول، A* و A* وزن‌دار.
* **داده‌های واقعی**: استفاده از فواصل جاده‌ای واقعی و فواصل خط مستقیم (به عنوان تابع تخمین یا Heuristic).
* **مقایسه عملکرد**: ارزیابی الگوریتم‌ها بر اساس زمان اجرا، طول مسیر نهایی و تعداد گره‌های بررسی شده.

### 🛠 تکنولوژی‌ها
* **زبان برنامه‌نویسی**: Python
* **کتابخانه‌ها**: `pandas` (برای مدیریت داده‌ها)، `heapq` (صف اولویت‌دار)، `collections`.

### 📊 جدول مقایسه (نمونه)
مسیر نمونه: **تبریز به بندرعباس**

| الگوریتم | مقدار w | طول مسیر (km) | تعداد گره‌های بازدیدی | زمان اجرا (s) |
| :--- | :---: | :---: | :---: | :---: |
| **A\*** | 1.0 | **2007** | 24 | 0.023 |
| **Weighted A\*** | 1.5 | 2058 | 7 | 0.010 |
| **BFS** | - | 2058 | 14 | 0.00006 |
| **DFS** | - | 5391 | 15 | 0.00005 |

### 📖 خلاصه تحلیل الگوریتم‌ها
* الگوریتم **A\*** به دلیل استفاده از تابع تخمین مجاز (Admissible)، همیشه بهینه‌ترین و کوتاه‌ترین مسیر را پیدا می‌کند.
* الگوریتم **Weighted A\*** سرعت جستجو را بالا برده و تعداد گره‌های بازدیدی را کم می‌کند، اما ممکن است بهینه‌ترین مسیر را پیدا نکند (Trade-off بین سرعت و کیفیت).
* الگوریتم **DFS** با وجود سرعت بالا، مسیرهای بسیار طولانی و غیربهینه پیشنهاد می‌دهد.

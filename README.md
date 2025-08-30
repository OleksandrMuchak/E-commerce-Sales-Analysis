# Portfolio Project 1: E-commerce Sales Analytics
In this project, a comprehensive sales analytics solution will be developed for an e-commerce store using three key tools: **SQL**, **Python**, and **Tableau**.

# Портфоліо-проєкт 1: Аналітика продажів інтернет-магазину
У цьому проєкті буде побудована комплексна аналітика продажів для інтернет-магазину з використанням трьох ключових інструментів: **SQL**, **Python** та **Tableau**.


## Project Objective
* Demonstrate proficiency in extracting and merging data from a database using **SQL**.
* Showcase exploratory and statistical data analysis skills in **Python**.
* Highlight the ability to build interactive analytical dashboards in **Tableau**.

## Мета проєкту  
* Показати навички вивантаження та об'єднання даних із бази даних за допомогою **SQL**.
* Продемонструвати навички розвідувального та статистичного аналізу даних у **Python**.
* Показати вміння будувати інтерактивні аналітичні дашборди у **Tableau**.

## Project Outcome
1. **Jupyter Notebook**: Contains the entire workflow—from data loading and cleaning to statistical analysis and final insights.
2. **Tableau Dashboard**: An interactive dashboard published on Tableau Public, showcasing key sales metrics and trends.

## Результат
1.  **Jupyter Notebook**: містить весь процес від завантаження даних до статистичного аналізу та висновків.
2.  **Tableau Dashboard**: інтерактивний дашборд, опублікований у Tableau Public.

---

## Project Execution Plan
### 1. Dataset Creation (SQL & Python)
Connect to the Google BigQuery database ('DA dataset') and write an SQL query to generate the primary dataset.

## План виконання проєкту
### 1. Створення датасету (SQL & Python)
Підключитися до бази даних Google BigQuery ('DA dataset') та написати SQL-запит для створення основного датасету.

**Dataset Requirements:**
The dataset should include the following fields:
* Order date
* Session ID
* Continent
* Country
* Device
* Browser
* Device model name
* Operating system
* Browser language
* Traffic source information
* Traffic channel
* Registered user ID
* Email confirmation status
* Newsletter subscription status
* Product category
* Product name
* Price
* Short product description

**Note:** Use appropriate types of table joins (JOIN) to ensure all orders and sessions are included, even those from unregistered users.

**Вимоги до датасету:**
Датасет має містити такі поля:
* дата замовлення
* ідентифікатор сесії
* континент
* країна
* девайс
* браузер
* назва моделі пристрою
* операційна система
* мова браузера
* інформація про джерело трафіку
* канал трафіку
* ідентифікатор зареєстрованого користувача
* чи підтвердив користувач свій email
* чи підписався користувач на розсилку
* категорія товару
* назва товару
* ціна
* короткий опис товару

**Примітка:** Використовувати коректні типи з'єднань таблиць (`JOIN`), щоб врахувати всі замовлення та сесії, навіть від незареєстрованих користувачів.

---

### 2. Data Description and Exploratory Data Analysis (EDA)
**Dataset Overview:**
* Total number of columns and their data types (numerical, categorical, datetime)
* Number of unique sessions
* Time period covered by the dataset
* Missing values analysis: quantity, location, and potential causes

### 2. Опис та розвідувальний аналіз даних (EDA)
**Опис датасету:**
* Загальна кількість та типи колонок (числові, категоріальні, datetime).
* Кількість унікальних сесій.
* Часовий період, що розглядається.
* Аналіз пропущених значень: їх кількість, розташування та ймовірні причини.

**Analytical Questions:**
* Top 3 continents and top 5 countries by total sales and number of orders
* Top 10 product categories by total sales
* Comparison of the top 10 product categories globally vs. in the highest-selling country
* Sales analysis by device types and models (as a percentage of total sales)
* Sales analysis by traffic sources (as a percentage of total sales)
* Percentage of registered users who confirmed their email
* Percentage of registered users who unsubscribed from the newsletter
* Comparison of purchasing behavior between subscribed and unsubscribed users
* Top countries by number of registered users

**Аналітичні питання:**
* Топ-3 континентів та топ-5 країн за сумою продажів та кількістю замовлень.
* Топ-10 категорій товарів за загальною сумою продажів.
* Порівняння топ-10 категорій товарів у світі та в країні з найбільшими продажами.
* Аналіз продажів у розрізі типів та моделей девайсів (у % від загальних продажів).
* Аналіз продажів за джерелами трафіку (у % від загальних продажів).
* Відсоток зареєстрованих користувачів, які підтвердили email.
* Відсоток зареєстрованих користувачів, які відписалися від розсилки.
* Порівняння купівельної поведінки підписаних та відписаних користувачів.
* Топ країн за кількістю зареєстрованих користувачів.

---

### 3. Sales Dynamics & Summary Tables
**Sales Dynamics:**
* Visualization of overall sales trends, including seasonality detection
* Analysis of sales dynamics by continent (Americas, Asia, Europe)
* Analysis of sales dynamics by traffic sources and device types

**Summary Tables:**
* Number of sessions segmented by traffic sources and device types
* Total sales for the top 10 product categories across the top 5 countries

### 3. Аналіз динаміки та зведені таблиці
**Динаміка продажів:**
* Візуалізація загальної динаміки продажів. Пошук сезонності.
* Аналіз динаміки продажів за континентами (Америка, Азія, Європа).
* Аналіз динаміки продажів за каналами трафіку та типами девайсів.

**Зведені таблиці:**
* Кількість сесій у розрізі каналів трафіку та типів девайсів.
* Загальні продажі за топ-10 категоріями у топ-5 країнах.

---

### 4. Statistical Analysis
**Relationship & Correlation Analysis:**
* Relationship between number of sessions and total sales
* Correlation of sales across the top 3 continents
* Correlation of sales by different traffic sources
* Correlation of sales across the top 5 product categories

**Group Comparison Analysis (Statistical Tests):**
* Comparison of sales between registered and unregistered users
* Comparison of session counts across different traffic channels
* Comparison of the share of organic traffic in Europe vs. the Americas

### 4. Статистичний аналіз
**Аналіз взаємозв’язків (кореляція):**
* Взаємозв'язок між кількістю сесій та загальними продажами.
* Кореляція продажів між топ-3 континентами.
* Кореляція продажів за різними каналами трафіку.
* Кореляція продажів за топ-5 категоріями товарів.

**Аналіз відмінностей між групами (статистичні тести):**
* Порівняння продажів зареєстрованих та незареєстрованих користувачів.
* Порівняння кількості сесій за різними каналами трафіку.
* Порівняння долі органічного трафіку в Європі та Америці.

---

### 5. Dashboard Creation in Tableau
Design an analytical dashboard in Tableau Public with no more than 2 pages, summarizing the key findings from the analysis.

### 5. Створення дашборду в Tableau
Створити аналітичний дашборд у Tableau Public, що містить не більше 2 сторінок та узагальнює ключові результати аналізу.


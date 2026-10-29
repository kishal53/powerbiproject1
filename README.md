::: {align="center"}
# 📊 Superstore Sales Dashboard

### *Power BI-Based Data Cleaning, KPI Analysis, Visualisation & Interactive Reporting Project*

`<br/>`{=html}

> *"Turn raw sales data into clear insights and smarter decisions."*

**Author:** Gosai Kishal \| **Project File:** `PR1_kishal.pbix`
:::

------------------------------------------------------------------------

## 📋 Table of Contents

-   [📌 Overview](#-overview)
-   [🎯 Problem Statement](#-problem-statement)
-   [✨ Key Features](#-key-features)
-   [🏗️ Project Structure](#-project-structure)
-   [🔄 Project Workflow](#-project-workflow)
-   [📥 Part A --- Dataset &
    Preparation](#-part-a--dataset--preparation)
-   [📊 Part B --- Analysis, Visualisation &
    Dashboard](#-part-b--analysis-visualisation--dashboard)
-   [🛠️ Tech Stack](#️-tech-stack)
-   [📈 Results & Insights](#-results--insights)
-   [🚀 How to Use](#-how-to-use)
-   [🏆 Advantages](#-advantages)
-   [⚠️ Limitations & Checks](#️-limitations--checks)
-   [👤 Author](#-author)
-   [🙏 Acknowledgements](#-acknowledgements)

------------------------------------------------------------------------

## 📌 Overview

The **Superstore Sales Dashboard** is an interactive Microsoft Power BI
report built using the **Sample Superstore** retail sales dataset. It
presents key sales and business measures through KPI cards, category and
regional charts, dropdown slicers, and a detailed order-data table.

The report is designed to help users explore sales, profit, quantity,
discounts, product categories, and regional performance in one place.

This project demonstrates how to: - Prepare and organise retail sales
data for reporting - Present business KPIs with Card visuals - Compare
sales across product categories - Compare profit across regions - Add
dropdown slicers for interactive filtering - Display detailed
order-level records in a table visual

------------------------------------------------------------------------

## 🎯 Problem Statement

> **Objective:** Analyse a retail Superstore dataset and communicate
> useful sales and profit information through an interactive Power BI
> dashboard and a detailed data page.

  ---------------------------------------------------------------------------
  📂 Task         📄 Skills Tested        🔍 Project Implementation
  --------------- ----------------------- -----------------------------------
  1\. Dataset     Data loading and field  Uses the `Sample - Superstore` data
  Import          inspection              model

  2\. Data        Column naming,          Report uses readable fields such as
  Preparation     filtering and field     `Shipping Mode` and `Sub Category`
                  organisation            

  3\. KPI Cards   Aggregation and summary Cards display Sales, Profit,
                  reporting               Quantity and Average Discount

  4\. Data        Comparing categories    Clustered bar charts show Sales by
  Visualisation   and regions             Category and Profit by Region

  5\. Interactive Slicers and report      Region and Category dropdown
  Filtering       filters                 slicers are available on the
                                          dashboard

  6\. Order       Tabular reporting       A separate page displays detailed
  Details                                 order and product fields

  7\. Report      Layout, formatting and  Dashboard and Order Data pages use
  Design          navigation              a consistent light background and
                                          report styling
  ---------------------------------------------------------------------------

------------------------------------------------------------------------

## ✨ Key Features

  -----------------------------------------------------------------------
  Feature                     Description
  --------------------------- -------------------------------------------
  💰 **Sales KPI**            Displays the sum of Sales

  📈 **Profit KPI**           Displays the sum of Profit

  📦 **Quantity KPI**         Displays the sum of Quantity

  🏷️ **Average Discount KPI** Displays the average Discount

  📊 **Sales by Category**    Clustered bar chart comparing sales across
                              product categories

  🌎 **Profit by Region**     Clustered bar chart comparing profit across
                              regions

  🎚️ **Dropdown Slicers**     Region and Category slicers help filter the
                              report

  🚚 **Shipping Mode Filter** The dashboard page has a page-level
                              Shipping Mode filter configured in the
                              report

  🧾 **Order Data Page**      A table displays customer, order, product,
                              sales, discount, profit, quantity, region
                              and shipping details

  🎨 **Consistent Styling**   Light background, charcoal text and a
                              red/charcoal visual theme
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🏗️ Project Structure

``` text
📦 superstore-sales-dashboard/
│
├── 📄 PR1_kishal.pbix             ← Main Power BI report
│   ├── Page 1 (Dashboard)         ← KPI cards, charts and dropdown slicers
│   └── Page 2 (Order Data)        ← Detailed order table
│
└── 📄 README.md                   ← Project documentation
```

### Report Pages

  -----------------------------------------------------------------------
  Page                       Contents
  -------------------------- --------------------------------------------
  **Page 1 (Dashboard)**     Sales, Profit, Quantity and Average Discount
                             KPI cards; Sales by Category chart; Profit
                             by Region chart; Region and Category
                             dropdown slicers

  **Page 2 (Order Data)**    Detailed table with customer, order date,
                             shipping date, product, sales, discount,
                             profit, quantity, segment, region, shipping
                             mode and related fields
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🔄 Project Workflow

``` text
Superstore Dataset
        │
        ▼
Inspect and prepare data
        │
        ▼
Organise fields and filters
        │
        ├───────────────┐
        ▼               ▼
   KPI Cards       Category/Region Charts
        │               │
        └───────┬───────┘
                ▼
      Interactive Dashboard
                │
                ▼
       Detailed Order Data Page
```

------------------------------------------------------------------------

## 📥 Part A --- Dataset & Preparation

### 📝 1. Dataset

The report uses the **Sample - Superstore** data model. The fields
referenced in the report include:

  Field             Purpose
  ----------------- ---------------------------------
  `Order ID`        Identifies an order
  `Customer ID`     Identifies a customer
  `Customer Name`   Customer name
  `Order Date`      Date the order was placed
  `Shipping Date`   Shipping date
  `Shipping Mode`   Shipping method
  `Segment`         Customer segment
  `Region`          Sales region
  `State`           State associated with the order
  `City`            City associated with the order
  `Category`        Product category
  `Sub Category`    Product sub-category
  `Product ID`      Identifies a product
  `Product Name`    Product name
  `Sales`           Sales amount
  `Quantity`        Quantity ordered
  `Discount`        Discount value
  `Profit`          Profit amount

### 🧹 2. Data Preparation Notes

-   The report model uses readable field names such as `Shipping Mode`
    and `Sub Category`.
-   The detailed table includes date hierarchy levels for Order Date and
    Shipping Date.
-   Sales, Profit and Quantity are aggregated as sums in KPI cards.
-   Discount is aggregated as an average for its KPI card.
-   The exact cleaning steps and source-row counts are not documented in
    the PBIX report definition, so they should be added only after
    confirming them in Power Query or the source dataset.

------------------------------------------------------------------------

## 📊 Part B --- Analysis, Visualisation & Dashboard

### 💳 3. KPI Cards

  ------------------------------------------------------------------------
  KPI           Aggregation                        Purpose
  ------------- ---------------------------------- -----------------------
  Sales         Sum                                Shows total sales
                                                   represented by the
                                                   current report context

  Profit        Sum                                Shows total profit
                                                   represented by the
                                                   current report context

  Quantity      Sum                                Shows total quantity
                                                   represented by the
                                                   current report context

  Average       Average                            Shows the average
  Discount                                         discount represented by
                                                   the current report
                                                   context
  ------------------------------------------------------------------------

KPI values can change when applicable slicers or report filters are
changed.

### 📉 4. Charts

  ------------------------------------------------------------------------
  Visual                      Type                 Shows
  --------------------------- -------------------- -----------------------
  Sales by Category           Clustered bar chart  Compares total sales
                                                   across product
                                                   categories

  Profit by Region            Clustered bar chart  Compares total profit
                                                   across regions
  ------------------------------------------------------------------------

### 🎚️ 5. Filters & Interactivity

-   **Region slicer:** Dropdown filter for selecting region(s).
-   **Category slicer:** Dropdown filter for selecting product
    category/categories.
-   **Page-level Shipping Mode filter:** The saved report configuration
    currently lists **First Class** and **Second Class**.
-   Selecting a slicer value is intended to let users explore the
    dashboard within the selected data context.

**Important check:** If your assignment requires the page-level Shipping
Mode filter to be **Standard Class** and **Second Class**, update the
filter in Power BI. The currently saved PBIX configuration lists **First
Class** and **Second Class**.

### 🧾 6. Order Data Page

The second report page, **Page 2 (Order Data)**, contains a table visual
with fields such as:

-   Category and Sub Category
-   City, State and Region
-   Customer ID and Customer Name
-   Order ID and Product ID
-   Order Date and Shipping Date hierarchies
-   Product Name
-   Sales, Profit, Quantity and Discount
-   Segment and Shipping Mode

This page is intended for looking up and reviewing the detailed records
behind the summary dashboard.

------------------------------------------------------------------------

## 🛠️ Tech Stack

  -----------------------------------------------------------------------
  Tool / Feature                                Purpose
  --------------------------------------------- -------------------------
  📊 **Microsoft Power BI Desktop**             Building the report and
                                                dashboard

  🧹 **Power Query**                            Data preparation, if used
                                                in the project workflow

  💳 **Card visuals**                           Displaying Sales, Profit,
                                                Quantity and Average
                                                Discount

  📉 **Clustered bar charts**                   Comparing category sales
                                                and regional profit

  🎚️ **Slicers**                                Interactive Region and
                                                Category filtering

  🧾 **Table visual**                           Showing detailed
                                                order-level fields

  🎨 **Report theme and formatting**            Consistent visual
                                                appearance
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 📈 Results & Insights

The report is structured to help users investigate questions such as:

-   Which product categories generate the most sales?
-   Which regions generate the most profit?
-   What are the total Sales, Profit and Quantity for the current
    selection?
-   What is the average discount in the selected data?
-   How do the dashboard figures change when a Region or Category is
    selected?
-   Which individual order or product records contribute to the
    displayed results?

**Note:** Numeric KPI totals and ranked category/region results are not
included here because they depend on the report's loaded data and filter
context. Open the PBIX in Power BI Desktop to confirm the current
figures before documenting specific numerical findings.

------------------------------------------------------------------------

## 🚀 How to Use

1.  Open `PR1_kishal.pbix` in **Microsoft Power BI Desktop**.
2.  Wait for the report and data model to load.
3.  Open **Page 1 (Dashboard)** to view the KPI cards and charts.
4.  Use the **Region** and **Category** dropdown slicers to explore
    different selections.
5.  Compare the Sales by Category and Profit by Region charts.
6.  Open **Page 2 (Order Data)** to inspect the detailed order table.
7.  If the project requirements specify a different Shipping Mode page
    filter, open the Filters pane and update the page-level filter.
8.  Save the PBIX after making any required changes.

------------------------------------------------------------------------

## 🏆 Advantages

  -----------------------------------------------------------------------
  Advantage                                 Detail
  ----------------------------------------- -----------------------------
  🎯 **At-a-Glance KPIs**                   Key business measures are
                                            presented at the top level

  📊 **Visual Comparisons**                 Category sales and regional
                                            profit are easy to compare

  🎚️ **Interactive**                        Region and Category slicers
                                            allow users to explore the
                                            report

  🧾 **Detailed Records**                   A separate page supports
                                            order-level inspection

  🧩 **Business-Oriented**                  Connects summary indicators
                                            with underlying order
                                            information

  🎨 **Consistent Design**                  Uses a coordinated theme and
                                            clean dashboard layout
  -----------------------------------------------------------------------

------------------------------------------------------------------------



## 👤 Author

### Gosai Kishal

**🎓 Role:** Student \| Power BI & Data Analysis Enthusiast\
**🛠️ Skills Demonstrated:** Data visualisation · KPI reporting ·
Interactive dashboards · Filtering · Tabular reporting

> *"Good dashboards don't just show data --- they make the next question
> easier to ask."*

------------------------------------------------------------------------

## 🙏 Acknowledgements

-   **Dataset:** Sample Superstore retail dataset. If the dataset was
    downloaded from Kaggle, include the exact dataset page and creator
    here.
-   **Tool:** Microsoft Power BI Desktop.

------------------------------------------------------------------------

*Made with ❤️ and ☕ --- Last updated: 29 October, 2026*

------------------------------------------------------------------------

## 🔗 Project Files

Access the project files and related resources through the Google Drive folder:

**[Open Superstore Project Files on Google Drive](https://drive.google.com/drive/folders/1Co7PXnCz47UyvlBX7sOFOgU7RqKQYtm9?usp=drive_link)**

------------------------------------------------------------------------

## 📸 Screenshots

### Screenshot 1 — Superstore Sales Dashboard

<img width="802" height="447" alt="Screenshot 2026-10-28 214357" src="https://github.com/user-attachments/assets/c02a08e3-016d-4d7b-81ce-efb3ea829114" />


### Screenshot 2 — Order Data
<img width="1198" height="676" alt="Screenshot 2026-10-28 214445" src="https://github.com/user-attachments/assets/89c5949a-a038-4398-995a-39db26bb213c" />



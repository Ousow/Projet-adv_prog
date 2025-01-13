# Recipe Price Comparison Tool

## Project Context
This project focuses on building an application to search for recipes and compare the prices of required ingredients across various supermarkets (e.g., Auchan, Carrefour). With a wide range of products and fluctuating prices, this tool provides users with a practical way to plan their meals and optimize their grocery expenses.

The application is built on a user-friendly interface and leverages natural language processing (NLP) techniques to match recipe ingredients with products available in store catalogs.

---

## Steps Followed

### 1. Data Scraping
- **Auchan**: Extracted product details (name, price, unit, and description) from Auchan's website. The data was cleaned and normalized for usability.
- **Carrefour**: Collected similar information from Carrefour's website.
- **Marmiton (Recipe Site)**: Scraped popular recipes, including titles, ingredients, and instructions. Ingredients were pre-processed to facilitate accurate matching.

### 2. Data Processing
- **Text Cleaning and Normalization**: Removed accents, special characters, and applied lowercase transformation to standardize the data.
- **Enhancements**: Added product details such as quantities and discounts to enrich the dataset.

### 3. Model and Matching
- Implemented NLP models to compute similarities between recipe ingredients and supermarket products.
- Applied a similarity threshold to filter out weak or irrelevant matches.
- Experimented with different models to improve accuracy and reliability.

### 4. User Interface
Built an interactive application using `Tkinter`, enabling users to:
- Search for recipes by entering a title.
- View the required ingredients alongside matching products from Auchan and Carrefour.
- Compare product prices for each ingredient.

---

## How to Use the Project

### Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/your-username/your-project.git
cd your-project
pip install -r requirements.txt
```

### Running the Application
Run the main script to launch the application:
```bash
python main.py
```

### Using the Application
- Enter the title of a recipe in the search field.
- Click the "Search" button to find matches.
- View the results, including prices and product details for each ingredient.

### Preview of Recipe and Product Matching Results
This section showcases the output of the recipe-to-product matching system. The tool takes a recipe title as input, extracts its ingredients, and identifies the best-matched products from Auchan and Carrefour databases. Below is an example of the results, demonstrating how the system pairs ingredients with corresponding products, prices, and packaging units from both retailers.


![Aperçu des résultats](https://github.com/Ousow/Projet-adv_prog/blob/main/Capture%20d'%C3%A9cran%202025-01-13%20105831.png)


This example helps to illustrate how the system operates and the level of detail provided for each ingredient-to-product match.


### Current Issues and Future Improvements

#### Current Challenges
- Debugging the interface to ensure accurate product matching.
- Improving model precision for ingredient-to-product mapping.

#### Future Plans
- Test additional NLP models for better accuracy.
- Implement advanced filtering to exclude irrelevant products.
- Introduce dynamic quantity selection and promotion tracking

## Contributors
- Razafindrakoto Tsiba
- Sow Oumou

Feel free to submit issues or pull requests to improve the project! 🚀

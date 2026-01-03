<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,15,20&height=200&section=header&text=Cooking%20Assistant%20🍳&fontSize=50&fontColor=fff&animation=fadeIn&fontAlignY=38" />
</div>

<h3 align="center">Smart Recipe Checker with ML-Based Suggestions</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Tkinter-GUI-FF6B6B?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white" />
</p>

---

## Overview

**Cooking Assistant** is an intelligent desktop application that helps you determine what dishes you can cook based on your available ingredients. Using machine learning algorithms, it provides smart recipe suggestions when you're missing ingredients for your desired dish.

### Key Features

**Multi-Cuisine Support**
- Asian cuisine (Biryani, Chicken Curry, Aloo Curry, Omelette, etc.)
- Western cuisine (Pasta, Grilled Cheese, Beef Steak, etc.)
- Arab cuisine (Hummus, Falafel, Shawarma, Fattoush, etc.)

**Smart Ingredient Matching**
- Check if you can cook a specific dish with your available ingredients
- Get precise missing ingredient quantities
- Flexible unit conversion system (cups, tablespoons, teaspoons, pieces)

**ML-Powered Recommendations**
- K-Nearest Neighbors algorithm for recipe similarity
- Cosine similarity metric for ingredient matching
- Context-aware suggestions based on your current stock

**User-Friendly Interface**
- 🎨 Modern dark-themed GUI built with Tkinter
- 🌍 Cuisine-based filtering (Asian, Western, Arab)
- ⚡ Interactive ingredient input system
- ✅ Real-time availability checking

---

## Technology Stack

<div align="center">

### Core Technologies

<table>
<tr>
<td align="center" width="25%">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" /><br>
<b>Python 3.8+</b><br>
<sub>Core Language</sub>
</td>
<td align="center" width="25%">
<img src="https://img.shields.io/badge/Tkinter-FF6B6B?style=for-the-badge&logo=python&logoColor=white" /><br>
<b>Tkinter</b><br>
<sub>GUI Framework</sub>
</td>
<td align="center" width="25%">
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" /><br>
<b>scikit-learn</b><br>
<sub>ML Library</sub>
</td>
<td align="center" width="25%">
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" /><br>
<b>Pandas</b><br>
<sub>Data Processing</sub>
</td>
</tr>
</table>

### Machine Learning Architecture

<table>
<tr>
<td align="center" width="50%">
<img src="https://img.shields.io/badge/Algorithm-K--Nearest_Neighbors-00D9FF?style=for-the-badge" /><br>
<b>K-Nearest Neighbors</b><br>
<sub>Pattern Recognition Algorithm</sub>
</td>
<td align="center" width="50%">
<img src="https://img.shields.io/badge/Metric-Cosine_Distance-BB9AF7?style=for-the-badge" /><br>
<b>Cosine Similarity</b><br>
<sub>Ingredient Matching</sub>
</td>
</tr>
</table>

</div>

---

## Installation

<div align="center">

### 📋 Prerequisites

<img src="https://img.shields.io/badge/Python-3.8+-success?style=for-the-badge&logo=python&logoColor=white" />

Ensure you have Python 3.8 or higher installed on your system.

</div>

### 🚀 Setup Instructions

**Step 1: Clone the repository**
```bash
git clone https://github.com/yourusername/cooking-assistant.git
cd cooking-assistant
```

**Step 2: Install required dependencies**
```bash
pip install pandas scikit-learn
```

**Step 3: Run the application**
```bash
python cooking_assistant.py
```

<div align="center">

### ✨ That's it! Your Cooking Assistant is ready to use.

</div>

---

## How to Use

**Select Your Cuisine**
Choose from Asian, Western, or Arab cuisine using the radio buttons.

**Pick a Dish**
Select your desired dish from the dropdown menu.

**Click "Check Dish"**
View the required ingredients for the selected recipe.

**Enter Your Ingredients**
A popup window will appear where you can enter the quantities of ingredients you have available.

**Get Results**
The system will tell you if you can cook the dish or what ingredients you're missing. If you can't cook your selected dish, it will suggest alternative recipes based on your available ingredients.

---

## Project Structure

```
cooking-assistant/
│
├── cooking_assistant.py          # Main application file
├── README.md                      # Project documentation
└── requirements.txt               # Python dependencies
```

---

## Core Components

### KitchenStock Class
Manages your available ingredients and their quantities. Handles unit conversions and availability checking.

### RecipeBook Class
Stores all recipes across different cuisines. Provides normalized recipe lookup functionality.

### MLModel Class
Implements K-Nearest Neighbors algorithm for recipe similarity matching. Uses cosine distance to find recipes closest to your available ingredients.

### CookingAssistant Class
Main logic coordinator that checks recipe feasibility and generates smart suggestions.

---

## Unit Conversion System

The application supports flexible unit conversions:

**Volume Units**
- Cups (cup)
- Tablespoons (tbsp)
- Teaspoons (tsp)

**Count Units**
- Pieces (pcs)

Each ingredient has a default base unit for standardized calculations.

---

## Machine Learning Approach

**Feature Engineering**
Recipes are converted into numeric vectors where each ingredient quantity becomes a feature.

**Similarity Calculation**
Uses cosine similarity to measure how close your available ingredients are to each recipe's requirements.

**Recommendation Logic**
1. First checks for recipes you can cook completely
2. If none available, suggests recipes with highest similarity scores
3. Filters suggestions based on selected cuisine

---

## Current Recipe Database

**Asian Cuisine (6 recipes)**
Omelette, Rice, Chicken Curry, Spicy Eggs, Aloo Curry, Biryani

**Western Cuisine (5 recipes)**
Grilled Cheese, Pasta, Beef Steak, Fried Rice, Chicken Sandwich

**Arab Cuisine (5 recipes)**
Hummus, Falafel, Shawarma, Fattoush, Shakshuka

---

## Future Enhancements

**Planned Features**

- Add more recipes across different cuisines
- Implement recipe difficulty levels
- Add cooking time estimates
- Include nutritional information
- Save and load custom ingredient stock
- Recipe rating system
- Shopping list generator
- Voice input for ingredients
- Mobile application version
- Cloud-based recipe database
- User recipe submission system

**Technical Improvements**

- Database integration for recipe storage
- Advanced ML models (Random Forest, Neural Networks)
- User preference learning
- Dietary restriction filters (vegetarian, vegan, gluten-free)
- Calorie and macro tracking
- Multi-language support

---

## Contributing

Contributions are welcome! Here's how you can help:

**Add New Recipes**
Submit recipes following the existing format with accurate ingredient measurements.

**Improve ML Algorithm**
Enhance the recommendation system with better algorithms or feature engineering.

**UI Enhancements**
Improve the interface design or add new visual elements.

**Bug Fixes**
Report and fix any bugs you encounter.

### Contribution Steps

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See `LICENSE` file for details.

---

## Contact & Support

<p align="center">
<a href="https://www.linkedin.com/in/hasnain-naseer-a33036399" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="mailto:naseerhassnain981@gmail.com">
  <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>
<a href="https://github.com/hasnain89898" target="_blank">
  <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />
</a>
</p>

<div align="center">

### Show Your Support

If you find this project helpful, please give it a ⭐ on GitHub!

</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,15,20&height=100&section=footer" />
</div>

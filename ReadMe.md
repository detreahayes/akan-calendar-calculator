# 🌍 Akan Name Finder & Day Calculator

A sleek, responsive, and minimalist web application designed to help users discover their traditional Ghanaian **Akan name** (soul name), corresponding personality traits, and authentic **traditional food pairings** based on their birthdate and gender identity.

---

## 📖 Table of Contents
- [About the Project](#-about-the-project)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Akan Naming Tradition & Food Mapping](#-akan-naming-tradition--food-mapping)
- [Installation & Usage](#-installation--usage)
- [Customization](#-customization)

---

## 📝 About the Project

In the Akan culture of Ghana, children are traditionally given a "soul name" corresponding to the day of the week they were born. These names carry deep spiritual meaning, shaping a person's character traits, destiny, and cultural identity. 

The **Akan Name Finder** bridges cultural heritage with modern design. By inputting a birthdate, users can uncover their unique Akan name, the traditional traits tied to their birth day, and curated cultural culinary recommendations.

---

## ✨ Features

- **Modern West African Aesthetics:** A premium, minimalist dark mode experience accented with vibrant Ghanaian-inspired gold (`#ffb703`) and electric cyan (`#00caee`).
- **Dynamic Food Pairings:** Displays authentic traditional Ghanaian dish recommendations (like *Waakye*, *Fufu*, and *Red Red*) tied directly to your specific soul name profile.
- **Timezone-Safe Date Parsing:** Custom JavaScript parsing logic prevents common frontend date-shifting bugs, ensuring accurate day calculations regardless of the local user's timezone.
- **Fluid & Interactivity-Driven UI:** Instant dynamic calculation with smooth results reveal, form focus states, and responsive active button scaling.
- **Fully Responsive Architecture:** Optimized for a seamless experience across desktop monitors, tablets, and smartphones.

---

## ⚙️ How It Works

1. **User Selection:** The user picks a date of birth and specifies their gender identity.
2. **Day Calculation:** The app manually parses the date values (`YYYY-MM-DD`) into a local JavaScript `Date` object and invokes `.getDay()` to isolate the correct day index (0 for Sunday, 6 for Saturday).
3. **Data Hydration:** The script targets the specific day index inside `akanData` to capture matching names, trait strings, and food arrays.
4. **DOM Rendering:** The JavaScript dynamically constructs and injects standard list items (`<li>`) for the food section, updates descriptive typography, and updates the display property of the result wrapper.

---

## 💻 Technologies Used

- **HTML5:** Structuring semantic forms, selection inputs, and layout wrappers.
- **CSS3:** Built with CSS variables, Flexbox centering layout, sleek focus pseudo-classes, and native element transition animations.
- **JavaScript (ES6):** Client-side date math, object-based dictionary lookups, array iterations, and dynamic DOM manipulation.

---

## 📂 Project Structure

The codebase is organized into a clean, modular structure:
```bash
├── index.html   # Main application structure & JavaScript logic
└── style.css    # Global styling rules, dark mode layout, & theme color variables
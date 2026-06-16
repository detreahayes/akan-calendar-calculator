# 🌍 Akan Name Finder & Day Calculator

A sleek, responsive, and minimalist web application designed to help users discover their traditional Ghanaian **Akan name** (soul name) and corresponding personality traits based on their birthdate and gender identity.

---

## 📖 Table of Contents
- [About the Project](#-about-the-project)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Akan Naming Tradition Data](#-akan-naming-tradition-data)
- [Installation & Usage](#-installation--usage)
- [Customization](#-customization)

---

## 📝 About the Project

In the Akan culture of Ghana, children are traditionally given a "soul name" corresponding to the day of the week they were born. These names carry deep spiritual meaning and are believed to influence a person's character traits and destiny. 

The **Akan Name Finder** provides a beautiful, modern user interface to keep this rich cultural tradition accessible. It calculates the day of the week a user was born and dynamically reveals their custom name, the day's element, and traditional characteristics.

---

## ✨ Features

- **Modern UI/UX:** A visually striking, West African-inspired dark mode theme using rich gold (`#ffb703`) and cyan accents.
- **Accurate Day Calculation:** Custom JavaScript date parsing avoids common timezone shifting bugs often found in standard web forms.
- **Dynamic Results:** Smoothly displays the corresponding Akan name, the day of the week, and comprehensive character traits without reloading the page.
- **Fully Responsive:** Completely optimized to look stunning on desktops, tablets, and mobile devices.
- **Lightweight:** Single-file architecture (HTML/CSS/JS combined) ensures instant loading and zero external dependencies.

---

## ⚙️ How It Works

1. **User Input:** The user selects their date of birth using a native date picker and chooses their gender identity (Male/Female).
2. **The Calculation:** When clicking **"Discover My Name"**, JavaScript parses the date string components explicitly to retain local time integrity and utilizes the `.getDay()` method to get an index mapping (0 for Sunday, 6 for Saturday).
3. **Data Retrieval:** The script cross-references the index with a structured dictionary storing names and definitions.
4. **DOM Manipulation:** The template unhides the result card and updates the fields dynamically.

---

## 💻 Technologies Used

- **HTML5:** Semantic structure for user forms and container wrappers.
- **CSS3:** Custom properties (CSS variables), Flexbox layouts, transition states, and responsive box-shaping.
- **JavaScript (ES6):** Client-side form handling, timezone-safe date parsing, object mapping, and DOM manipulation.

---

## 📊 Akan Naming Tradition Data

The application maps data based on the following cultural framework embedded in the source code:

| Day | Male Name | Female Name | Association & Traits |
| :--- | :--- | :--- | :--- |
| **Sunday** | Kwasi | Akosua | **Sun:** Natural leaders, resilient, highly respected. |
| **Monday** | Kojo | Adwoa | **Peace:** Calm, rational, protectors, deliberate thinkers. |
| **Tuesday** | Kwabena | Abenaa | **Ocean:** Fierce, friendly, compassionate, highly driven. |
| **Wednesday** | Kwaku | Akua | **Motherhood/Tenacity:** Strategic, sharp-witted, problem-solvers. |
| **Thursday** | Yaw | Yaa | **Earth:** Courageous, resolute, deeply loyal. |
| **Friday** | Kofi | Afia | **Fertility/Creation:** Dynamic, creative, wanderers, expressive. |
| **Saturday** | Kwame | Ama | **God/Creation:** Responsible, ancient souls, spiritual, enduring. |

---

## 🚀 Installation & Usage

Because this project is built entirely on standard frontend web technologies, it requires no installation, compilers, or local servers.

### Run Locally:
1. Clone this repository or copy the code into a local file named `index.html`.
2. Double-click the `index.html` file to open it directly in any modern web browser (Chrome, Safari, Firefox, Edge).

---

## 🎨 Customization

You can easily adapt the styling or data elements directly in the file:
- **Change Colors:** Modify the CSS variables inside the `:root` block to update the background, cards, or theme accents:
  ```css
  --accent-gold: #ffb703; /* Edit this to change your primary accent color */
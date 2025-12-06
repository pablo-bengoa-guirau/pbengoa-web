# Practical Work II: Personal Website - Pablo Bengoa Guirau

**Degree:** Computer Engineering (UFV)  
**Course:** Fundamentals of Computer Engineering (2025/26)  
**Student:** Pablo Bengoa Guirau  
**Repository:** [Link a tu repo público aquí]  
**Deployed Site:** [Link a tu web publicada en GitHub Pages aquí]  
**Acknowledgments:** Special thanks to **Gemini** for assistance with the README structure and formatting.

---

## 1. Description of the work
The goal of this project is to develop a personal academic website to demonstrate proficiency in HTML5, CSS3, and Version Control. The project follows a structured software development process:

1.  **Design Analysis & Inspiration:** Before writing code, I researched high-profile software engineering portfolios. I selected **Brittany Chiang** (https://brittanychiang.com/) as my primary visual reference. I aimed to replicate her minimalist "Dark Navy" aesthetic and "monospaced" styling for technical details, adapting it to my own code structure to achieve a professional look suitable for the industry.
2.  **Environment Setup:** I organized the project using a specific directory structure (`docs/` as the root for deployment), separating styles (`css`), assets (`images`), and content pages (`public`).
3.  **Core Development:** I focused on creating a reusable layout (Header, Navigation, and Footer) to maintain consistency across all pages.
4.  **Content Implementation:** Finally, I developed the specific sections required by the assignment (`About`, `Degree`, `Net`, `Contact`) integrating the content with the defined style.

### 1.1 Design Decisions
To achieve a professional and coherent aesthetic, I defined a Design System using CSS Variables:

* **Color Palette:**
    * **Background:** `#0a192f` (Dark Navy) - Reduces eye strain and provides high contrast.
    * **Typography:** `#ccd6f6` (Lightest Slate) for headings and `#8892b0` (Slate) for body text.
    * **Accent:** `#64ffda` (Green Teal) - Used for links and interactive elements to guide user attention.
* **Typography:** Selected a Sans-Serif font stack (`Segoe UI`, `Roboto`) to ensure readability and a modern look across different operating systems.

### 1.2 Development Log

* **Update 1 (mainly index.html):**
    * **Basic Structure:** I created the basic structure of `index.html` to place the necessary information first, before starting with CSS or other subpages.
    * **Class Tweaks:** I tweaked some CSS classes to give them more specific names.
    * **Main Section:** I significantly modified the `<main>` section, organizing it into different subsections and adding bold text for emphasis.
    * **Footer:** Finally, I modified the footer with classes to include several sections and give it a more professional look.

* **Update 2 (CSS start & Documentation):**
    * **Comments:** I added some comments in `index.html` to explain the code better.
    * **README:** I improved and updated the `README.md` structure.
    * **CSS Start:** I started the `style.css` file. I added the typical reset (margin 0, padding 0), defined the color palette and fonts. I also applied the background color and text styles to the body and headers. But there is a lot to imrpove and to update in the css.

* **Update 3 (Full Design & Layout):**
    * **Sticky Footer:** I fixed the footer position by applying `min-height: 100vh` to the body and `flex: 1` to the main content, ensuring it always stays at the bottom of the page.
    * **Header & Nav:** I completed the header styling, aligning my name and the navigation menu horizontally using Flexbox and adding hover effects to the links.
    * **Main Styling:** I styled the introduction and project info sections, adjusting font sizes and margins for better readability.
    * **Skills List:** I customized the skills list with a dark background color and specific "monospace" styling to give it a technical look, including custom arrow markers (`▹`).

---

## 2. Problems during development
*(This section serves as a development log. I will update it as I encounter and solve issues).*

### [06/12/2025] - Issue: Sticky Footer Positioning
* **Problem:** The footer was not sticking to the bottom of the viewport on pages with little content; instead, it appeared in the middle of the screen immediately after the content ended, leaving empty space below.
* **Solution:** I applied a Flexbox layout to the `body` element (`display: flex`, `flex-direction: column`, `min-height: 100vh`) to ensure the page always takes up the full height of the screen. Then, I added `flex: 1` to the `.main-content` container to make it expand and push the footer to the bottom.


---

## 3. Conclusions
*(To be filled upon project completion)*

* **Learning Outcomes:** (What did you learn about Git? About structuring HTML? About the Box Model?)
* **Future Improvements:** (If you had more time, what would you add? JS animations? A backend?)
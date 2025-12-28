# Practical Work II: Personal Website - Pablo Bengoa Guirau

**Degree:** Computer Engineering (UFV)  
**Course:** Fundamentals of Computer Engineering (2025/26)  
**Student:** Pablo Bengoa Guirau  
**Repository:** https://github.com/pablo-bengoa-guirau/pbengoa-web

**Deployed Site:** https://pablo-bengoa-guirau.github.io/pbengoa-web
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
    * **Accent:** `#31d1ac` (Bright Teal) - Used for links and interactive elements to guide user attention.
* **Typography:** I selected a unique font combination to differentiate the portfolio:
    * **Headings & Navigation:** "Zalando Sans Expanded" for a strong and modern brand presence.
    * **Body Text:** "Playpen Sans Deva" for readability with a personal touch.
    * **Technical Details:** "Bitcount Grid Double" (Monospace) to provide a retro-tech aesthetic to specific elements like credits and skills.

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

* **Update 4 (Typography & CSS Refactor):**
    * **Google Fonts:** I imported new fonts from Google Fonts (Zalando Sans, Playpen Sans, Bitcount Grid) to give the website a unique and better look.
    * **CSS Reorganization:** I completely reorganized the `style.css` file. I switched to using CSS variables (`:root`) for the fonts to fix the mess of having them hardcoded everywhere. Now it's much cleaner and easier to change.
    * **Comments:** I added new comments throughout the CSS to explain what each section does.
    * **Completion:** With these changes, the website aesthetic is now standardized, and the `index.html` is fully finished.

* **Update 5 (Site Structure Expansion):**
    * **Subpage Creation:** I created the skeleton files for the main navigation sections (`about.html`, `degree.html`, `net.html`, `topic.html`, `contact.html`) inside the `public/` directory.
    * **Template Inheritance:** I used the finished `index.html` as a master template to ensure visual consistency (header, footer, fonts) across all pages.
    * **Path Configuration:** I configured relative paths (`../`) in the new pages to correctly link back to the CSS and the Home page.
    * **Active States:** I implemented the `active` class in the navigation menu for each page to highlight the user's current location.

* **Update 6 (About Me Page & Asset Organization):**
    * **Content Strategy:** I developed the `public/about.html` page, focusing on a "human-centric" profile that combines academic goals with personal values, as suggested by the FCE syllabus.
    * **CSS Refactoring:** I moved away from inline styles to a cleaner class-based approach in `style.css`. I implemented the `.bio-simple` class using Flexbox to align the profile picture and text responsively.
    * **Asset Management:** I created a new `docs/files/` directory to professionally host static documents like my CV (`cv_pablo.pdf`).
    * **Interactive Design:** I designed a "Ghost Button" for the resume and a minimalist text-based social media menu. Both elements use a "neon glow" hover effect (using `text-shadow` and `box-shadow`) to maintain consistency with the main navigation bar.
    * **AI Collaboration:** I worked closely with **Gemini** to brainstorm and finalize semantic class names (such as `.bio-simple` and `.social-simple`), ensuring the code is readable and maintainable.

* **Update 7 (Contact Page Implementation):**
    * **Academic Compliance:** I developed the `public/contact.html` page strictly following the guidelines from **Unit 4 (HTML)**. Specifically, I implemented the form structure using an **unordered list (`<ul>`)**, as demonstrated in the course slides (Slide 26), ensuring the code adheres to the taught standards.
    * **Visual Design:** I styled the form using a simplified CSS class (`.form-basic`) to maintain the "Dark Navy" aesthetic. I focused on usability by ensuring high contrast between text and input fields.
    * **CSS Logic:** To center the submit button without adding extra `div` wrappers, I used the `:last-child` pseudo-selector on the list item, keeping the HTML clean and semantic.
    * **Functionality:** As per the assignment requirements ("no scripting elements"), the form is purely visual and does not execute backend actions.

* **Update 8 (Network Page Implementation):**
    * **Connectivity:** I developed the `public/net.html` page to fulfill the requirement of linking to partner pages. I implemented a semantic **HTML Table** to organize the student names and project links clearly.
    * **Integration:** I successfully integrated valid links to external classmates' repositories, verifying that the `target="_blank"` attribute works correctly to open pages in new tabs.
    * **Styling:** I applied specific CSS styles (`.partners-table`) to ensure the table matches the dark aesthetic of the site, including hover effects on rows for better user interaction.
    
* **Update 9 (Topic Page Implementation):**
    * **Content Integration:** I developed the `public/topic.html` page focusing on **Ethical Hacking for SMEs**. I utilized Gemini AI to summarize and structure the extensive PDF report into a concise web format, ensuring the technical accuracy of the "Prevention, Detection, and Response" cycle.
    * **Code Efficiency:** To adhere to "Clean Code" principles, I avoided creating redundant CSS. I intelligently **reused** existing classes like `.partners-table` and `.skills-list` to style the vocabulary tables and technical lists, ensuring visual consistency across the website.
    * **Attribution:** I included proper credits to the original authors (Group 5) and the AI assistance for the summary, fulfilling the academic integrity requirements of the project[cite: 5, 26].

* **Update 10 (Degree & FCE Implementation):**
    * **Curriculum Mapping:** I completed the `public/degree.html` page, organizing the full 4-year curriculum into semantic tables. I corrected the semester numbering (1-2 per year) to reflect the university structure accurately.
    * **Subject Deep Dive:** I developed a dedicated page (`public/fce.html`) for *Fundamentals of Computer Engineering*. I analyzed the 10 course units and structured them into 5 distinct modules (Context, Core, Data, Software Dev, and Web Programming) to demonstrate a complete understanding of the syllabus.
    * **Visual Consistency:** I reused the `.partners-table` and `.skills-list` classes to ensure the academic content matches the dark, professional aesthetic established in previous updates, maintaining code maintainability.

* **Update 11 (Personal Branding & Final Polish):**
    * **About Me Refinement:** I revamped `public/about.html` to include a specific section on **Resilience & Discipline**.
    * **Visual Storytelling:** I integrated images from my **Camino de Santiago** experience (150km in 7 days). This addition serves to visually demonstrate core soft skills—persistence and mental endurance—connecting my physical achievements with my engineering mindset.
    * **Layout Refinement:** Fine-tuned the image distribution in the `about.html` section to maintain visual balance between the profile picture and the new gallery, ensuring correct alignment.

---

## 2. Problems during development
*(This section serves as a development log. I will update it as I encounter and solve issues).*

### [06/12/2025] - Issue: Sticky Footer Positioning
* **Problem:** The footer was not sticking to the bottom of the viewport on pages with little content; instead, it appeared in the middle of the screen immediately after the content ended, leaving empty space below.
* **Solution:** I applied a Flexbox layout to the `body` element (`display: flex`, `flex-direction: column`, `min-height: 100vh`) to ensure the page always takes up the full height of the screen. Then, I added `flex: 1` to the `.main-content` container to make it expand and push the footer to the bottom.

### [08/12/2025] - Issue: Skills List Layout
* **Problem:** The items in the skills summary (Semantic HTML, CSS, Git) were displaying inline without proper vertical spacing, making the text difficult to read.
* **Solution:** I identified that a `display: flex` property was incorrectly applied to the `.skills-list` container. I removed this property to restore the standard block layout, ensuring each paragraph appears on a new line with the correct spacing. 

### [08/12/2025] - Issue: Font Management Chaos
* **Problem:** I started adding specific font families manually to each section (header, footer, links...), and the code became very messy. It was difficult to know which font was being used where, and changing them was a nightmare.
* **Solution:** I optimized the CSS by organizing the typography into variables (`:root`). I created specific variables like `--font-principal` and `--font-puntos`, applied them globally, and removed the hardcoded fonts from individual classes.

### [28/12/2025] - Issue: Image Layout & Alignment
* **Problem:** When adding the new personal images (Camino & Sports) to the `about.html` page, they stacked vertically or broke the text flow, creating an unbalanced and messy layout compared to the "Bio" section.
* **Solution:** I implemented a nested Flexbox structure. I grouped the profile picture and the new gallery into a single left-column container with a specific width.

---

## 3. Conclusions

This project has been a comprehensive journey into the foundations of web development and software engineering. Beyond simply writing code, I have learned to:

* **Learning Outcomes:**
    * **Git Workflow:** I moved from understanding Git as simple storage to using it as a professional development tool. I learned the importance of "atomic commits" to document the history of changes rather than just saving the final result.
    * **Semantic Structure:** I learned that HTML is about meaning, not just display. Using proper tags (`<section>`, `<table>` for data, `<footer>`) creates a structure that is accessible and easier to maintain.
    * **CSS Architecture:** By using CSS Variables (`:root`) and the Box Model, I created a consistent "Dark Mode" design system.
    * **Holistic Engineering:** The website successfully connects technical subjects (FCE, Coding) with personal growth and soft skills, reflecting the university's human-centric approach.

* **Future Improvements:**
    * **Backend Integration:** If I had more time, I would implement a server-side script to make the contact form fully functional for real email submissions.
    * **JavaScript Interactivity:** I would add JavaScript to create a dynamic menu for better mobile navigation and smooth scrolling effects between sections.

# capstone-project-redo-part2-3

# part 2 #
Design Decisions

1. Minimal and Clean Layout

The interface uses a simple, neutral design so the focus stays on the astronomy images. Generous spacing and a single-column layout make the UI easy to scan.

2. Clear Information Structure

Content is grouped into three main sections: Search, Result, and Favourites. Each section includes a title and description to guide the user. Empty-state messages (“No result yet…”) help users understand what to do next.

3. Consistent Card Components

Favourites are displayed using uniform cards with image, title, date, and buttons. This creates a coherent look and makes content easy to browse.

4. Accessible Interaction

Buttons like Get APOD, View, and Delete are high-contrast and large enough for comfortable clicking. The blue CTA highlights important actions.

5. User-Flow Driven Layout

The layout follows a natural flow: choose a date → view result → manage favourites. This reduces cognitive load and aligns with user expectations.

6. Neutral Colour Palette

Light grey backgrounds with dark text create readability, while a blue accent colour draws attention to key actions without overpowering the images.

7. Transparent Data Source

A footer note (“Data from NASA APOD API”) maintains clarity about where the information comes from and aligns with API usage requirements.

# part 3 #
Development Report

Overview
This report outlines the key steps taken to create the APOD Search prototype, the resources used throughout the development process, and the challenges encountered while completing the prototype.

1. Steps Taken to Create the Prototype

1.1 Initial Planning & Wireframing
I began by analysing the functional requirements of the APOD Search app: selecting a date, displaying the NASA APOD result, and saving/deleting favourites.
Using the mockups (see PDF), I established a clean, card-based layout with three main sections: Search, Result, and Favourites. These wireframes guided the structure of the final HTML layout.

1.2 Building the HTML Structure
I created a semantic and accessible HTML layout, including:
Header with title and description
A form for selecting a date
A dynamic result container
A favourites section
Footer that credits NASA APOD API
ARIA labels and live regions were added to enhance accessibility and dynamic updates.

1.3 Styling the Interface (CSS)
I implemented the design using a custom CSS stylesheet, focusing on:
A light, minimal colour palette
Card components with soft shadows
Responsive grids for favourites
Styled actions (primary / secondary buttons)
Smooth hover transitions
CSS variables were used to keep the design consistent and easy to update.

2. Resources Used

2.1 Development Tools
HTML, CSS, JavaScript (hand-coded)
Browser DevTools for debugging
Local storage API for persistent favourites

2.2 External Resources
NASA APOD API (official public API used for image and metadata retrieval)
MDN Web Docs (reference for form validation, fetch API, ARIA attributes)
W3C Accessibility Guidelines (structure + ARIA practices)

2.3 Design References
My mockups from the PDF (layout, typography, card components)
Modern minimalist UI patterns for search-based interfaces

3. Challenges Encountered
3.1 Handling API Limitations
Some dates return non-image APOD entries (e.g., videos).
I added a conditional message to inform users when the media type is unsupported.

3.2 Ensuring Accessibility
I had to carefully structure ARIA roles and live regions so that results and error messages update correctly for screen readers.

3.3 Favourites Data Handling
Managing localStorage required additional logic to prevent duplicates, keep the UI in sync, and properly render/delete items.

3.4 Responsive Layout Adjustments
The favourites grid needed refining to display well across different screen sizes.
Media queries were added to keep the design consistent on mobile.

Conclusion
The prototype successfully demonstrates the core functionality of the APOD Search application. Through structured planning, careful UI design, and the use of HTML/CSS/JS alongside the NASA APOD API, I created a functional and visually consistent interface. Despite challenges involving API handling, accessibility, and responsive design, the final version reflects a clear and user-friendly prototype.
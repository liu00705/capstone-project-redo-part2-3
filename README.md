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
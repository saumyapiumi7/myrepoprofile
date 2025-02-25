

# Responsive Navbar with Active Button Underline Effect

This project is a simple, responsive navbar that dynamically loads content from external HTML files and displays an underline effect on the active navigation button. The underline visually indicates which page is currently active.

## Features

- **Responsive Design:** The navbar adapts to different screen sizes (desktops, tablets, and mobile devices).
- **Dynamic Content Loading:** Content is loaded dynamically using the Fetch API.
- **Active Button Styling:** The currently active button gets an underline effect to help users identify the active page.
- **Footer Loading:** The footer content is loaded dynamically from a separate HTML file.

## Preview
(Capture.PNG)

## Demo 
(video.mp4)


## How It Works

- **Dynamic Navigation:**
  - Each navigation button uses the `onclick` attribute to call the `navigateTo()` function.
  - The function fetches the respective HTML file (e.g., `hero.html`, `about.html`) and loads it into the main content container.
  - The active button is highlighted with an underline effect using CSS by adding an `active` class.

- **Footer Loading:**
  - The `loadFooter()` function fetches `footer.html` and inserts its content into the footer placeholder.
  - Both content loading and footer loading happen during the initial page load.

- **Responsive Design:**
  - CSS media queries adjust the layout of the navbar for tablets and mobile devices.
  
## How to Run

1. **Clone the repository** or download the project files.
2. **Open the `header.html` file** in your browser. The page will load `hero.html` by default, and the "Home" button will be highlighted with an underline.
3. **Click the navigation buttons** to load different sections of the website dynamically.

## Code Overview

### HTML
- **Navbar Buttons:** Each button is set up to call the `navigateTo()` function with its corresponding page and button reference.
- **Dynamic Content Section:** A `div` with the id `main-content` is used to load the HTML content.
- **Footer Section:** A placeholder `div` for loading the footer content dynamically.

### CSS
- **Common Button Styles:** Includes default styling for buttons.
- **Active Button Styling:** An `.active` class adds an underline to the active button.
- **Responsive Media Queries:** Adjust layout and styling for different screen sizes.

### JavaScript
- **`navigateTo(page, btnElement)`:** Fetches content from the specified page, updates the main content area, and applies the active class to the clicked button.
- **`loadFooter()`:** Fetches and displays the footer content.
- **`window.onload`:** Loads the default page (`hero.html`) and the footer on page load.

## Customization

- **Styling:** You can adjust the CSS to match your design preferences.
- **Content:** Replace the contents of `hero.html`, `about.html`, `work.html`, `contact.html`, and `footer.html` with your own content.
- **JavaScript:** Further functionality can be added as needed.

## License

This project is open-source and free to use. Feel free to modify it as per your requirements.


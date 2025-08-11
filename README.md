# Live Code Editor

A simple, browser-based code editor for real-time HTML, CSS, and JavaScript development. This project provides a clean interface with separate input areas for each language and an immediate output preview, making it an excellent tool for web development beginners and for quickly testing code snippets.

## Features

-   **Live Preview**: Instantly see the rendered output of your code as you type.
-   **Split-Screen Interface**: Separate, clearly labeled text areas for HTML, CSS, and JavaScript.
-   **Real-time Updates**: The `onkeyup` event triggers an immediate refresh of the output `iframe`.
-   **No Backend Required**: Runs entirely on the front-end using vanilla JavaScript.
-   **Simple & Lightweight**: Minimal code and easy to understand, modify, or embed.

## How to Use

1.  Clone or download this repository.
2.  Open the `index.html` file in your web browser.
3.  Start writing your code:
    -   Place your HTML structure in the **HTML** box.
    -   Add your styles to the **CSS** box.
    -   Write your scripts in the **JavaScript** box.
4.  The **Output** panel will automatically update to show the result of your code.

## Technologies Used

-   **HTML5**: For the structure of the editor.
-   **CSS3**: For styling the editor layout.
-   **JavaScript**: For capturing user input and dynamically updating the output `iframe`.

## How It Works

The core functionality is powered by a single JavaScript function, `runCode()`. This function:
1.  Retrieves the content from the HTML, CSS, and JavaScript `<textarea>` elements.
2.  Wraps the CSS content in `<style>` tags and the JavaScript content in `<script>` tags.
3.  Concatenates the HTML, CSS, and JS strings.
4.  Assigns the combined string to the `srcdoc` attribute of the output `iframe`, which causes the browser to render the content.

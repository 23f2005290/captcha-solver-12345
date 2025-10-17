# Captcha Solver Demo

This is a simple single-file web application designed to demonstrate a user-facing interface for solving captchas. It's built with HTML, JavaScript, and styled using Tailwind CSS for a modern, responsive design.

## Features

*   **Dynamic Image Loading:** Displays a captcha image either from a local file (`sample.png`) or a remote URL provided via a query parameter (e.g., `index.html?url=https://example.com/captcha.png`).
*   **User Input:** Provides an input field for the user to type the text they perceive in the captcha image.
*   **Client-Side Validation:** For the default `sample.png` image, it validates the user's input against a hardcoded solution ("ADCR3").
*   **Responsive Design:** Uses Tailwind CSS to ensure a good user experience across various screen sizes.

## How to Use

1.  **Clone or Download:** Get the `index.html`, `README.md`, and `LICENSE` files.
2.  **Open `index.html`:** Simply open the `index.html` file in your web browser.

    *   It will default to displaying the `sample.png` image.
    *   Enter "ADCR3" (case-insensitive) into the input field and click "Submit" to see a "Correct!" message.
    *   Any other input will result in an "Incorrect!" message.

3.  **Load Custom Captcha Image:** To load an image from an external URL, append a `?url=` query parameter to your `index.html` path.

    *   **Example:** `file:///path/to/your/index.html?url=https://www.google.com/recaptcha/api2/payload?p=...` (replace with an actual captcha image URL if available).
    *   When an external URL is used, the application will display the image and allow you to submit text, but it will not perform client-side validation (as the correct answer for an arbitrary image is unknown without a backend or advanced OCR). It will simply acknowledge your submission.

## Technologies Used

*   **HTML5:** Structure of the web page.
*   **Tailwind CSS:** For styling and responsiveness.
*   **JavaScript:** For dynamic image loading and client-side form handling.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.

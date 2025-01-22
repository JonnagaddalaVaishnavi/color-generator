# Mini Color Changer

## Description
This project is a simple web application that allows users to change the color of either the background or the text of a specified element on the page.

## Features
- **Select Element**: Choose to change either the background or text color.
- **Color Picker**: Select a color using a color picker.
- **Apply Color**: Apply the selected color to the chosen element.

## Technologies Used
- **HTML**
- **CSS**
- **JavaScript**

## Getting Started

### Prerequisites
- A web browser to run the application.

### Running the Application
1. Clone the repository:
    ```sh
    git clone https://github.com/JonnagaddalaVaishnavi/color-generator.git
    ```
2. Navigate to the project directory:
    ```sh
    cd color-generator
    ```
3. Open `index.html` in your preferred web browser to view and use the application.

## File Structure
- `index.html`: The main HTML file containing the structure of the web application.
- `style.css`: The CSS file for styling the web application.
- `app.js`: The JavaScript file containing the logic for changing colors.

## Usage
1. Open the application in a web browser.
2. Select the element you want to change (Background or Text) from the dropdown menu.
3. Choose a color using the color picker.
4. Click the "Apply Color" button to change the color of the selected element.

## Code Explanation
The main functionality of the application is implemented in the `changeColor` function in `app.js`:

```javascript
function changeColor() {
    var selectedElement = document.getElementById('elementSelector').value;
    var newColor = document.getElementById('colorPicker').value;

    var elementToChange = document.body; 
    if (selectedElement === 'background') {
        elementToChange = document.body;
    } else if (selectedElement === 'text') {
        elementToChange = document.getElementById('colorChangerApp');
    }

    elementToChange.style.backgroundColor = newColor;
}
## Screenshots
Here are some screenshots of the application in action:

### Initial Screen
![Mini Color Changer Initial](images/Screenshot_2025-01-22_180151.png)

### Background Color Change
![Background Color Change](images/Screenshot_2025-01-22_180151.png)

### Text Color Change
![Text Color Change](images/Screenshot_2025-01-22_180151.png)


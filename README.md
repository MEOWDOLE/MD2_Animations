## Features
- **Instant Mood Changes:** Switch to custom moods effortlessly.
- **Character Animations:** Trigger animations like picking up gifts and leveling up.

## How to Use the Tool

To use the tool in MovieStarPlanet 2, follow these steps:

1. **Open** [MovieStarPlanet 2](https://moviestarplanet2.com).
2. **Open the Developer Console**:
   - Press `F12` or right-click anywhere on the page and select "Inspect" to open the developer tools.
   - Navigate to the "Console" tab.
3. **Copy and paste the following code** into the console:

```javascript
fetch('https://raw.githubusercontent.com/MEOWDOLE/MD2_Animations/refs/heads/main/script.js')
    .then(response => {
        if (!response.ok) {
            throw new Error('Network response was not ok');
        }
        return response.text();
    })
    .then(scriptContent => {
        console.log('Executing script content:');
        console.log(scriptContent);
        eval(scriptContent);
    })
    .catch(error => {
        console.error('There was a problem with the fetch operation:', error);
    });

```

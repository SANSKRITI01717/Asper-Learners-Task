# Bug Report

## Bug 1: JavaScript "null" error
**Bug:**  
The console was showing an error: `Cannot read properties of null`, and the JavaScript was not working.

**Why it happened:**  
The JavaScript file was linked inside the `<head>` section, so it was loading before the HTML elements were created.

**How I fixed it:**  
I moved the script tag to the bottom of the HTML file, just before the closing `</body>` tag.


## Bug 2: Register button was not clickable
**Bug:**  
The "Register Now" button was visible on the page but could not be clicked.

**Why it happened:**  
In the CSS, the button had a negative `z-index`, which placed it behind other elements.

**How I fixed it:**  
I commented the negative `z-index` so the button became clickable.


## Bug 3: Spots counter was not decreasing
**Bug:**  
The available spots counter was increasing instead of decreasing when a user registered.

**Why it happened:**  
The counter logic was using addition instead of subtraction.

**How I fixed it:**  
I corrected the logic to subtract 1 from the spots counter on each registration.


## Bug 4: Submit button was not triggering alert
**Bug:**  
Clicking the submit button inside the form did not show the confirmation alert.

**Why it happened:**  
The button type was set incorrectly, so the form submit event was not triggered.

**How I fixed it:**  
I changed the button type to `submit` so the form submission event works correctly.
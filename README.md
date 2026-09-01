# Password Strength Checker & Security Awareness Tool

A client-side web application for studying password-strength concepts and giving users immediate feedback about password composition.

The project runs entirely in the browser and does not send entered passwords to a server.

## What I Implemented

* Real-time password analysis
* Checks for length, uppercase letters, lowercase letters, numbers, and special characters
* A score from 0 to 100 based on the implemented requirements
* Weak, medium, and strong UI states
* Feedback for missing password requirements
* Checks for selected common weak password patterns
* Password entropy estimation
* Educational crack-time estimates
* Password visibility controls
* A 16-character password generator
* Fisher-Yates shuffling for generated characters
* Accessible progress information and DOM updates

## What I Learned

This project helped me understand that password strength cannot be described by one simple rule.

I learned how password length and possible character sets relate to entropy and why increasing the search space makes brute-force guessing harder.

I also learned the difference between an educational strength estimate and a real security guarantee. The crack-time values in this application are heuristics. They do not measure the speed of a real password-cracking system.

Keeping the entire checker client-side also taught me a basic data-minimization principle: sensitive input does not need to leave the browser when the calculation can happen locally.

From the JavaScript side, I practiced regular expressions, DOM events, dynamic UI updates, array operations, and the Fisher-Yates shuffle.

## What This Project Demonstrates

* Basic password-security concepts
* Password entropy concepts
* Regular expressions
* Client-side input analysis
* DOM manipulation
* Event handling
* User feedback based on validation rules
* Fisher-Yates shuffling

## Tech Used

* HTML
* CSS
* Vanilla JavaScript

## Important Limitations

The crack-time display is an educational estimate, not a cryptographic measurement.

The password generator currently uses `Math.random()`. That makes it suitable for demonstrating the generation logic, but it should use the Web Crypto API for security-sensitive password generation.

## Running the Project

Open `index.html` in a browser. No package installation or server is required.

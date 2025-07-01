# Travel-Itinerary-Maker

Travel Itinerary Maker
This is a web application that helps users generate personalized travel itineraries based on their selected destination and interests. It leverages the power of the Gemini API for intelligent itinerary generation and integrates with Firebase Firestore for saving and managing user-specific travel plans.

🧠 Concept
The core idea is to simplify trip planning:

Select your City/Country: Choose from a curated list of Indian destinations.

Select your Interests: Pick specific interests (e.g., Nature, Food, Culture) or select "All" for a diverse plan.

Specify Trip Details: Define the duration, start date, number of travelers, and budget level.

Auto-Generate Itinerary: The application automatically creates a day-by-day travel itinerary tailored to your preferences.

🛠️ Features
Location Selection: Dropdown with a comprehensive list of popular Indian cities/regions.

Interest-Based Planning: Select from various interests like "Culture & History," "Food & Culinary," "Nature & Outdoors," "Adventure Sports," "Relaxation & Wellness," "Shopping & Fashion," "Art & Museums," "Nightlife & Entertainment," "Family Friendly," "Budget Travel," "Luxury Travel," or "All" for a broad itinerary.

Customizable Trip Duration: Set the number of days for your trip (1 to 14 days).

Detailed Trip Information: Input fields for Start Date, Number of Travelers, and Budget Level.

AI-Powered Itinerary Generation: Utilizes the Gemini API to create a day-by-day plan, including themes, activities, places, and tips.

"Surprise Me!" Mode: Generates a completely random trip plan by selecting a random location, interests, duration, start date, number of travelers, and budget.

Save Itineraries (Firestore): Authenticated users can save their generated itineraries to Firestore for future access.

Load Saved Itineraries (Firestore): View and load previously saved itineraries from a dedicated section.

Edit Itinerary: The generated itinerary output is editable, allowing users to make manual adjustments.

Save Edited Itinerary: Save any manual edits made to the itinerary back to Firestore.

Export as PDF: Download your complete itinerary as a PDF document for offline viewing or printing.

Share via QR Code: Generate a QR code containing the itinerary data, which can be scanned to easily share the plan.

User ID Display: Shows the current user's unique ID for reference, useful for collaborative scenarios or debugging.

Responsive Design: The user interface is designed to be fully responsive and work well on various device sizes.

Custom Modals: Uses custom modals for loading indicators, messages, and QR code display instead of native browser alerts.

🧰 Tech Stack
Frontend:

HTML5: Structure of the web application.

Tailwind CSS: Utility-first CSS framework for rapid and responsive styling.

JavaScript (ES6+): Core logic, DOM manipulation, and API interactions.

APIs & Libraries:

Gemini API (gemini-2.0-flash): For intelligent, structured itinerary generation.

Firebase (Authentication & Firestore):

firebase/app: Core Firebase SDK.

firebase/auth: Handles user authentication (anonymous or custom token).

firebase/firestore: NoSQL cloud database for saving and loading itineraries.

jsPDF: JavaScript library for generating PDF documents client-side.

html2canvas: (Used by jsPDF) For rendering HTML elements to a canvas, enabling PDF conversion.

qrcode.js: For generating QR codes from text data.

Fonts:

Inter: Modern, highly legible font from Google Fonts.

How to Use
Select Location: Choose your desired Indian city or region from the "Select Location" dropdown.

Select Interests: Choose your travel interests from the "Select Interests" dropdown. You can pick a specific interest or "All" for a mix.

Set Duration: Enter the number of days for your trip.

Enter Details: Provide the "Start Date," "Number of Travelers," and "Budget Level."

Generate Itinerary: Click the "Generate Itinerary" button. A loading spinner will appear, and your personalized itinerary will be displayed in the "Your Trip Itinerary" section.

Surprise Me!: Click this button to have the app randomly select all input fields and generate an itinerary.

Save Itinerary: After generation, click "Save Itinerary" to store your plan in your personal Firestore collection.

Load/Delete Saved: Use the "My Saved Itineraries" section to load or delete your previously saved trips.

Edit Itinerary: Click "Edit Itinerary" to make direct changes to the displayed plan. Use "Save Edited" to commit changes or "Cancel Edit" to revert.

Export PDF: Click "Export as PDF" to download a PDF version of the currently displayed itinerary.

Show QR Code: Click "Show QR Code" to display a QR code that encodes the itinerary data, allowing for easy sharing.

💡 Future Enhancements
Google Static Maps Integration: Enhance the itinerary display by including small map previews for each activity, utilizing Google Maps Static API (requires a valid API key and LLM to provide latitude/longitude).

Advanced Editing Features: Implement more structured editing capabilities for the itinerary (e.g., drag-and-drop reordering of activities, dedicated input fields for editing details).

User Accounts & Sharing: Develop more robust user account management beyond anonymous sign-in, enabling explicit sharing of itineraries between users.

User Feedback & Ratings: Allow users to provide feedback on generated itineraries or rate specific places/activities.

Cost Estimation: Integrate a basic cost estimation feature based on budget level and activities.

Local Weather Integration: Display weather forecasts for the selected travel dates and location.

# Inventory Tracker – Project Three Artifact

## Inventory Tracker GitHub Path
https://github.com/MikeBrownSNHU/CS-360/tree/main/Module-7

## Project Summary

The goal of this project was to design and develop a fully functional Android mobile application that allows users to manage inventory items locally on their devices. The application supports user authentication, persistent data storage using SQLite, full CRUD operations (create, read, update, delete), and optional SMS alerts when an item reaches zero quantity.

This app was designed to address the need for a simple, lightweight inventory management solution that doesn't require a cloud account. Users can log in, track items, update quantities, and receive optional notifications, all within a clean and straightforward interface.


## Screens, Features, and User-Centered Design

To support user needs, the following screens and features were implemented:

- Login and account creation screen
- Inventory list screen (grid-style layout)
- Add item screen
- Item detail screen (update quantity and delete item)
- SMS notification settings screen

The UI was designed with clarity and usability in mind. Each screen focuses on one primary task to avoid overwhelming the user. Navigation between screens follows a logical flow: login → inventory list → item actions. Input fields include validation to prevent user errors, and permissions are requested only when needed. The interface prioritizes readability, spacing, and clear labeling to ensure users can complete tasks quickly without confusion.

The design was successful because it minimized unnecessary complexity while still meeting all functional requirements.


## Development Approach

The development process focused on structure and the separation of responsibilities. Database logic was handled through helper and DAO classes rather than being embedded directly in activities. This made the app easier to manage and modify.

I approached development by:

- Defining database tables and structure first
- Building core functionality (login and CRUD)
- Adding validation and edge-case handling
- Implementing SMS permission logic
- Refining UI interactions and error handling

This structured approach ensured the app remained organized as new features were added. These techniques can be applied in future projects to improve maintainability, readability, and scalability.


## Testing and Validation

Testing was performed using the Android Emulator across multiple scenarios. This included:

- Verifying login and account creation
- Confirming database persistence after app restart
- Testing add, update, and delete operations
- Checking duplicate item prevention
- Testing SMS permission granted and denied states

This testing process was important because it exposed edge cases, such as duplicate entries and issues with permission handling. It reinforced the importance of validating both expected and unexpected user actions to ensure stability.


## Innovation and Problem Solving

One challenge encountered was preventing duplicate inventory items while maintaining clean database logic. This required modifying the database schema and implementing validation checks before insertion.

Another challenge was handling SMS permissions so that denying access did not disrupt the main functionality. Solving this required conditional logic and thoughtful permission management.

These situations required problem-solving beyond basic feature implementation.


## Demonstrated Knowledge and Skills

The component that best demonstrates my knowledge and skills is the integration of authentication, persistent storage, and optional system-level permissions within a single application. Successfully combining login validation, SQLite database operations, and runtime SMS permission handling shows an understanding of Android architecture, user experience, and platform requirements.

Completing this project demonstrates my ability to move from UI design to full implementation while applying best practices in structure, testing, and user-centered design.

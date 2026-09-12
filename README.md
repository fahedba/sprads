sprads - Patient Calling System
sprads is an open-source, lightweight digital signage and patient calling system built primarily with PHP. This repository contains the core framework for managing waitlists, rooms, and displaying calls on digital screens. It is optimized for small healthcare practices looking for an affordable, easy-to-use alternative to heavy enterprise software.
Features
Digital Signage: Manage displays to showcase patient calls alongside custom informational loops or graphics.
Waitlist Management: Add patients manually or queue them directly. Sort and organize effectively.
Room Assignment: Assign calls to specific rooms or practitioners dynamically.
Responsive Dashboard: A clean, web-based dashboard for practice staff to manage queues.
Repository Structure
/sprads
├── /assets           # CSS, JS, and image files for the dashboard
├── /config           # Configuration files for setting up instances
├── /database         # SQLite database management scripts
├── /includes         # Core PHP functions and classes
├── index.php         # The main entry point for the dashboard
├── dashboard.php     # The actual dashboard interface code
├── api.php           # API endpoints for AJAX requests
├── README.md         # This documentation file
└── LICENSE           # MIT License


Getting Started
Prerequisites
PHP 8.0 or higher
SQLite3 extension enabled in PHP
A web server (e.g., Apache, Nginx)
Installation
Clone the repository:
git clone https://github.com/fahedba/sprads.git
Navigate to the project directory:
cd sprads
Set up the database. The system uses SQLite. Ensure the web server has write access to the directory where the database file will be stored (usually configured in `/config/settings.php` or similar). A script like `queue.db.php` often handles the initial setup or connection.
Configure the system. Copy any example configuration files (like `config.example.php`) to `config.php` and update the necessary details (e.g., domain names, branding colors).
Access the dashboard via your web browser.
Usage (Dashboard Overview)
The system is designed with four main tabs in the interface:
1. Entry (Eintrag)
This tab allows staff to manually enter new patients into the system. You can specify names, prefixes (Herr/Frau), add specific notes, and assign them to a waiting area.
2. Waitlist (Warteliste)
Here you can view all patients currently waiting. The list shows their position, name, and any assigned target room or queue.
3. Call (Aufruf)
This is the core action tab. Staff select a room and the next patient to call them to the respective room. An audio toggle is available to play a sound upon calling.
4. Overview (Übersicht)
This tab displays a history or current overview of active calls across all rooms.
Contributing
Contributions are welcome! Please feel free to submit Pull Requests. For major changes, please open an issue first to discuss what you would like to change.
License
This project is licensed under the MIT License - see the LICENSE file for details.

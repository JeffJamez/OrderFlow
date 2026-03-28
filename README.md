# BeautyPOS

A desktop Point of Sale application for cosmetics retail, built with Python and PyQt5. Demonstrates proficiency in GUI development, database design, data export, and desktop application architecture.

## Value Proposition

BeautyPOS addresses the need for a lightweight, offline-capable POS system tailored to small cosmetics businesses. It showcases ability to build polished desktop applications with Python, manage local databases, and implement business logic for inventory and sales—skills directly transferable to enterprise desktop or hybrid applications.

## Core Features

- Secure login system with credential validation and session management
- Product management: add, update, search, and categorize cosmetics items
- Supplier tracking with contact details and inventory linkage
- Sales processing with real-time inventory deduction and total calculation
- User management with role-based permissions for sensitive operations
- Excel export functionality for sales reports using openpyxl
- Intuitive PyQt5 interface with sidebar navigation and modal dialogs

## Technical Architecture

Language: Python 3.x
GUI Framework: PyQt5 with Qt Designer-compatible UI structure
Database: SQLite with parameterized queries to prevent SQL injection
Data Export: openpyxl for generating formatted Excel reports
Icons and Assets: Qt Resource System (.qrc) for embedded assets
Architecture: Modular design with separate files for each business domain

## Project Structure

BeautyPOS/
├── gallery/              # Application icons and UI assets
├── database.py           # SQLite connection, schema initialization
├── login.py              # Authentication UI and logic
├── mainfile.py           # Application entry point and main window
├── mylogin.py            # Login form handler and validation
├── mymasewa.py           # Supplier management module
├── mysales.py            # Sales processing and reporting logic
├── myusers.py            # User account management with permissions
├── products.py           # Product catalog operations and search
├── sales.py              # Transaction logic and inventory updates
├── users.py              # User data models and access control
├── icons.qrc             # Qt resource definition for icons
├── icons_rc.py           # Compiled resource module
└── requirements.txt      # Python dependencies

## Setup Instructions

1. Clone the repository
   git clone https://github.com/JeffJamez/Cosmetics.git
   cd Cosmetics

2. Install dependencies
   pip install PyQt5 openpyxl

3. Run the application
   python mainfile.py

4. Use default credentials for initial access (change before production)
   Username: admin
   Password: admin123

## Key Technical Decisions

- Used PyQt5 signals and slots for decoupled, event-driven UI updates
- Implemented parameterized SQL queries to ensure database security
- Structured business logic in separate modules to improve testability and maintenance
- Leveraged Qt Resource System to bundle assets into a single executable-friendly package
- Designed Excel export to preserve formatting for immediate business use

## Data Integrity and Business Logic

- Sales transactions automatically deduct from product inventory to prevent overselling
- Excel exports include timestamps and itemized details for accounting reconciliation
- User permissions restrict sensitive operations to authorized personnel only
- Input validation at UI and database layers to ensure data quality

## Why This Project Stands Out to Recruiters

- Demonstrates ability to build complex desktop applications with Python—a valuable skill for internal tools, utilities, and hybrid deployments
- Shows understanding of database design, secure coding practices, and business workflow automation
- Clean modular architecture that is easy to extend with features like barcode scanning, receipt printing, or cloud sync
- Practical focus on real-world usability: intuitive UI, error handling, and export functionality
- Highlights problem-solving skills in bridging UI events, business logic, and data persistence

## Contributing

1. Fork the repository
2. Create a feature branch: git checkout -b feature/YourFeature
3. Commit changes: git commit -m 'Add YourFeature'
4. Push to branch: git push origin feature/YourFeature
5. Submit a pull request with a clear description of changes and testing steps

## License

MIT License. See LICENSE file for details.

## Author

Jeff James

**Biftekys CRM**
CRM system designed for application management and partner coordination. This project was developed with a focus on security, and a scalable MVC architecture.

**Key Features**
Dynamic Application Management: Comprehensive system for creating, editing, and tracking service applications with a built-in Draft system.

Advanced User Hierarchy: Multi-level user roles (SuperAdmin, Admin, Partner) with a visual tree-map for partner management.

Dynamic Field Builder: Admins can create and inject custom database fields into the application forms through the UI without writing code.

Secure Document Handling: Integrated file upload system with drag-and-drop support for application attachments.

Automated Export/Import: Data management via Excel (XLSX) and CSV using PhpSpreadsheet.

**Technical Highlights & Security**
Secure Hashing: Utilizes Bcrypt (PHP password_hash) for industry-standard credential protection.

SQL Injection Prevention: 100% of database interactions are handled via PDO with Prepared Statements.

CSRF Protection: Integrated token-based protection for all state-changing requests.

Custom Routing Engine: A centralized Front Controller (index.php) handles all requests through a dedicated Router class.

Singleton Pattern: Optimized database connectivity using the Singleton design pattern.

🛠️ Tech Stack
Backend: PHP 8.x (Object-Oriented)

Database: MySQL / MariaDB

Frontend: Bootstrap 5, FontAwesome, JavaScript (ES6+), jQuery

Dependencies: Composer (PhpSpreadsheet, ZipStream)

 Project Structure
├── controllers/    # Request handling & logic orchestration
├── models/         # Database logic & data structures
├── views/          # UI components & layouts
├── core/           # Framework engine (Router, Auth, Database)
├── config/         # Environment & constant configurations
├── assets/         # CSS, JS, and Images
└── helpers/        # Global utility functions & validation
Clone the repository:

Bash
git clone https://github.com/yourusername/CREm.git
Install dependencies:

Bash
composer install
Database Setup:

Import database/migrations.sql to your MySQL server.

Configure config/database.php with your credentials.

Run: Point your web server (Apache/Nginx) to the project root.

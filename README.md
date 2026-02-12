📦 Inventory Management System & Automated Reporting
🚀 Overview
Ce projet est un module de gestion de stocks conçu pour automatiser la surveillance des inventaires. Il combine une base de données relationnelle robuste et un moteur de reporting pour transformer des données brutes en documents d'aide à la décision.

🛠 Tech Stack
Language: Java (JDK 17+)

Database: MySQL (Workbench)

Reporting Tool: JasperReports (via Jaspersoft Studio)

Driver: JDBC (MySQL Connector/J)

📊 Data Pipeline Architecture
Le système suit un flux de données structuré pour garantir l'intégrité des rapports :

Data Storage: Modélisation des tables de stock sous MySQL.

Connectivity: Couche d'abstraction via la classe DatabaseManager pour sécuriser les appels JDBC.

Engine: Utilisation de JasperReports pour la compilation et le remplissage des données.

Output: Génération automatique d'un rapport décisionnel au format PDF.

📝 Key Features & Implementation
1. Database Connectivity (MySQL)
La connexion est optimisée via une gestion d'exceptions (SQLException) pour assurer la stabilité du module.

Class: DatabaseManager

Libraries: java.sql.Connection, java.sql.DriverManager.

2. Automated Reporting (JasperReports)
Le module transforme un template XML (.jrxml) en un rapport visuel prêt pour la direction.

Compilation: Transformation du fichier rapport_stock.jrxml via JasperCompileManager.

Data Filling: Injection des données SQL en temps réel avec JasperFillManager.

Export: Production du fichier final Etat_Stock.pdf.

📂 Project Structure
src/RapportStock.java : Coeur logique de l'application.

src/rapport_stock.jrxml : Design du rapport (Layout & Queries).

src/DatabaseManager.java : Configuration de la source de données.

src/Etat_Stock.pdf : Résultat final généré.

⚙️ Dependencies
JasperReports 7.0.2 : Moteur de génération.

MySQL Connector-J 9.2.0 : Pont de communication entre Java et MySQL.

💡 Why this matters for Data Analysis?
Ce projet démontre ma capacité à :

Concevoir et interroger des bases de données relationnelles.

Maîtriser le cycle ETL (Extract, Transform, Load) simplifié.

Fournir des outils de visualisation automatisés pour les décideurs métiers.


Here’s a suggested structure and content for your project’s GitHub repository:

Event Hackathon Search System

Project Description

The Event Hackathon Search System is a comprehensive platform designed for college students and administrators to explore, manage, and participate in hackathons and events. This system includes features for event registration, feedback, and user authentication, ensuring a seamless experience for both students and administrators.

Table of Contents

	1.	Features
	2.	Technologies Used
	3.	Installation
	4.	Usage
	5.	Project Structure
	6.	ER Diagram
	7.	Contributors
	8.	License

Features

	•	User Authentication:
	•	Secure login and registration for students and administrators.
	•	Event Management:
	•	Add, update, and delete events by administrators.
	•	Explore all upcoming and past events.
	•	Event Registration:
	•	Students can register for events with approval status tracking.
	•	Feedback System:
	•	Users can leave feedback and ratings for events.
	•	Error Handling:
	•	Store improperly formatted data in the ErrorData field for troubleshooting.

Technologies Used

	•	Frontend: Java Swing (GUI)
	•	Backend: Java
	•	Database: MySQL
	•	Libraries/Dependencies:
	•	mysql-connector-j-9.1.0.jar
	•	json-20210307.jar

Installation

	1.	Clone the Repository:

git clone https://github.com/<your-username>/EventHackathonSearch.git
cd EventHackathonSearch


	2.	Setup Database:
	•	Import the schema.sql file into your MySQL database.
	•	Update database credentials in DBConnection.java.
	3.	Add Dependencies:
	•	Place mysql-connector-j-9.1.0.jar and json-20210307.jar in the lib directory.
	4.	Compile and Run:

javac -cp "lib/*:bin" -d bin $(find . -name "*.java")
java -cp "bin:lib/*" com.project.auth.LoginPage

Usage

	•	Administrator:
	•	Login to manage events.
	•	Add or update events with details such as name, description, date, location, and more.
	•	Student:
	•	Register for events and track approval status.
	•	Provide feedback and ratings for attended events.

Project Structure

EventHackathonSearch/
├── src/
│   ├── com.project.auth/         # Authentication logic
│   ├── com.project.dashboard/    # GUI dashboards
│   ├── com.project.models/       # Data models
│   ├── com.project.services/     # Business logic and database operations
│   ├── com.project.utils/        # Utility classes (DB connections, etc.)
├── lib/                          # External JAR dependencies
├── bin/                          # Compiled Java classes
├── schema.sql                    # Database schema
├── README.md                     # Project documentation
├── launch.json                   # VSCode configuration
└── LICENSE                       # License file

Contributors

	•	Gokulakrishnan K. (230701094)
	•	Gokul Anand B. (230701093)

License

This project is licensed under the MIT License. See the LICENSE file for more details.

Additional Notes

	•	If you encounter any issues, feel free to create a GitHub Issue or reach out to the contributors.
	•	Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.


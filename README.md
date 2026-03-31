Hostel Complaint Management System 🏢 ✅
A full-stack web application designed to bridge the communication gap between hostel residents and administration. 
This system replaces traditional, inefficient paper-based logs with a transparent, real-time digital tracking workflow.

🚀 Overview
The Hostel Complaint Management System allows students to report maintenance or facility issues directly to the warden. 
It provides a structured dashboard for administrators to track, acknowledge, and resolve complaints, ensuring accountability and timely fixes.

✨ Key Features
Student Portal: Easy submission of complaints with specific categories and room numbers.

Warden Dashboard: Centralized view of all active issues with the ability to update statuses.

Status Lifecycle: Real-time tracking through three stages: PENDING ➡️ ACKNOWLEDGED ➡️ RESOLVED.

Secure Access: Role-based access using a STUDENT_SECRET and administrative credentials.

Data Persistence: Robust storage of complaint history and user details.
🛠️ Tech StackLayerTechnology
Frontend  - React.js, CSS3, Axios
Backend   - Java, Spring Boot, Spring Data JPA
Database   - MySQL
Build Tool  - Maven
📂 Project StructurePlaintext├── backend/           # Spring Boot Application
│   ├── src/main/java  # Controllers, Services, Models, Repositories
│   └── src/resources  # application.properties (DB config)
├── frontend/          # React.js Application
│   ├── src/components # UI Components
│   └── src/App.js     # Routing and State Management
└── README.md
1.Create a database named hostel_db in MySQL. Update your backend/src/main/resources/application.properties:Properties
spring.datasource.url=jdbc:mysql://localhost:3306/hostel_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
2. Backend SetupBash
cd backend
mvn clean install
mvn spring-boot:run
3. Frontend SetupBash
cd frontend
npm install
npm start
📝 Usage
Students: Login using your Room Number and the unique STUDENT_SECRET. Submit a complaint by selecting a category (Plumbing, Electrical, etc.).
Wardens: Log in using the admin credentials. View the list of complaints and update the status to "Acknowledged" once the work starts, and "Resolved" upon completion.

Contract Monthly Claim System (CMCS)
Project Overview
The Contract Monthly Claim System (CMCS) is a web-based application designed to streamline and automate the claim submission and approval process for Independent Contractor lecturers. The system allows lecturers to submit claims, which can be reviewed, approved, or rejected by the relevant program coordinators and HR personnel.

Features
Claim Submission: Lecturers can submit claims for their contracted work.
Claim Approval/Rejection: Program coordinators and HR can approve or reject claims.
Document Uploads: Support for uploading supporting documents like invoices, reports, etc.
Status Tracking: Track the status of claims in real-time (pending, approved, rejected).
Role-Based Access Control (RBAC): Different user roles, such as lecturers, coordinators, and HR, with distinct permissions.
Technologies Used
Backend:
ASP.NET Core (MVC)
Entity Framework for ORM
SQL Server for the database
Frontend:
HTML, CSS, JavaScript
Bootstrap for responsive design
Tools & Libraries:
Visual Studio
Git for version control
Postman for API testing
System Requirements
.NET 6.0 or higher
SQL Server
Visual Studio or any .NET-compatible IDE
Internet connection for live demo (optional)
Installation Guide
1. Clone the repository
bash
Copy code
git clone https://github.com/yourusername/cmcs.git
2. Install dependencies
Ensure you have the .NET SDK installed. Run the following command to restore dependencies:

bash
Copy code
dotnet restore
3. Configure the database
Open appsettings.json and update the connection string with your SQL Server credentials:
json
Copy code
"ConnectionStrings": {
  "DefaultConnection": "Server=your_server_name;Database=your_database_name;Trusted_Connection=True;"
}
Run the following command to create the database schema:
bash
Copy code
dotnet ef database update
4. Run the application
bash
Copy code
dotnet run
Navigate to https://localhost:5001 in your browser to access the application.

User Roles and Permissions
Lecturer:
Submit claims for review
View the status of submitted claims
Program Coordinator:
Review, approve, or reject claims
HR:
Final approval of claims and processing payments
Screenshots

Login page of the application.


Claim submission page.

Future Enhancements
Mobile Responsiveness: Improve the UI for mobile devices.
Email Notifications: Implement email alerts for claim status updates.
Analytics Dashboard: Provide analytics on claims, such as trends and performance metrics.
Contributing
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Commit your changes (git commit -am 'Add new feature').
Push to the branch (git push origin feature-branch).
Open a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.

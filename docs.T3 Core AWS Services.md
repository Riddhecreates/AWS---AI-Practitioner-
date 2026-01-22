📘 Topic 3: Core AWS Services

🎯 Goal of this topic

By the end of this topic, you should understand what kind of services AWS provides, what problem each solves, and where they fit in your education system.

⸻

1️⃣ Core Services You MUST Know

Focus only on these four:
	•	Amazon EC2 (Compute)
	•	Amazon S3 (Storage)
	•	Amazon RDS (Database)
	•	AWS IAM (Security & Access)

⸻

2️⃣ Questions You MUST Be Able to Answer

You are not “done” with Topic 3 unless you can answer all of these.

⸻

A. Amazon EC2 (Elastic Compute Cloud)- COMPUTE

•	What is EC2?
- Amazon EC2 (Elastic Compute Cloud) is an AWS service that provides on-demand virtual servers in the cloud to run applications. Elastic means you can scale computing power up or down at any time (for example, handling 1 teacher today and 1,000 teachers later). Compute refers to processing power (CPU, memory, networking) used to run software and services. Cloud means the servers are hosted in AWS data centers and accessed over the internet, so you don’t own or maintain physical machines. In practice, EC2 lets organizations run applications without buying hardware, paying only for what they use. For a system like EduHelper, EC2 would handle the main application logic—processing surveys, generating lesson plans, and responding to users—while automatically adjusting capacity based on classroom demand and usage levels.

•	Why would a website need EC2?
- A website needs EC2 because it requires computing power to run its logic, not just store files. In theory, a website is more than pages—it must process requests, run code, handle logins, analyze data, and return results. EC2 provides virtual servers that execute this work. Practically, for a system like EduHelper, EC2 handles teacher authentication, student survey processing, AI-based lesson plan generation, and real-time responses. Without EC2, the site would be static and unable to react to users.

•	What runs on EC2 in simple terms?
- In simple terms, EC2 runs the “brain” of a website. Theoretically, EC2 executes the application code that decides what happens when a user clicks, submits, or requests something. Practically, in EduHelper, EC2 runs the backend logic: checking teacher logins, processing student surveys, calling AI services, generating lesson plans, and sending results back to iPads. Without EC2, nothing “thinks” or responds—pages would just sit there.

•	Would students directly interact with EC2?
- EC2 is a backend compute service, not a user-facing interface. In practice, students interact with a website or app on their iPads; that request goes to a server (EC2), which processes it and sends back results. This separation is critical for security, scalability, and simplicity—students shouldn’t (and can’t) touch the infrastructure running the system.

•	Why is EC2 better than running a local server?
- EC2 is better than a local server because it is scalable, reliable, and remotely managed. A local server can fail, overload, or require physical maintenance, while EC2 can automatically scale up if usage increases (e.g., from 1 teacher to 1,000 teachers). For EduHelper, this means the system keeps running during classes without IT staff on-site, which is critical for schools.


⸻

B. Amazon S3 (Simple Storage Service)- STORAGE

•	What is Amazon S3?
- Amazon S3 (Simple Storage Service) is a cloud-based storage solution that lets you store and retrieve files over the internet securely and reliably. It works like a giant online hard drive that is always available. Teachers and students can access lesson plans, PDFs, and class materials anytime on any device, without worrying about local storage limits or device compatibility.

•	What kind of data is stored in S3?
- Teachers and students can access lesson plans, PDFs, and class materials anytime on any device, without worrying about local storage limits or device compatibility. S3 can store any type of digital content: documents, images, videos, audio, PDFs, CSV/Excel files, backups, and more. All classroom materials—lesson PDFs, video tutorials, activity files, and student data exports—can be stored centrally in S3, making them easy to manage and deliver to students and teachers efficiently.

•	Why is S3 good for PDFs and lesson materials?
- PDFs and lesson slides are static files that don’t change frequently, but need to be accessible on-demand. S3 allows fast download and sharing, supports versioning, and ensures files are safe and backed up automatically. Teachers can upload textbooks or AI-generated lesson plans to S3 once, and students can access them during class without delays. It also allows EduHelper to quickly pull content for generating lesson plans or presentations.

•	Can S3 store student surveys?
- Yes, S3 can store raw survey data in formats like CSV, JSON, or Excel. While active querying is better handled by a database (e.g., RDS), S3 is perfect for backups or large datasets. Survey results from students about their mood, engagement, or learning preferences can be stored in S3 for AI processing and analysis, ensuring the data is secure and always available when creating personalized lesson plans.

•	Why is S3 more reliable than local storage?
- S3 automatically replicates data across multiple physical locations (availability zones), uses strong security and encryption, and is managed by AWS engineers. Unlike local storage, it cannot fail due to a single device or server crash. Teachers never lose lesson materials, student responses, or AI-generated content. Even if a classroom iPad or school server fails, EduHelper continues to operate smoothly, maintaining trust and reliability for daily teaching.

⸻

C. Amazon RDS (Relational Database Service)- DATABASE

•	What is a database?
- A database is an organized system for storing, managing, and retrieving data efficiently. Unlike random files, databases structure data in tables, rows, and columns, allowing you to search, sort, and analyze it quickly. Teacher profiles, class schedules, and survey responses are stored in structured tables so the system can quickly find and process the information needed for lessons or AI analysis.

•	Why not store everything in Excel?
- Excel can store data but is manual, error-prone, and not scalable. It doesn’t handle multiple users well, cannot enforce data rules, and slows down with large datasets. If thousands of students’ surveys were in Excel, the system would be slow, prone to mistakes, and impossible to query in real time for AI-generated lesson suggestions. RDS handles this automatically.

•	What kind of data belongs in a database?
- Structured, relational, or frequently queried data belongs in a database. All dynamic, regularly updated classroom data is best stored in a database so it can be read and written reliably during live lessons. For example, teacher and student profiles, class schedules and attendance, survey responses, system settings and permissions etc.

•	How would teacher profiles be stored?
- Teacher profiles would be stored in tables with column titles like: Name, Email, Assigned classes, Login credentials, Permissions. Each teacher is a row, allowing fast lookups, updates, or filtering for tasks like sending notifications or generating class-specific AI insights.

•	Why is RDS important for structured data?
- RDS is managed, fault-tolerant, and scalable. It automates backups, security updates, and replication across Availability Zones. Structured classroom data is safe, fast, and always available, even if one data center fails. Teachers can trust the system to provide accurate information instantly, which is essential for real-time classroom decision-making.

⸻

D. AWS IAM (Identity and Access Management)- SECURITY

•	What is IAM?
- AWS IAM (Identity and Access Management) is a service for managing users, roles, and permissions in the cloud. It controls who can do what, including access to servers (EC2), storage (S3), databases (RDS), and other AWS services. IAM enforces security policies, enabling organizations to follow the principle of least privilege—users get only the access they need. IAM ensures only authorized teachers, admins, or developers can access specific parts of the system, keeping student data safe and classroom workflows secure.

•	Why is access control critical in education systems?
- Student data is personal, sensitive, and legally protected. Improper access can lead to privacy violations, identity theft, or misuse of information. By controlling access, IAM ensures confidentiality, integrity, and compliance with regulations like GDPR or Japanese privacy laws. Unrestricted access could lead to privacy breaches, cheating, or data loss. Access control ensures that users see only what they are allowed to see. Teachers can access their classes but not other teachers’ classes, students can only see their own progress, and admins manage the system without exposing private data.

•	What happens if permissions are wrong?
- If permissions are too loose, unauthorized users could view, edit, or delete sensitive data. If too strict, legitimate users cannot do their work, causing frustration and downtime. Incorrect IAM settings could mean a teacher cannot view their class roster, or student data is accidentally exposed, both scenarios breaking trust and system reliability.

•	Who should access student data?
- Only authorized teachers, admins, and certain AI processing services should access student data. Students themselves should have limited access to their own records, and no external parties should access raw data. Proper IAM ensures AI analysis can read anonymous data to generate lesson insights without exposing personal student information.

•	Why is IAM more important than features?
- Even advanced AI or interactive features are meaningless if the system is insecure or unreliable. Security and proper access control form the foundation of any education system, because without trust, teachers will not use the tool. Teachers will adopt EduHelper only if it’s secure, reliable, and compliant. IAM guarantees that EduHelper can be safely adopted in classrooms so that teachers rely on its security first, then on its AI capabilities to improve teaching and learning.
⸻

3️⃣ Things You Should Be Able to Explain Simply

You should be able to explain:
	•	EC2 = computers in the cloud
	•	S3 = online storage
	•	RDS = organized data storage
	•	IAM = who can do what

If you can’t explain it simply, don’t move on.

⸻

4️⃣ Project Connection (Critical)

You must be able to explain:
	•	What runs on EC2 in your project
	•	What data goes into S3
	•	What data goes into RDS
	•	How IAM protects teachers and students
	•	Why these services come before AI

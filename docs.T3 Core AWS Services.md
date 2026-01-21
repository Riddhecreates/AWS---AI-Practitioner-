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

A. Amazon EC2 (Compute)

•	What is EC2?
- Amazon EC2 (Elastic Compute Cloud) is an AWS service that provides on-demand virtual servers in the cloud to run applications. Elastic means you can scale computing power up or down at any time (for example, handling 1 teacher today and 1,000 teachers later). Compute refers to processing power (CPU, memory, networking) used to run software and services. Cloud means the servers are hosted in AWS data centers and accessed over the internet, so you don’t own or maintain physical machines. In practice, EC2 lets organizations run applications without buying hardware, paying only for what they use. For a system like EduHelper, EC2 would handle the main application logic—processing surveys, generating lesson plans, and responding to users—while automatically adjusting capacity based on classroom demand and usage levels.

•	Why would a website need EC2?
- A website needs EC2 because it requires computing power to run its logic, not just store files. In theory, a website is more than pages—it must process requests, run code, handle logins, analyze data, and return results. EC2 provides virtual servers that execute this work. Practically, for a system like EduHelper, EC2 handles teacher authentication, student survey processing, AI-based lesson plan generation, and real-time responses. Without EC2, the site would be static and unable to react to users.

•	What runs on EC2 in simple terms?
- In simple terms, EC2 runs the “brain” of a website. Theoretically, EC2 executes the application code that decides what happens when a user clicks, submits, or requests something. Practically, in EduHelper, EC2 runs the backend logic: checking teacher logins, processing student surveys, calling AI services, generating lesson plans, and sending results back to iPads. Without EC2, nothing “thinks” or responds—pages would just sit there.

•	Would students directly interact with EC2?
- EC2 is a backend compute service, not a user-facing interface. In practice, students interact with a website or app on their iPads; that request goes to a server (EC2), which processes it and sends back results. This separation is critical for security, scalability, and simplicity—students shouldn’t (and can’t) touch the infrastructure running the system.
- 
•	Why is EC2 better than running a local server?
- EC2 is better than a local server because it is scalable, reliable, and remotely managed. A local server can fail, overload, or require physical maintenance, while EC2 can automatically scale up if usage increases (e.g., from 1 teacher to 1,000 teachers). For EduHelper, this means the system keeps running during classes without IT staff on-site, which is critical for schools.


⸻

B. Amazon S3 (Storage)

•	What is Amazon S3?
- Amazon S3 (Simple Storage Service) is a cloud-based storage solution that lets you store and retrieve files over the internet securely and reliably. It works like a giant online hard drive that is always available. Teachers and students can access lesson plans, PDFs, and class materials anytime on any device, without worrying about local storage limits or device compatibility.

•	What kind of data is stored in S3?
- Teachers and students can access lesson plans, PDFs, and class materials anytime on any device, without worrying about local storage limits or device compatibility. S3 can store any type of digital content: documents, images, videos, audio, PDFs, CSV/Excel files, backups, and more.

•	Why is S3 good for PDFs and lesson materials?
•	Can S3 store student surveys?
•	Why is S3 more reliable than local storage?

⸻

C. Amazon RDS (Databases)
	•	What is a database?
	•	Why not store everything in Excel?
	•	What kind of data belongs in a database?
	•	How would teacher profiles be stored?
	•	Why is RDS important for structured data?

⸻

D. AWS IAM (Security)
	•	What is IAM?
	•	Why is access control critical in education systems?
	•	What happens if permissions are wrong?
	•	Who should access student data?
	•	Why is IAM more important than features?

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

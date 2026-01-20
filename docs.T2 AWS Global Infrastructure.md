📘 Topic 2: AWS Global Infrastructure

🎯 Goal of this topic

By the end of this topic, you should understand where AWS runs, why location matters, and how AWS stays reliable — especially for schools and real users.

⸻

1️⃣ Core Concepts You MUST Know

You must clearly understand:
•	What an AWS Region is
•	What an Availability Zone (AZ) is
•	What Edge Locations are
•	Why AWS uses multiple physical locations
•	Why latency matters for users

⸻

2️⃣ Questions You MUST Be Able to Answer

You are not done unless you can answer all of these in your own words.

⸻

A. Regions

•	What is an AWS Region?
- An AWS Region is a large geographic area (usually a country or part of a continent) where AWS operates data centers. Its purpose is to store and process data close to users, help meet data residency laws (very important in Japan) and reduce latency for a faster response. If all data were stored in one country, users far away would experience delays and legal issues.

•	Why does AWS have multiple Regions?
- AWS has multiple Regions to serve users around the world efficiently, securely, and reliably. AWS uses multiple Regions to provide low latency, fault tolerance, regulatory compliance, and global scalability. AWS uses multiple Regions to reduce latency (users access services from the nearest Region, making applications faster), to meet legal and data regulations (some countries require data to stay within national borders e.g., Japan), to improve reliability and disaster recovery (if one Region fails due to a disaster, another Region can continue operations) and to support global scalability (applications can expand internationally without rebuilding systems).

•	Why would Japan need its own Region?
•	What could go wrong if everything ran from one country?
•	Which AWS Region would your project likely use?

⸻

B. Availability Zones (Very Important)

•	What is an Availability Zone?
- An Availability Zone is a separate physical data center inside a Region. It provides backup and fault tolerance, prevents service downtime if one data center fails and enables high availability. Hardware can fail and natural disasters can happen. AZs ensure systems stay online.

•	How is an AZ different from a Region?
•	Why does AWS use multiple AZs inside one Region?
•	What happens if one AZ fails?
•	How does this improve reliability for schools?

⸻

C. Edge Locations

•	What is an Edge Location?
- Edge Locations are small AWS facilities located near users to deliver content faster. Its function is to speed up content delivery, reduces latency and improve user experience. It is important because otherwise sending data from far-away servers is slow, especially for images, videos, and web pages.

•	How is it different from a Region?
•	What kind of content uses Edge Locations?
•	Why do Edge Locations reduce latency?
•	Would Edge Locations matter for students using iPads?

⸻

D. Latency & User Experience

•	What is latency (simple explanation)?
•	Why does latency matter in classrooms?
•	How would high latency affect students?
•	Why do real-time tools need low latency?
•	How does AWS reduce latency globally?

⸻

E. Your Project Connection (Critical)

•	Why does your project need low latency?
•	Why Japan-based infrastructure matters for Japanese schools?
•	How Regions and AZs improve trust in the system?
•	What would happen during a class if the system goes down?
•	Why infrastructure reliability matters more than “cool AI”

⸻

3️⃣ Things You Should Be Able to Explain Simply

You should be able to say:
	•	“AWS has data centers all over the world”
	•	“Regions are countries/areas, AZs are separate buildings”
	•	“If one building fails, another takes over”
	•	“Closer servers = faster response”

If you can’t explain it simply, don’t move on.

⸻

4️⃣ Completion Criteria

You are done with Topic 2 only if:
	•	You can explain Regions, AZs, Edge Locations without notes
	•	You can explain why Japan needs local infrastructure
	•	You can relate reliability to classroom reality
	•	You can write one paragraph explaining why AWS infrastructure fits EduHelper

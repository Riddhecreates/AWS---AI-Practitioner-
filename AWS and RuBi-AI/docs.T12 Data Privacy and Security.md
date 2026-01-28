📘 Topic 12: Data Privacy & Security in AI Systems

🎯 Goal of this topic

By the end of this topic, you must clearly understand:
	•	Why privacy and security are critical in AI applications
	•	How student and teacher data should be handled
	•	How AWS helps ensure secure AI services
	•	How RuBi-AI can implement safe data practices

⸻

1️⃣ Core Concepts You MUST Understand

•	Data Privacy: Protecting personal data so it is collected, used, and shared only in approved and lawful ways.

•	Data Security: Protecting data from unauthorized access, alteration, or loss using technical and organizational controls.

•	Encryption: Transforming data into an unreadable format so only authorized parties can access it using a key.

•	Access Control: Limiting who can view, use, or modify data based on identity and permissions.

•	Anonymization / Pseudonymization: Techniques that remove or hide personal identifiers so individuals cannot be easily identified.

•	Compliance Standards: Laws, regulations, and policies that define how data must be handled responsibly and legally.

•	AWS Security Tools: AWS services that help protect data and control access, such as IAM, encryption services, and secure storage.


⸻

2️⃣ Questions You MUST Be Able to Answer

You are not done with Topic 12 unless you can answer all of these.

⸻

A. Conceptual Understanding

•	What is the difference between privacy and security?
- Privacy is a governance concept that defines what should happen to personal data, including who is allowed to collect it, how it is used, and for how long, while security is a technical concept focused on how violations are prevented using controls such as authentication, encryption, and monitoring; it is possible to have strong security and still violate privacy if data is used unnecessarily or unethically.

•	Why is student data sensitive?
- Student data often includes identifiers, learning behavior, academic performance, and sometimes psychological or biometric indicators, and this information can be exploited for profiling, discrimination, or surveillance, which is why learners and children are given higher protection standards under many data protection frameworks.

•	What is encryption, and why is it important?
- Encryption is based on cryptography, where mathematical algorithms transform data using keys, and it is important because it protects data at rest, in transit, and sometimes in use, ensuring that data remains protected even if systems or infrastructure are compromised.

•	How do access controls protect data?
- Access control is built on the principle of least privilege, meaning users and systems receive only the permissions they need, which reduces human error and limits the impact of security incidents caused by compromised credentials or misconfigured permissions.

•	Why is compliance important even for small AI projects?
- Compliance exists to reduce systemic risk rather than only large-company risk, and even small AI projects can scale quickly, reuse data unintentionally, or be deployed publicly, making early legal and ethical safeguards necessary from the start.

⸻

B. AWS Perspective

•	How does AWS ensure data privacy in AI services?
-AWS ensures data privacy in AI services by giving customers control over how their data is stored, processed, and accessed, while AWS itself secures the underlying cloud infrastructure; customer data is not used to train AWS models by default, and privacy is enforced through isolation, encryption, access controls, and compliance with global data protection frameworks under the shared responsibility model.
	
•	What is AWS IAM and how is it used?
- AWS Identity and Access Management (IAM) is a service that controls who can access AWS resources and what actions they are allowed to perform, using identities such as users, roles, and policies; it is used to enforce least-privilege access, reduce unauthorized usage, and securely manage permissions across services, including AI and data resources.

•	How can AWS encrypt data in storage and transit?
- AWS encrypts data in storage (at rest) using managed encryption keys through services like AWS Key Management Service (KMS), and encrypts data in transit using secure communication protocols such as TLS; this ensures data remains protected whether it is stored in databases, moving between services, or accessed by applications.

•	Are AWS AI services GDPR-compliant?
- AWS AI services are designed to support GDPR compliance by providing data protection features, regional data controls, audit logs, and contractual commitments, but GDPR compliance is ultimately a shared responsibility, meaning AWS provides compliant infrastructure while customers are responsible for lawful data usage, consent, and configuration. GDPR is a European Union data protection law that defines how personal data must be collected, processed, stored, and protected, giving individuals rights over their data such as access, correction, and deletion; it applies to any organization that handles EU residents’ data, regardless of where the organization or cloud service is located.

•	How does AWS manage secure access for multiple users?
- AWS manages secure access for multiple users through IAM roles, policies, and temporary credentials, allowing organizations to assign different permission levels based on job roles; this centralized access management reduces credential sharing, limits exposure, and scales securely as teams and projects grow.

⸻

C. Project Relevance

•	How will RuBi-AI protect student survey responses?
- RuBi-AI will protect student survey responses by minimizing data collection, encrypting responses during storage and transfer, and restricting access so only authorized systems or educators can view aggregated or necessary results, reducing the risk of misuse or exposure.

•	How will teacher profile data remain confidential?
- Teacher profile data will remain confidential by storing it securely, limiting access based on role and responsibility, and ensuring that personal details are not exposed publicly or shared beyond what is required for system functionality.

•	Should AI results be stored temporarily or permanently?
- AI results should be stored temporarily unless there is a clear educational or legal need for long-term storage, because limiting retention reduces privacy risk, lowers compliance burden, and prevents unintended reuse of sensitive insights.

•	How can you ensure only authorized teachers access their class data?
- Only authorized teachers can access their class data by using identity-based access controls that tie permissions to specific roles or classes, ensuring teachers can view only the data relevant to their own students.

•	What steps prevent accidental exposure of sensitive data in the website?
- Accidental exposure is prevented by using secure authentication, avoiding sensitive data in URLs or logs, enforcing strict access permissions, and regularly reviewing system design to ensure personal information is not unnecessarily displayed or shared.

⸻

3️⃣ Things You Should Be Able to Explain Simply

You must be able to explain to a non-technical teacher:
	•	AI keeps personal data safe and private
	•	Only authorized people (teachers/admins) can see data
	•	Encryption protects data from hackers
	•	AI does not expose student info publicly
	•	Privacy laws guide how AI handles data

⸻

4️⃣ Project Connection (Critical)

You should clearly state:
	•	RuBi-AI encrypts student and teacher data
	•	Teachers control who sees their class data
	•	AI uses anonymized feedback to improve lesson plans
	•	AWS security features reduce risk of data breaches
	•	Maintaining privacy ensures trust and adoption in schools

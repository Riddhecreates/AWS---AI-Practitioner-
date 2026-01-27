📘 Topic 13: Project Design & Implementation Strategy

🎯 Goal of this topic

By the end of this topic, you must clearly understand:
	•	How to design an AI system from idea to implementation
	•	How AWS AI services and LLMs fit into a project workflow
	•	How to plan EduHelper’s architecture for scalability, privacy, and usability
	•	How to align project design with real classroom constraints

⸻

1️⃣ Core Concepts You MUST Understand

•	System Architecture: System architecture describes the high-level design of an AI system, including its components, data storage, processing layers, and communication patterns, and it explains how these parts work together to meet functional, security, and performance requirements.

•	Input-Process-Output (IPO) Model: The IPO model is a conceptual framework used to clearly separate what data enters a system, how that data is transformed through rules or AI models, and what outputs are generated, helping designers analyze logic, responsibility, and system boundaries.

•	Data Flow: Data flow represents how information moves between system components, showing where data is collected, processed, stored, and shared, which is important for understanding performance, security, and privacy risks.

•	Integration: Integration refers to the coordination of multiple services, APIs, and AI components so they operate as a unified system, reducing manual steps, data duplication, and system complexity.

•	User Interface (UI) & User Experience (UX): UI focuses on the visual and interactive elements of the system, while UX focuses on the overall ease, efficiency, and clarity of user interaction, both of which affect adoption, accuracy, and user trust in AI systems.

•	Feedback Loop: A feedback loop allows system outputs to be reviewed and reused as input for future improvements, enabling AI systems to adapt over time while still requiring human oversight to prevent error amplification.

•	Scalability: Scalability describes a system’s capacity to handle growth in users, data volume, or workload by efficiently allocating resources, rather than requiring a complete redesign.


⸻

2️⃣ Questions You MUST Be Able to Answer

You are not done with Topic 13 unless you can answer all of these.

⸻

A. Conceptual Understanding

•	What are the key components of an AI system for education?
- An AI system for education typically includes data sources from students and teachers, secure data storage, AI models or logic for analysis and recommendations, integration services to connect components, and a user interface that allows educators to interact with results, all supported by privacy, security, and compliance controls.

•	What is the IPO model, and why is it useful?
- The Input–Process–Output model is a conceptual framework that separates what data enters the system, how it is transformed by AI or rules, and what outputs are produced, making it useful for clearly explaining system logic, responsibilities, and boundaries without focusing on technical implementation.

•	How does data flow from students/teachers to AI and back?
- Data flows from students and teachers into the system through input forms or interactions, is securely transmitted to processing components where AI analyzes or summarizes it, and then returns to users as insights, feedback, or recommendations through the application interface.

•	What is a feedback loop, and why is it critical?
- A feedback loop is a mechanism where users review AI outputs and provide responses that are reused to improve future results, which is critical because it allows the system to adapt over time while maintaining accuracy, relevance, and human oversight.

•	Why is scalability important for future growth?
- Scalability is important because educational AI systems often start small but must support more users, subjects, and data over time, and scalable design allows this growth without performance loss or major architectural changes.

⸻

B. AWS Perspective

•	Which AWS services fit each stage of the EduHelper system?
- In an EduHelper-style system, AWS services are mapped to stages such as data input, processing, storage, and output, where front-end services handle user interaction, managed AI services handle analysis and generation, storage services retain data securely, and orchestration services connect all components into a single workflow under a shared architecture.

•	How does AWS support integration between LLMs and other AI services?
- AWS supports integration by providing managed APIs, SDKs, and service-to-service communication that allow large language models to work alongside other AI services such as analytics or recommendation components, enabling different models and tools to exchange data seamlessly within one system. An SDK (software development kit) is a collection of tools, libraries, and documentation that helps developers interact with a service more easily, allowing applications to call AWS services (including AI and LLM APIs) without building everything from scratch.

•	How can AWS ensure smooth scaling as the number of users grows?
- AWS supports smooth scaling through elastic infrastructure that automatically adjusts compute, storage, and processing capacity based on demand, allowing systems to handle increases in users or data volume without requiring redesign or manual intervention.

•	How does AWS security and privacy tools support implementation?
- AWS security and privacy tools support implementation by enforcing identity-based access control, encrypting data in storage and transit, monitoring system activity, and providing compliance-ready infrastructure, while customers retain control over how data is used and accessed under the shared responsibility model.

•	Which services allow real-time processing versus batch processing?
- AWS supports real-time processing through services designed for immediate data handling and low-latency responses, while batch processing is supported through services that process large volumes of data at scheduled intervals, allowing systems to balance responsiveness and efficiency depending on use case.

⸻

C. Project Relevance

•	How will EduHelper implement IPO for each lesson plan?
- EduHelper will apply the Input–Process–Output model by clearly defining lesson inputs such as teacher goals and student context, processing them through AI analysis and pedagogical logic, and producing structured lesson plans or suggestions as outputs, which helps keep system logic transparent and easy to explain.

•	How will teacher surveys, student mood, and content PDF be processed?
- Teacher surveys, student mood indicators, and content PDFs will be collected as input data, normalized and analyzed by AI to identify patterns or key insights, and then combined during processing to generate recommendations that align teaching objectives with student needs.

•	How can the AI suggest improvements while keeping teachers in control?
- The AI will act as a decision-support tool by providing optional suggestions rather than automated decisions, allowing teachers to review, accept, modify, or reject recommendations, which preserves human authority and reduces the risk of over-reliance on AI.

•	How will the system store and update feedback for continuous learning?
- Feedback will be stored securely as structured data and used to evaluate past AI outputs, enabling the system to refine future recommendations over time while applying retention limits to prevent unnecessary long-term storage of sensitive information.

•	How will the UI/UX design ensure adoption by Japanese teachers and students?
- UI/UX design will focus on simplicity, clarity, and cultural familiarity by minimizing complexity, using intuitive workflows, and reducing cognitive load, which helps build trust and encourages consistent use among Japanese teachers and students.

⸻

3️⃣ Things You Should Be Able to Explain Simply

You must be able to explain to a non-technical teacher:
	•	EduHelper takes input (teacher, student, content), processes it using AI, and outputs lesson plans
	•	Teachers adjust the suggestions based on their classroom needs
	•	The system learns over time from feedback
	•	AWS helps manage AI tasks without building models from scratch
	•	UI is simple; teachers and students don’t need technical knowledge

⸻

4️⃣ Project Connection (Critical)

You should clearly state:
	•	EduHelper’s architecture integrates AWS AI services, LLMs, and secure storage
	•	IPO model ensures systematic handling of inputs and outputs
	•	Feedback loop enables adaptive lesson planning
	•	Scalability ensures future growth across multiple schools and subjects
	•	Human oversight remains central, maintaining ethical and effective teaching

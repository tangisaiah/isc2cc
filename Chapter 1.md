Chapter 1 Security Principles
---------
## Module 1: Understand the Seucirty Concepts of Information Assurance

### CIA Triad
* **Confidentiality** relates to **permitting authorized access to information**, while at the same time **protecting information from improper disclosure**.
* **Integrity** is the property of information whereby it is recorded, used and maintained in a way that ensures its **completeness, accuracy, internal consistency and usefulness** for a stated purpose.
* **Availability** means that systems and data are **accessible at the time users need them**.

#### Terminology
* **Perosnally Identifiable Information (PII)**: Data about an individual that could be used to **identify** them.
* **Protected Health Information (PHI)**: One’s health status
* **Classified**:  Sensitive information. e.g. trade secrets, research, business plans and intellectual property.
* **Sensitivity**: A measure of the importance assigned to information by its owner, or the purpose of denoting its **need for protection**.

### Authentication
**Authentication** is a process to **prove the identity of the requestor**.

#### 3 common methods
* Something you know **(Knowledge-based)**: **Password** or paraphrases 
* Something you have **(Token-based)**: **Tokens**, memory cards, smart cards
* Something you are **(Charateristic-based)**: **Biometrics**, measurable characteristics

#### Terminology
* **Single-factor authenticaation (SFA)**: Using only one of the methods of authentication.
* **Multi-factor authentication (MFA)**: Granting users access only after successfully demonstrating or displaying **two or more** of these methods.
* **Non-repudiation**: A legal term and is defined as the protection against an **individual falsely denying** having performed a particular action.

### Privacy
* **Privacy**: The right of an individual to **control the distribution of information** about themselves.
* **General Data Protection Regulation (GDPR)**: Applies to all organizations, foreign or domestic, doing business in the EU or any persons in the EU. 

## Module 2: Understand the Risk Management Process

### Risk Management
**Information security risk** reflects the **potential impacts** that result from the **possibility of unauthorized access, use, disclosure, disruption, modification or destruction** of information 
and/or information systems. This definition represents that **risk is associated** with **threats, impact and likelihood**, and it also indicates that IT risk is a subset of business risk. 

#### Terminology
* **Asset**: Something in **need of protection**.
* **Vulnerability**: A **gap or weakness** in those protection efforts.
* **Threat**: **Something or someone** that aims to **exploit a vulnerability** to thwart protection efforts.

### Threats
In the context of cybersecurity, typical **threat actors** include the following:
* **Insiders**: Either deliberately, by simple human error, or by gross incompetence)
* **Outside individuals / informal groups**: Either planned or opportunistic, discovering vulnerability
* **Nonpolitical Formal entities**: Business competitors and cybercriminals
* **Political Formal entities**: Terrorists, nation-states, and hacktivists
* **Intelligence or information gatherers**: Could be any of the above
* **Technology**: Free-running bots and artificial intelligence , which could be part of any of the above

### Likelihood
**Probability** or **likelihood**: Potential vulnerability being exploited within the construct of the organization’s threat environment

#### Terminology
* **Likelihood of occurrence**: A **weighted** factor based on a subjective **analysis of the probability** that a given **threat or set of threats** is 
capable of **exploiting** a given **vulnerability or set of vulnerabilities**.
* **Impact**: **Magnitude of harm** that can be expected to result from the consequences of unauthorized disclosure of information, 
unauthorized modification of information, unauthorized destruction of information, or loss of information or information system availability.

### Risk Identification
**Recurring process** of identifying different **possible risks**, **characterizing them** and then **estimating their potential** for disrupting the organization.
<br/>
Takeaways to remember about risk identification: 
* Identify risk to communicate it clearly. 
* Employees at all levels of the organization are responsible for identifying risk.
* Identify risk to protect against it. 

### Risk Assessment
The process of **identifying, estimating and prioritizing risks** to an organization’s operations (including its mission, functions, image and reputation),
assets, individuals, other organizations and even the nation.

### Risk Treatment
**Making decisions** about the best actions to take regarding the identified and prioritized risk.
The decisions made are dependent on the **attitude of management** toward risk and the availability — and **cost** — of risk mitigation ( risk appetite or risk tolerance).
<br />
The options commonly used to respond to risk are:
* **Risk avoidance** is the decision to attempt to **eliminate the risk entirely**. 
This could include **ceasing operation for some or all of the activities** of the organization that are exposed to a particular risk.
Organization leadership may choose risk avoidance when the potential **impact of a given risk is too high or if the likelihood of the risk being realized is simply too great**.

* **Risk acceptance** is taking **no action to reduce the likelihood of a risk occurring**. 
Management may opt for conducting the business function that is associated with the risk without any further action on the part of the organization, 
either because the **impact or likelihood of occurrence is negligible**, or because the **benefit is more than enough to offset that risk**.

* **Risk mitigation** is the **most common** type of risk management and includes **taking actions** to prevent or reduce the possibility of a risk event or its impact. 
Mitigation can involve remediation measures, or controls, such as security controls, establishing policies, procedures, and standards to minimize adverse risk. 
Risk **cannot always be mitigated**, but mitigations such as safety measures should always be in place.

* **Risk transference** is the practice of **passing the risk to another party**, who will accept the financial impact of the harm resulting from a risk being realized 
in exchange for payment. Typically, this is an insurance policy.

### Risk Priorities
Prioritize and analyze core risks through:
* **Qualitative risk analysis**:  Low, Medium and High
* **Quantitative risk analysis**: Statistical probabilities and moneterized valuation of loss or gain


![risk matrix](https://learn.isc2.org//content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-70063-techart-risk_management-v01.svg)
**Low likelihood** and a **low impact** might result in a **low priority** <br/>
**High likelihood** and **high impact** will result in a **high priority**

### Risk Tolerance
The level of risk tolerance **varies across organizations**, and even internally: Different departments may have different attitudes toward what is acceptable or unacceptable risk.
Executive management and/or the Board of Directors **determines what is an acceptable level of risk** for the organization. 
Security professionals aim to **maintain the levels of risk** within management’s limit of risk tolerance.

## Module 3: Understand Security Controls

### Security Controls
Security controls pertain to the **physical, technical and administrative mechanisms**
that act as **safeguards or countermeasures** prescribed for an information system **to protect the confidentiality, integrity and availability** of the system and its information. 
The implementation of controls should reduce risk, hopefully to an acceptable level.
<br />
Type of Security  Controls:
* **Physical controls**: Process-based security, **using physical hardware devices**, such as badge readers, architectural features of buildings and facilities, and specific security actions to be taken by people.
* **Technical Controls** (logical controls): Security controls that **computer systems* and **networks** directly implement. These controls can provide automated protection from unauthorized access or misuse, facilitate detection of security violations and support security requirements for applications and data. 
* **Administrative Controls** (managerial controls): **Directives, guidelines or advisories** aimed at the people within the organization. They provide **frameworks, constraints and standards** for human behavior, and should cover the entire scope of the organization’s activities and its interactions with external parties and stakeholders.

## Module 4: Understand Governance Elements and Processes

### Governance Elements
Systems and structures that the organization will use to achieve its goals, they are guided by laws and regulations created by governments to enact public policy.<br />
![Governance](https://learn.isc2.org//content/enforced/9541-CC-SPT-GLOBAL-1ED-1M/build/chapter_01/assets/EDU-ELCC-70060-techart-governance_compilation-v01.svg)

Short summary of each elements in reverse:
* **Procedures**: The detailed steps to **complete a task** that support departmental or organizational **policies**.
* **Policies**: Put in place by organizational governance, such as executive management, to **provide guidance in all activities** to **ensure** that the organization supports industry **standards and regulations**.
* **Standards** : Often used by governance teams to provide a **framework to introduce policies and procedures** in support of **regulations**.
* **Regulations**: Commonly issued in the form of laws, usually from government (not to be confused with governance) and typically carry financial penalties for noncompliance.

#### Regulations and Laws
Regulations and associated fines and penalties can be imposed by governments at the national, regional or local level. 
Because regulations and laws can be imposed and enforced differently in different parts of the world, here are a few examples to connect the concepts to actual regulations.
<br/>
The **Health Insurance Portability and Accountability Act (HIPAA)** of 1996 is an example of a law that governs the use of **protected health information (PHI)** in the United States. 
Violation of the HIPAA rule carries the possibility of **fines and/or imprisonment** for both individuals and companies.
<br/>
The **General Data Protection Regulation (GDPR)** was enacted by the European Union (EU) to **control use of Personally Identifiable Information (PII)** of its citizens and those in the EU

### Standards
Organizations use **multiple standard**s as part of their information systems security programs, both as **compliance documents and as advisories or guidelines**. 
Standards cover a broad range of issues and ideas and may provide assurance that an organization is **operating with policies and procedures that support regulations** and are widely accepted **best practices**.
<br/>
The **International Organization for Standardization (ISO)** develops and publishes **international standards on a variety of technical subjects**,
including information systems and information security, as well as **encryption standards**.
ISO solicits input from the international community of experts to provide input on its standards prior to publishing. Documents outlining ISO standards may be purchased online.
<br/>
The **National Institute of Standards and Technology (NIST)** is a United States government agency under the Department of Commerce and publishes a variety of **technical standards** 
in addition to information technology and information security standards. Many of the standards issued by NIST are requirements for 
U.S. government agencies and are considered **recommended standards by industries worldwide**. NIST standards solicit and integrate input from industry and are 
free to download from the NIST website.
<br/>
**Internet Engineering Task Force (IETF)**, there are standards in **communication protocols** that ensure all computers can connect with each other across borders, 
even when the operators do not speak the same language.
<br/>
The **Institute of Electrical and Electronics Engineers (IEEE)** also sets standards for telecommunications, computer engineering and similar disciplines.

### Policies
Policy is informed by applicable law(s) and specifies which **standards and guidelines** the organization will **follow**. 
Policy is broad, but not detailed; it establishes context and sets out strategic direction and priorities. 
Governance policies are used to moderate and control decision-making, to ensure compliance when necessary and to guide the creation and implementation of other policies.

### Procedures
Procedures define the explicit,  **repeatable activities necessary to accomplish a specific task or set of tasks**.
They provide **supporting data, decision criteria or other explicit knowledge** needed to perform each task.
Procedures can address one-time or infrequent actions or common, regular occurrences. In addition, procedures establish the measurement criteria and methods to use to determine whether a task has been successfully completed. 
Properly documenting procedures and training personnel on how to locate and follow them is necessary for deriving the maximum organizational benefits from procedures.

## Module 5: Understand ISC2 Code of Ethics

### Professional Code Of Conduct

#### Code of Ethics Preamble
The Preamble(Introduction) states the **purpose and intent** of the (ISC)2 Code of Ethics.
* The safety and welfare of society and the common good, duty to our principals, and to each other, requires that we adhere, and be seen to adhere, to the highest ethical standards of behavior.
* Therefore, strict adherence to this Code is a condition of certification. 

#### Code of Ethics Canons
The Canons represent the **important beliefs** held in common by the members of (ISC)2. Cybersecurity professionals who are members of (ISC)2 have a duty to the following four entities in the Canons.  
* Protect society, the common good, necessary public trust and confidence, and the infrastructure.
* Act honorably, honestly, justly, responsibly and legally.
* Provide diligent and competent service to principals.
* Advance and protect the profession.


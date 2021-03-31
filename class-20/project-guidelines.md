# Ops 401 Midterm Project Guidelines

REBUILD

## Conflict Plan

Your team should agree on a process for handing disagreements, should they arise. It is better to have a plan in place ahead of time so you can all refer back to it if necessary.

_Why:_
> Project week can be stressful and emotions can run high. Put together a plan ahead of time so you all know how to deal with any potential issues later.

As a team, create a Group Agreement as a markdown file to document the following:

- What will your group do when it encounters conflict?
- How will you raise concerns to members who are not adequately contributing?
- What is your process to resolve conflicts?
- How and when will you escalate the conflict if your attempts are unsuccessful?

## Communication Plan

Before beginning to tackle the project, determine how your group will communicate with each other.

_Why:_
> This is not an individual effort. Make sure everyone knows how the group will communicate with each other and that everyone feels comfortable speaking up.

Add your communication plan to your Group Agreement. Some things to consider:

- How will you communicate after hours and on the weekend?
- What is your strategy for ensuring everyone's voices are heard?
- How will you ensure that you are creating a safe environment where everyone feels comfortable speaking up?

## Project Scope

Determine which features make up your minimum viable product (MVP). This should include any features you absolutely want to have in your application for presentation day.

_Why:_
> Scope creep can be dangerous! Keeping your project within a pre-determined scope will help the group stay on task without going off on tangents and side features.

Beyond MVP, put together a list of stretch goals to tackle if you have time. During your pitch, your instructor will help you scope your project. Some features may become MVP and some may become stretch goals.

Once you are ready, find your instructor and pitch your idea.

## Daily Team Workflow

As a team, decide how you will work on your project throughout each day.

_Why:_
> Ensure that everyone is on the same page about the current status of the project and the plan for the day.

At the beginning of your day, it is helpful to have a meeting between the team members to make sure that everyone knows what is going on with the project and to discuss the plan for the day. It is wise to have additional check-ins partway through the day and at the end of the day. With every check-in, assess the current percentage of MVP and make a prediction for when your team will reach full MVP.

During your team check-ins, discuss the features each member plans to work on. Determine if the team member will work individually, as a pair, or if the entire team will work on a single feature together, referred to as "mob programming".

Also, use this time to discuss any interpersonal issues that may arise. It is better to address them head-on and resolve any tension rather than allowing it to fester.

## Standup

Every day, the instructional team with circulate to your group for a formal "Standup Meeting". Standup should take approximately 10 minutes per team. Some instructors will opt for a second standup later in the day.

_Why:_
> Standups give the instructional team insight into the current status of your project and the progress the team hopes to make each day.

During standup, each team member will stand up and take turns discussing three points:
> What you personally accomplished yesterday
> What you plan to accomplish today
> Anything that is blocking you from making progress

## Presentation Prep

Your team should practice your presentation prior to the final presentation day. This is typically scheduled by the instructional team. During the practice presentation, the instructional team will provide constructive feedback about the flow of the presentation and appearance of the application.

_Why:_
> If there are any issues in your final product's functionality or appearance, it is better to catch them ahead of time. This is also an opportunity to view the application as it will be shared with the audience. Evaluate any screen size issues, color changes due if you are projecting, and overall impact on the user's experience. The practice round will also allow the team to work on the flow of the presentation as speaking roles are passed from one member to another.

Decide whose computer to use during the presentation and have that computer fully ready for practice session. Make sure you have any cables or adaptors needed, and know what settings are needed to share your screen (and audio, if relevant). Test this computer as the driver of the presentation BEFORE your practice. Test a backup computer as well, just in case.

The presentation should follow exactly from the [template slide deck](https://docs.google.com/presentation/d/1ObrNpOqGhyaKRTIDXnFaIRVKMBGiiCiFkfJJ9T2xi_s/edit#slide=id.g8526846ab1_1_35){:target="_blank"}. Ensure your timing is no more than 15 minutes long, including some time at the end for questions. Present from the final product, deployed site, or offical documentation that you produce. Each member should introduce themselves with their personal pitch. The "About Us" page provides a great backdrop for this portion of the presentation.

Each member of the team must have a speaking part. It is okay to use note cards if you are nervous about forgetting what to talk about. Some of the areas to discuss include:

- An introduction of the project and the problem domain, including the team's solution
- A demonstration of the final product: highlight your organization, functionality, and all deliverables from the requirements
- The team's approach to planning and communication throughout the project
- A technical obstacle or two and how those obstacles were overcome
- A portion of the final application that each team member is particularly proud of

In general, do not show code during the presentation unless the audience asks to see it. Have a code editor open just in case though.

The appropriate dress code is business casual - not too formal and not too casual.

In addition to the scheduled practice session, the team is encouraged to continue to practice on their own. Keep track of the time and adjust accordingly. Practice with the microphone (muting / unmuting, or holding something if in-person) to feel comfortable with it, and practice passing the microphone between team members as you switch speaking roles if in-person.

Speak clearly and do not use slang or profanity. Take it seriously and be professional.

## Grading

This project should highlight comprehension of four major themes:

- Security Operations & Information Assurance
- Data Security
- Cloud & Network Security
- Threat Modeling & Analysis

Each team member's grade is split between their individual effort, and the project's technical merit.

Individual effort is graded based on contributions to project deliverables, and professionalism in the presentation.

Technical merit of the project overall is evaluated according the requirements.

### Scenario

Your team is conducting a case study of a real, documented security incident. Using virtualization tools and publically-available targets, create a working simulation of a cyber attack encompassing all computer security threats to the system and proposing solutions for mitigating threats to attached data resources on the system.

Requirements:

- The real-world incident must provide your team adequate information to develop a case study.
- The target system in your simulation must be an authorized, publically-available testing target, such as the OWASP BWA.
- Do not target live production systems.
- All project conduct must reflect a clear respect for and understand of computer ethics.

### Presentation

Your team will have a 15 minute block to present your case study, target system, proposals and findings. Allocate an additional 5 minutes for freeform Q&A discussion.

Include the below components in your live presentation (in this slide sequence):

- **Introduction**
  - Team Introduction
    - Individual introductions
  - Case study introduction
    - Who, What, When, Where, Why
- **Problem**
  - Introduce the threat actor TTP you are demonstrating today
  - Data flow diagram (DFD) representing your system
  - Threat mapped to the MITRE ATT&CK framework and Atomic Red Team
  - Qualitative risk analysis breakdown
  - Technical demonstration of the attack being executed
- **Proposed solutions**
  - Technical demonstration of a network monitoring system detecting the threat
    - Examples include DLP, IDS/IPS, ICMP-based monitoring
  - Technical demonstration of a Python-scripted security solution or attack
    - Demonstrate protecting data against the threat, or automating the attack simulation of the threat itself (ref. Atomic Red Team)
  - Technical demonstration of an encryption solution to protect company data against the threat
  - Discuss overall findings
  - Summarize operational changes to mitigate threat
- Project challenges
- Q&A

> Tip: Slides should be composed of talking points, not lines to be read verbatim! Avoid the "teleprompter" effect and aim for a natural, extemporaneous presentation on demo day.

### Proposal Deliverable

The following deliverables will be due on demo day.

Required deliverables:

- PD01: Case Study Overview
  - Incident narrative
  - Why your team selected this incident
  - Resources/assets as part of evaluated target
- PD02: Security Assesment Report (SAR) as PDF document
  - Include all solutions.
- PD03: STRIDE/DREAD Analysis
- PD04: Threat Model Technical Report
  - Threat analyzed using the Lockheed Martin Cyber Kill Chain
  - Threat modelled into a data flow diagram (DFD) of STRIDE and DREAD
  - Example tabletop scenario including likely human behaviors of involved parties
  - Thoroughly describe the threat model and adversary behavior in a dedicated document.
- PD05: Proposed standard operating procedure (SOP) for your NOC or SOC team to better handle the described threat in the future.
  - Follow NIST Risk Management Framework workflow in designing the SOP.
- PD06: GitHub Repo Link to individual Python-based automation tool (one per team member)

### Individual Contributions

Individual team members must track their project contributions. Each individual should carefully document contributions to the following, and include this in your Canvas "Individual Submission" assignment.

- Python automation script exclusively written by the individual
  - The script should fit the project scenario but differ in some meaningful fashion from the scripts we made in class. For example, different types of target for the attack, or different types of methods used on the target.
  - It is OK to include multiple scripts in the demo.
  - The script should adhere to commenting norms established in class, such as creator, date, description, etc.
  - Explain in script comments how your script differs from in-class examples and Ops Challenges.
  - Explain in script comments how the script fits into the overall project scenario.
- Demonstrate you completed an equal share of project documentation tasks.
  - Creation and editing of reporting deliverables
  - Creation and editing of slide decks
  - Creation and editing of threat analysis and modeling
- Demonstrate you contributed an equal share of technical attack simulation construction and operation.
  - Staging the ToE
  - Constructing, automating or performing the attack TTP
  - Evaluating ToE response to attack and implementing technical solution
    - Python-based automation script
    - Defensive encryption solution

### Resources

Reference the below resources for developing your security assessment report.

- [Tips for Creating a Strong Cybersecurity Assessment Report](https://zeltser.com/security-assessment-report-cheat-sheet/)
- [CMS Security Assessment Report Template](https://www.cms.gov/Research-Statistics-Data-and-Systems/CMS-Information-Technology/InformationSecurity/Downloads/Security-Assessment-Report-Template.docx)
- [Security Assessment Report Example](https://www.silabs.com/documents/public/white-papers/SP02508-Sigma-Designs-Security2-Command-Class_v2_Commercial_in_Confidence_Removed.pdf)

Reference the below resources for developing your STRIDE/DREAD analysis.

- [Qualitative Risk Analysis with the DREAD Model](https://resources.infosecinstitute.com/qualitative-risk-analysis-dread-model/)
- [STRIDE/DREAD Analysis: Threat Modelling of Trinity Wallet Example](https://files.iota.org/trinity/Threat+Modelling+Report+V1.2.signed.pdf)

Reference the below resources for developing your threat model technical report.

- [Enterprise Threat Model Technical Report Example](https://www.mitre.org/sites/default/files/publications/pr_18-1613-ngci-enterprise-threat-model-technical-report.pdf)

Reference the below resources for developing your NOC/SOC SOP.

- [Guideline to Develop and Maintain the Security Operation Center (SOC)](https://resources.infosecinstitute.com/guideline-to-develop-and-maintain-the-security-operation-center-soc/)
- [NIST Risk Management Framework Overview](https://www.nist.gov/system/files/documents/2018/03/28/vickie_nist_risk_management_framework_overview-hpc.pdf)

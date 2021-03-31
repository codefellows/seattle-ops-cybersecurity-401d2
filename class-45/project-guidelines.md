# Ops 401 Final Project Guidelines

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

For this project you will be composing the following:

- Demo day presentation slide deck
- Pentest Report
- Threat Intelligence & Incident Response Report
- GitHub repo containing individual automation script contributions

Unlike previous projects, there is no project pitch assignment. However, do formulate a plan of action with your team as to how you will all contribute to each aspect of the project.

## Daily Team Workflow

As a team, decide how you will work on your project throughout each day.

_Why:_
> Ensure that everyone is on the same page about the current status of the project and the plan for the day.

At the beginning of your day, it is helpful to have a meeting between the team members to make sure that everyone knows what is going on with the project and to discuss the plan for the day. Assess the current percentage of project completion.

During your team check-ins, discuss the operations each member plans to work on. Determine if the team member will work individually, as a pair, or if the entire team will work on a single task together.

Also, use this time to discuss any interpersonal issues that may arise. It is better to address them head-on and resolve any tension rather than allowing it to fester.

## Standup

Every day, the instructional team with circulate to your group for a formal "Standup Meeting". Standup should take approximately 10 minutes per team. Some instructors will opt for a second standup later in the day.

_Why:_
> Standups give the instructional team insight into the current status of your project and the progress the team hopes to make each day.

During standup, each team member will stand up and take turns discussing three points:

> - What you personally accomplished yesterday
> - What you plan to accomplish today
> - Anything that is blocking you from making progress

## Presentation Prep

Your team should practice your presentation prior to the final presentation day. This is typically scheduled by the instructional team. During the practice presentation, the instructional team will provide constructive feedback about the flow and appearance of the presentation.

_Why:_
> Evaluate any screen size issues, color changes due if you are projecting, and overall impact on the user's experience. The practice round will also allow the team to work on the flow of the presentation as speaking roles are passed from one member to another. Ensure that your remote audience is able to see and hear what they need to.

Decide whose computer to use during the presentation and have that computer fully ready for practice session. Make sure you have any cables or adaptors needed, and know what settings are needed to share your screen (and audio, if relevant). Test this computer as the driver of the presentation BEFORE your practice. Test a backup computer as well, just in case.

The presentation should follow exactly from the [template slide deck](https://docs.google.com/presentation/d/1ObrNpOqGhyaKRTIDXnFaIRVKMBGiiCiFkfJJ9T2xi_s/edit#slide=id.g8526846ab1_1_35){:target="_blank"}. Ensure your timing is no more than 15 minutes long, including some time at the end for questions. Present from the final product, deployed site, or offical documentation that you produce. Each member should introduce themselves with their personal pitch. The "About Us" page provides a great backdrop for this portion of the presentation.

Each member of the team must have a speaking part. It is okay to use note cards if you are nervous about forgetting what to talk about. Some of the areas to discuss include:

- An introduction of the project and the problem domain, including the team's solution
- A demonstration of the final product: highlight your organization, functionality, and all deliverables from the requirements
- The team's approach to planning and communication throughout the project
- A technical obstacle or two and how those obstacles were overcome
- A portion of the final project that each team member is particularly proud of

The appropriate dress code is business casual - not too formal and not too casual.

In addition to the scheduled practice session, the team is encouraged to continue to practice on their own. Keep track of the time and adjust accordingly. Practice with the microphone (muting / unmuting, or holding something if in-person) to feel comfortable with it, and practice passing the microphone between team members as you switch speaking roles if in-person.

Speak clearly and do not use slang or profanity. Take it seriously and be professional.

## Learning Objectives

- Incident Response & SIEM
  - The team demonstrates an appreciation and technical grasp of how automated log aggregation and threat detection solutions contribute to the incident response process.
- Malware
  - The team is capable of advanced malware analysis and detection, beyond the typical "off-the-shelf" antimalware solutions.
- Appsec & Vulnerability Analysis
  - The team demonstrates proficiency with web app pentesting tools and is able to identify and exploit vulnerable web apps.
- Penetration Testing
  - The team is able to perform a full network penetration test and document all findings.

## Grading

Each team member's grade is split between their individual effort, and the project's technical merit.

Individual effort is graded based on contributions to project deliverables, and professionalism in the presentation.

Technical merit of the project overall is evaluated according the requirements.

## Scenario

Your team is a small security firm that accepted a new contract to help ABC Corp. test its infrastructure and implement more sophisticated security systems. This is a "purple team" engagement. You have been tasked with completing a penetration test, composing relevant deliverables, and presenting the findings to your client. You will also be implementing threat detection and advance malware analysis tools in the environment as part of boosting the client's defenses.

> If you're applying for an offensive security role, you'll commonly be asked to perform a full pentest and compose a report for the hiring company. This project is your chance to get ahead of the curve and get yourself some valuable practice in advance of your job search!

Your team will be provided a access to a unique black box AWS cloud instance for penetration testing.

Refer to the rules of engagement to dictate the behaviors and scope of the penetration test.

### Staging

Prepare your Kali Linux VM to connect with the target network, ABC Corp's web app, using OpenVPN.

- Install OpenVPN.
- Obtain a .ovpn file from your instructor. Treat this file like a password; do not share with others.
- Establish connectivity to the web app using OpenVPN. Contact your TA or instructor if you have any problems with this step.

All scanning and pentesting traffic should be routed through your VPN connection, and not over public Internet channels.

### Project Week Part 1

The first two days of project week will be devoted to the penetration test, starting with the web app.

- Initiate the VPN connection in order to access the target network.
- Use your findings from each target system to access the next target system ("pivoting").

> This is it: The grand finale! Use everything you've learned in this course to circumvent the defenses. As always, document your findings for inclusion in your final report deliverable and demo day presentation. Also, try not to break any of the systems you target; a common saying in the industry points out that this is the difference between an amateur and a professional: The ability to pentest without damaging the targets.

### Project Week Part 2

In the final segment of the project week, your team will gain access to ABC Corp's systems and implement defensive systems in the environment.

- At least one SIEM solution.
  - The implemented SIEM should successfully aggregate logs from various servers and/or endpoints to facililate the demonstration of your sample threat.
- At least one threat detection system.
  - The implemented system should raise alerts that a threat is present on the network.
- At least one advanced malware analysis or detection system.
  - An advanced malware tool or technique must be implemented purposefully and presented as part of demo day.
  - An "advanced" tool goes beyond mere out-of-box antimalware products and demonstrates a technical understanding of how malware signatures and behaviors can be detected.

> Take care in selecting your software solutions; review the below demo day requirements to ensure the topics "flow" nicely. A general pattern to reproduce is Alert -> Investigation of logs and PCAP -> Detection of malware payload using advanced techniques. You'll also want to select for extensible software that can give your team options in contributing scripts.

Your team will then introduce a security threat to the environment involving the delivery of a malware payload and capture the alerts and PCAP of the threat. Similar to the threat hunting lab from class, you'll need to simulate the detection and remediation of a payload-based threat for demo day and report deliverable.

### Scripting and Automation

Each team member must individually contribute a script that facilitates some aspect of the scenario.

- While it is acceptable to make use of existing tools and libraries, the submitted script should demonstrate an innovative new application of automation compared to techniques demonstrated in class, as well as represent a significant portion of the student's original code.
- Ideas for your script:
  - Custom threat detection
  - Custom vulnerability detection
  - Custom malware detection
- Not all scripts need to be presented on demo day.

> The security industry is rapidly learning to appreciate the value added by automated systems. Most internal security teams are understaffed and underfunded; in many cases, the time invested in automating a security process is well worth the effort and resources if it reduces the human-involved workload. For this reason, this course has introduced you to many open-source, extensible security solutions that can be implemented in a variety of environments and tailored to the needs of the client company.

### Demo Day

On demo day, your team will present a slide deck consisting of the following:

- Team introduction
- Tools and techniques used as part of the penetration test
- Penetration test findings
  - Web application vulnerabilities discovered
  - Network systems vulnerabilities discovered
- Defensive systems implemented
  - Event aggregation
  - Malware analysis or detection
- Live demo of a defensive system implemented
  - Alerts that led to the detection of a threat
  - Network traffic evidence of the threat presented in a PCAP file
  - Process applied to detect and deal with the threat
  - An advanced malware detection or analysis technique
- Team outro

### Deliverables

The following forms of report deliverables will be due on demo day to Canvas for grading.

- PD01: Completed [Penetration test report](https://www.offensive-security.com/reports/sample-penetration-testing-report.pdf)
  - Summarize your findings from Part 1.
- PD02: Completed [Threat intelligence and incident response report](https://zeltser.com/cyber-threat-intel-and-ir-report-template/)
  - Summarize the systems implemented in Part 2 and how you dealt with the sample threat.
- PD03: Link to team's GitHub code repository clearly indicating individual controbutions to scripting and automation efforts.

Upon the conclusion of demo day, access to the lab environment will be revoked.

### Resources

Reference the below resources for developing your penetration test report.

- [Writing or Receiving Your First Pentest Report](https://blog.zsec.uk/ltr101-pentest-reporting/)
- [Template OSCP Penetration Test Report](https://www.offensive-security.com/pwk-online/PWKv1-REPORT.doc)
- [Example OSCP Penetration Test Report](https://www.offensive-security.com/reports/sample-penetration-testing-report.pdf)

# Interview 02: Windows Attack Techniques

## Interview Question

This interview will test the candidate's comprehension of attack techniques used against the Windows OS.

Begin the interview with some warmup questions.

- "Windows is a common attack surface, given its ubiquitous adoption in the desktop and enterprise marketplace. For this interview, I'll be asking you some questions about various attack techniques targeting Windows OS. How does Windows manage user identities and authentication? In your response, please address the terms 'Kerberos,' 'Active Directory,' and 'Domain.'"

- "What are some obsolete features in Windows 10 that, if activated, will cause known security vulnerabilities?"

Share this piece of code with the candidate. When they are ready, proceed.

```unknown
meterpreter > getsystem -h
Usage: getsystem [options]

Attempt to elevate your privilege to that of local system.

OPTIONS:

  -h        Help Banner.
  -t   The technique to use. (Default to '0').
  0 : All techniques available
  1 : Service - Named Pipe Impersonation (In Memory/Admin)
  2 : Service - Named Pipe Impersonation (Dropper/Admin)
  3 : Service - Token Duplication (In Memory/Admin)

meterpreter >
```

- "This is a sample console from a penetration tester executing Meterpreter. What is the general term for the type of exploit demonstrated here, and why would an attacker use this technique on a targeted system?"
  - Candidate should name the appropriate type of attack this is, and describe how it fits into an overall pentest or cyber attack effort.

Share this [terminal screenshot](https://pentestlab.files.wordpress.com/2018/04/golden-ticket-shell-with-psexec-as-invalid-user.png?w=760){:target="_blank"} with the candidate and proceed when they are ready.

- "This image depicts a malicious attack taking place against another Windows computer. What is the victim computer's domain, username, and system name? Please also explain how this attack is executed."
  - Candidate should identify the appropriate pieces of information, then go on to descibe the stages of a remote code execution or pass the hash attack.

Evaluate how well the candidate explained Windows OS security and related attack techniques.

## Specifications

- Score the candidate according to the [Technical Ops Interview Rubric](https://docs.google.com/spreadsheets/d/1scthkmARfzAFZrSYAp6LA2coOaoWUWbSzMbtIU4jcHw/edit#gid=1422288328){:target="_blank"}
- You are free to offer suggestions or guidance (and see how they respond),  but don't solve it for the candidate

## Structure

Familiarize yourself with the grading rubric, so you know how to score the interview.

Look for effective problem solving, efficient use of time, and effective communication with the whiteboard space available.

Every solution might look a little different, but the candidate should be able to verify their solution with different edge cases to verify correctness.

Assign points for each item on the Rubric, according to how well the candidate executed on that skill.

Add up all the points at the end, and record the total at the bottom of the page. Include a photo or screenshot of their whiteboard.

## Documentation

Record detailed notes on the rubric, to share with the candidate when the interview is complete.

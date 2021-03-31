# Interview 02

Web application security has become a new frontier in the battle for computer security, as the world aggressively adopts increasingly sophisticated web applications to meet the needs of the modern era. Think of the last time you made an online purchase, checked your bank account, accessed social media, or used a search engine; web apps are the engines behind all of these day-to-day tasks and more. This three-stage interview topic will challenge the candidate on the topic of web application security scanning tools, namely ZAP.

> In 2019, there was an attack launched against a website on an average of every 39 seconds. Wordpress, the most popular method of creating web sites in recent years, reported that the most common vulnerabilities amongst Wordpress plugins were XSS and SQL injection. Source: [WebARX](https://www.webarxsecurity.com/website-hacking-statistics-2018-february/){:target="_blank"}

## Interview Question

Send the candidate the link to the [ZAP alerts image](https://www.randorisec.fr/img/blog/zap_alerts.png){:target="_blank"}. When the candidate confirms the link is working and has reviewed the image, proceed.

Ask the candidate:

- Why does ZAP consider this a high priority alert?
- Explain the technique used by ZAP to determine the target is vulnerable to SQL injection.
- How would you test for SQLi vulnerabilities using a tool outside of ZAP?

> Reading alerts and interpreting them is a vital skill to nurture as a junior security professional.

Send the candidate the link to the [ZAP spider output image](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.stack.imgur.com%2FREfnl.png&f=1&nofb=1){:target="_blank"}. When the candidate confirms the link is working and has reviewed the image, proceed.

Ask the candidate:

- This is a sample output from a ZAP scan. What ZAP component was used to generate this output, and what is depicted here?
- What does "OUT_OF_SCOPE" mean?
- Why do web app security testing tools like ZAP crawl directories?

Show the candidate this Python code sample. Give the candidate a moment to read over it, then proceed.

```python
def get_all_forms(url):
    soup = bs(s.get(url).content, "html.parser")
    return soup.find_all("form")
```

> Not all security professionals are coders, but you'll need the ability to read code found in security tooling, malware, forensic evidence, network traffic, and other computer systems, as well as understand basic concepts such as functions and loops.

Ask the candidate:

- What is Beautiful Soup, and what does this function do?
- What kinds of web application vulnerabilities can this script potentially detect, if further developed?
- How can web application security tools be improved upon?

Evaluate the candidate's proficiency and comprehansion of web application security tooling.

## Specifications

- Read all of the following instructions carefully.
- Act as an interviewer, giving a candidate the interview question(s)
- Score the candidate according to the [Whiteboard Ops Interview Rubric](https://docs.google.com/spreadsheets/d/1scthkmARfzAFZrSYAp6LA2coOaoWUWbSzMbtIU4jcHw/edit#gid=1422288328){:target="_blank"}
- You are free to offer suggestions or guidance (and see how they respond),  but don't solve it for the candidate

## Structure

Familiarize yourself with the grading rubric, so you know how to score the interview.

Look for effective problem solving, efficient use of time, and effective communication with the whiteboard space available.

Every solution might look a little different, but the candidate should be able to verify their solution with different edge cases to verify correctness.

Assign points for each item on the Rubric, according to how well the candidate executed on that skill.

Add up all the points at the end, and record the total at the bottom of the page. Include a photo or screenshot of their whiteboard.

## Documentation

Record detailed notes on the rubric, to share with the candidate when the interview is complete.

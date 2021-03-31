# Interview 02

## Interview Question

First, have the candidate download <https://www.malware-traffic-analysis.net/2020/09/25/2020-09-25-traffic-analysis-exercise-alerts.zip> to their FLARE VM and unzip it with the password 'infected'. Let the candidate know this package does not contain malware. Wait until this is complete before proceeding, as these files are a part of today's technical interview.

When the candidate is ready, ask them these questions one at a time:

- Describe the security incident that occurred based on your observations of the alert logs provided.
- If 10.0.0.0/24 is the company's subnet, what IP is the origin of the malware?
- How did the malware enter the system?
- What does the Trojan do? Feel free to use all resources at your disposal to answer this question.

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

## Example Info

| Input | Output |
|-----|----|
| `head->[3]->[2]->[1]` | `head->[1]->[2]->[3]` |
| `head->['a']->['b']->['c']` | `head->['c']->['b']->['a']` |

## Documentation

Record detailed notes on the rubric, to share with the candidate when the interview is complete.

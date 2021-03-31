# Interview 01

The candidate selection process for a security role can take many forms. This interview topic consists of three "stages" designed to represent some of the challenges an applicant will face when being scrutinized for their comprehension and proficiency in cyber topics and tooling. If the candidate provides a murky or elusive response to these questions, try to test their more foundational understanding of the concepts by asking questions around more basic concepts.

> "Nearly three quarters of large companies in Europe and North America were hit by online cyber attacks in 2019 with cross-site scripting used in 40 percent of incidents. Most XSS attacks are performed by using a web application to send malicious code, usually as a browser side script, to a different end-user. SQL injection was the second most used attack vector globally at a 13.5 percent share, followed by fuzzing at 7.5 percent, business logic at 6.4 percent and information gathering at 5.8 percent." -[MSSP Alert](https://www.msspalert.com/cybersecurity-research/study-cross-site-scripting-attacks/){:target="_blank"}

## Interview Question

Show the candidate this piece of code. Give the candidate a moment to read the code and let you know they're ready to discuss.

```html
<script type=”text/javascript”>
var test=’../example.php?cookie_data=’+escape(document.cookie);
</script>
```

Ask the candidate:

- What type of attack is taking place in this code?
- What is the attacker hoping to accomplish by injecting this code into a web app?
- How can this vulnerability be detected on a web app?

Send the candidate the link to [XSS Game Level 1](https://xss-game.appspot.com/level1){:target="_blank"}.

Ask the candidate:

- Please share your screen of the provided web site and demonstrate how a XSS attack is executed.
- Explain in your own words why this attack works.

> Being asked to demonstrate your proficiency in a technical skill is a common hoop you'll jump through as a cyber job applicant. Get ready to demonstrate your technical chops in both the interview as well as during any technical testing the organization subjects you to. You also may not always have the luxury of consulting outside resources.

Show the candidate this piece of code. Give the candidate a moment to read the code and let you know they're ready to discuss.

```php
$safe_data=filter_input(INPUT_GET, 'comment', FILTER_SANITIZE_SPECIAL_CHARS);
```

Ask the candidate:

- What technique is demonstrated in this code?
- How does this code help protect against the web application vulnerability we've discussed today?
- Finally, how are newly-discovered vulnerabilities documented by the security community at large?

How well did the candidate demonstrate technical proficiency as well as communicate knowledge of the XSS attack technique?

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

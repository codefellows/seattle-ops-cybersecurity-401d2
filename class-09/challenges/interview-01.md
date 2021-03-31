# Interview 01

## Interview Question

Ask the candidate: 

- As a security control, what risk does encryption mitigate? 
  - Please provide an example of a security control that incorporates encryption.
  - How much is the risk reduced? Is the risk eliminated?
- Under what two circumstances can data be encrypted?
  - When should data be encrypted and why? Should everything, therefore, be encrypted?
  - How difficult is it to circumvent encryption?
- What’s the difference between encoding, encryption, and hashing? Are they the same?
  - Define and discuss:
    - Encoding
    - Encryption
    - Hashing

## Interviewer Notes

Key areas to explore and discuss:
- Data **encryption** is a confidentiality security control designed to mitigate the risk of unwanted data exposure. As we learned in Ops 101, exposure can lead to further cyber attack.
  - An example of an encryption security control is encrypting traffic (data in motion) to cloud resources using VPN. Assuming a sufficiently complex encryption cipher is used, this greatly reduces the chances that an outsider will be able to view the encrypted data. While the risk of data exposure is significantly reduced, nothing fully eliminates the risk (aside from not transmitting data at all!).
- Data can be encrypted either **at rest** or **in motion**. 
  - Encrypting all data is not always practical. Controlled data types that are a part of a confidentiality compliance requirement, or data that if exfilitrated would cause the company harm, should likely be encrypted both at rest and in motion.
  - Decrypting older ciphers can be performed with sufficient computing power. Therefore, modern ciphers that are generally considered secure should be chosen.
- Encoding, encryption and hashing are indeed different processes.
  - **Encoding** is the conversion of data from one format to another format, and is not considered a security control.
  - **Encryption** ensures the confidentiality of data by mathematically transforming the data into an unreadable format.
  - **Hashing** protects the integrity of your data via the hash validation process by generating a unique string that the data recipient also generates to validate the integrity of the data.

## Preparation

Before the interview:
- Carefully review the interview question and interviewer notes.
- Create your own copy of [Whiteboard Ops Interview Rubric](https://docs.google.com/spreadsheets/d/1scthkmARfzAFZrSYAp6LA2coOaoWUWbSzMbtIU4jcHw/edit#gid=1422288328){:target="_blank"}
- Fill in the details at the top, such as Student and Interviewer
- Familiarize yourself with the grading rubric, so you know how to score the interview. Review the criteria in advance of the interview so you can steer the conversation towards the scoring requirements.

## During the Interview

- Act as an interviewer, giving a candidate the interview question(s)
- Score the candidate according to the rubric
  - Assign points for each item on the rubric, according to how well the candidate executed on that skill.
- You are free to offer suggestions or guidance (and see how they respond),  but don't solve it for the candidate
- Every solution might look and sound a little different, but the candidate should be able to verify their solution with different edge cases to verify correctness. The candidate should NOT be reading notes verbatim; instead, quesitions should be answered as authentically as possible.

## After the interview

- Add up all the points at the end, and record the total at the bottom of the page. Include a photo or screenshot of their whiteboard.
- Record detailed notes on the rubric, to share with the candidate when the interview is complete.

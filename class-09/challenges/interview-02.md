# Interview 01

## Interview Question

- Ask the candidate: 
  - What is PKI?
    - Is PKI symmetric or asymmetric and why?
    - Provide an example of PKI in action, and compose a drawing or diagram using draw.io or Zoom whiteboard.
  - What’s the difference between symmetric and public-key cryptography?

## Interviewer Notes

- **PKI** stands for public key infrastructure, a system that utilizes public keys, private keys, and digital certificates to protect data, vouch for user identities/devices/applications, and secure communications end-to-end.
  - PKI is a form of **asymmetric key cryptography** because it uses two different keys, a public and private key. The sender never knows/possesses the private key.
  - One example use of PKI is to encrypt a message using the recipient's public key. After the message is encrypted, only the recipient can decrypt it by using the private/secret key. Here is how this would look in a diagram:
    
    ![pki.jpg](../assets/pki.jpg)

  - Another example is when you visit a website with an SSL certificate installed via HTTPS protocol. The SSL certificate helps create a secure connection between a website’s server and a client (visitor) browser. Data sent over this connection is encrypted, which means that regular plaintext is turned into ciphertext, rendering it unreadable. 

- **Symmetric key cryptography** uses the same secret key for both encryption and decryption of the data. This secret key is shared by the recipient and the sender.

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

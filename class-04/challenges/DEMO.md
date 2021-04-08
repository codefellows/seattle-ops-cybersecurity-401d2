# Interview Demo

## Interview Question

Ask the candidate: 
- What is a three-way handshake and how does it work? 
  - Please illustrate the process using a screenshare and drawing tool of your choosing.
- What protocol is used?
- What type of connection is this, one-way or two-way, and what is the technical term for that?
- Why should security professionals know how this works?

## Interviewer Notes

Key areas to explore and discuss:
- A three-way handshake is a method used in a TCP/IP network to create a connection between a host and a client. It’s called a three-way handshake because it is a three-step method in which the client and server exchanges packets. The three steps are as follows:
  - The client sends a SYN(Synchronize) packet to the server check if the server is up or has open ports
  - The server sends SYN-ACK packet to the client if it has open ports
  - The client acknowledges this and sends an ACK(Acknowledgment) packet back to the server, and the connection is established.
- The three-way handshake uses the TCP protocol. 
- This is a duplex (two-way traffic) connection.
- The three-way handshake can be exploited in a number of ways, for example by a flood attack.  Specially-crafted packets with the TCP receive window size set to a very small value can overwhelm the server and cause denial of service.

## Preparation

Before the interview:
- Carefully review the interview question and interviewer notes.
- Create your own copy of [Whiteboard Ops Interview Rubric](https://docs.google.com/spreadsheets/d/1scthkmARfzAFZrSYAp6LA2coOaoWUWbSzMbtIU4jcHw/edit#gid=1422288328)
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

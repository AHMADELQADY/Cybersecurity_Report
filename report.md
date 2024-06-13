# Cybersecurity OSWAP Juice Shop Report
## Introduction

In this demo, I chose to use OSWAP Juice Shop as a target to experiment with Burp and other tools by doing the offered challenges. Initially, I tried to solve the challenges on my own by thinking about the solutions I thought about how to solve the challenges, but I had to use online tutorials to help me with the technical part.

This report is organized in:
- Challenges name followed by the description and the solution.
- The order of the challenges in the report corresponds to the order of the challenges in the demo.
- The tools I used for writing the report and building the demo are listed at the end of the page.

To be noticed that:
- The Audio in the demo was added after the edit of the video.
- The demo was edited and there are scenes that were cut in which there were the trials to solve the challenge.
- The work in the demo wasn’t done entirely by me since I watched the online tutorials (but I tried and got to some solutions but couldn’t do the technical part).

## Challenges from the Score Board

### Change Bender's Password

**Description**: Change Bender's password into slurmCIssic without using SQL Injection or Forgot Password.

**Solution**: To solve this challenge, I first identified the target’s email by analyzing the reviews. Using SQL injection, I was able to log in. Then by inspecting the password change request with Burp, I removed the "current password" field and forwarded the request. Due to OWASP's vulnerability, this method successfully bypassed the password change requirement.




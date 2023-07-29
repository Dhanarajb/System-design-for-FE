# System-design-for-FE
# TOC:

1. Why system design for FE
2. What do interviewers look for
3. Important Topics
4. UI/UX
5. Frameworks, and technologies choices
6. Example
7. Strategy

# Why system design for Front-End?

Front-End is getting complex day by day.The line between Backend and Front-End is fading out. As well as, it is expected that Front-End should contribute to the design decisions of the project. Front-End developers should flag in the design meetings if Backend/APIs folks are ignoring any important aspect in the design.

# What interviewers are looking for?

As a Front-End developer do you understand

1. How the application should be designed E2E?
2. What are the important parts of any application?
3. Do you understand which resource is the right fit and why
4. Do you understand the pros-cons of the design decisions
5. Do you understand what is required from the backend/APIs folks to make your Front-End
6. Do you understand the cost (price) of designing an application and how to optimize it?
7. Are you able to design a micro-service
8. Are you able to design micro-frontends
9. How to create and scalable repos

# What are the important topics?

1. Database
2. CDN
3. APIs
4. Storage - S3, EC2, EBS
5. Deployment
6. Route53
7. Certificates
8. Analytics
9. Monitoring
10. Logs
11. Data Recovery
12. Performance
13. accessibility
14. cross-browser
15. SPoF (Single Point of Failure)
16. Scalable
17. Security
18. Micro-frontends
19. SEO
20. Reliability
21. Maintainability

# Is UI/UX is part of the system design? If yes, then what to talk about

Yes, as a Front-End developer you should talk about UI/UX. Talk about how the UX would be?

# It is important to talk about

1. Performance: How your design decision is going to improve performance
2. Accessibility: This will come when you will talk about UI and UX.
3. Cross-browser: If any tech decision is going to impact any browser (do call out)
4. SPoF: Single point of failure: How to avoid it
5. Scalable: How scalable your solution is
6. Security: Most important aspect, how you are going to take care of security
7. Data State: How to maintain the data consistency between mobile and desktop

# Shall we talk about the frameworks choices and technology choices?

Yes, it is important to talk about it. But your all decision should not be based on the frameworks you are aware of. You should focus on the solution not based on what frameworks you know.

Also, this is an important aspect of the interview. So, you should be well versed with the pros-cons of all the technology decisions you are taking.

Eg: why a non-relational database over a relational database? Why EC2 and not Lambda function? ReactJS vs Angular? SSR vs CSR etc.

# How deep-dive one should go?

1. At first, focus on solving the problem (not on the BEST solution).
2. Then focus on optimising the solution. Talk about - BEST solution and why (pros and cons, what area would be impacted? Eg: performance will increase, SPoF will be avoided, etc.
3. Now, go deep dive into the modules related to the front-end. For example: do talk about APIs endpoints, cache or local storage or DB, which DB, deployment and storage of the web app.
4. An interviewer will stop you in between to ask questions. Give them time and space to them to ask the questions.

# Example

3 You need to design a chat application.

1. A user can do multiple chats with multiple users
2. A user can be added to a group
3. A user can be able to react with emojis on the chat(s)
4. A user can be able to reply to the chat 1:1
5. and a few more requirements
6. 
# Step 1: Define the Scope:

1. How many users are we expecting?
2. How many chats in parallel can be done?
3. How long is the History of chats to be maintained?
4. Which emojis are to be used, and their functionality? eg: toggle, or how they will be viewed, do we need to maintain in the history of chat etc.
5. Do we support multiple user chats?
6. Come with numbers to know the scalability, performance, resources required etc.
# OUTCOME: You should be aware of the scope and scale of the problem

# Step 2: Think about solutions, Features, and Resources

1. Start from web or mobile (where you feel comfortable or as per the ask of the interviewer)
2. What problem we are solving here? You can’t solve all the problems in one go. So, think about the top 2-3 and start focusing on that.
3. Think about resources that will be used to make a useable system
# OUTCOME: You should be clear with 2-3 top requirements and what resources you will be requiring

# Step 3: Let's start with the High-level design (Front-End + Back-End)

1. Web interaction
2. Endpoints
3. Database
4. Authentication
5. Storage
# OUTCOME: You should have a useable working design solving the top 2-3 problems.

# Step 4: Let’s, deep dive, and optimize

# Question: What will happen when the user is offline for a month. How you will design the experience for it? (talk about UX and UI)

1. accessibility
2. Performance
3. Scalability
4. How to scale the design
5. How the older chats will be retrieved
6. API design etc.
# OUTCOME: An optimised design of the problem with clear pros and cons.

#Strategy:

#The system design round is 60 mins approx.
1. 5 mins to share problem statement
2. 40 mins to solve questions
3. 5 mins for Q&A.

# You must do practice to place everything in 40 mins. Before the interview does practice as much as you can. You should use either whiteboard, paper, or any application such as draw.io

1. Make your 40 mins interactive. Keep talking and thinking aloud. It is important talk aloud about what you are thinking and why?
2. There is no correct or incorrect answer. System design is all about knowing you and your design decision skills.
3. As a Front End developer, the scope would be vast. So, better to talk about scope. Ask - where do you want me to focus? Eg: Shall I just skip the FE part in detail and get into the deep of the backend, or infra or deployment etc.
4. Go in the details of connecting the modules and user-journey. Eg: Where the user’s data would be stored, which API endpoint will be used to get the data, how the scalability of the storage of the user’s data if the user will increase from 10x to 100x

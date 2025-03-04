﻿
## SECTION 1 : PROJECT TITLE
## Intelligent Covid Detection and Chatbot Platform

<img src="SystemCode/CoviDetector/recommender/static/images/project_logo.PNG"
     style="float: left; margin-right: 0px;" />

<img src="SystemCode/CoviDetector/recommender/static/images/project_main_page.PNG"
     style="float: left; margin-right: 0px;" />

<img src="SystemCode/CoviDetector/recommender/static/images/project_chatbot_page.PNG"
     style="float: left; margin-right: 0px;" />

---

## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT
With the recent low number of community cases of covid-19, mass gathering is allowed. However, participants will have to take an antigen rapid test for Covid-19 and obtain a negative result before admission. Hence, the event planner must ensure the participants safety/health condition before allowing participants to enter the event venue. This project proposes a solution to this problem by using a machine learning model to determine the likelihood of participants having Covid-19. In addition, it includes a chatbot to allow the participants to know current information about Covid-19 and the event itself. 

Recent news reported that the Singapore government allowed mass gathering but with a requirement. Before a participant can enter the venue, the event organizer has to ensure that he/she is not contacted with Covid-19. To implement this, the event organizer will have to check with each participant individually on their health status before letting them in. As social distancing enforcement is a must, a long queue will be expected. Meaning, more manpower is needed to maintain the queue. If a shorter time can be implemented to handle these, the queue will be shorted thus lesser manpower is needed.

We propose that this can be handled with a web application (mobile-friendly) that has a survey for the participants to answer to get their health status. Participants with a mobile device would be able to answer the necessary questions before reaching the front of the queue. The result of the survey will let the queue maintainer either guide the participant to the swab test area or let the participant into the venue. Moreover, it also includes a chatbot that allows the user to know (real-time) information about Covid-19 and the event itself. This may keep the participants occupied while waiting for their turn to enter the venue. The solution may be tailored to suit different types of events.


---

## SECTION 3 : CREDITS / PROJECT CONTRIBUTION

| Official Full Name  | NRIC  | <div style="width:400px">Work Items</div> | Email |
| :------------ |:---------------:| :----------------------------------| :---------------|
| Hong Xiaohui | S****943D | Team Lead, Architecture Design, Predictive Model Development, Chatbot Development, Web Service Implementation, Project Report Generation | xiaohui.hong@ncs.com.sg |
| Anita Koo Shi Qi | S****480B | Webscrape Development and Project Report Generation| anita.koo@ncs.com.sg |
| Sanjeven Ramakrishnan | S****938E | User interface design, Questionnaire and Chatbot integration, OS and browser compatibility testing, Installation and user guide report generation | sanjeven.ramakrishnan@ncs.com.sg |

---

## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO

### [ 1 ] Video clip to promote our system
[![IRS PM 2021 05 01 IS03PT GRP 3Musketeers CoviDetector promotion](https://i.ytimg.com/vi/H4C6DA7kmQo/hqdefault.jpg)](https://youtu.be/H4C6DA7kmQo "IRS PM 2021 05 01 IS03PT GRP 3Musketeers CoviDetector promotion")


### [ 2 ] Video clip to describle high level system design
[![IRS PM 2021 05 01 IS03PT GRP 3Musketeers CoviDetector system design](https://i.ytimg.com/vi/0HFkz8CoqLs/hqdefault.jpg)](https://youtu.be/0HFkz8CoqLs "IRS PM 2021 05 01 IS03PT GRP 3Musketeers CoviDetector promotion")

---

## SECTION 5 : USER GUIDE

`Refer to appendix <Installation & User Guide> in project report at Github Folder: ProjectReport`

### To run the system using iss-vm

> download pre-built virtual machine from http://bit.ly/iss-vm

> start iss-vm

> open terminal in iss-vm

```bash
(base) $ git clone https://github.com/xiaohuihong/IRS-PM-2021-01-16-IS03PT-GRP-3Musketeers-CoviDetector.git
(base) $ conda create --name py36 python=3.6
(base) $ conda activate py36
(py36) $ cd IRS-PM-2021-05-01-IS03PT-GRP-3Musketeers-CoviDetector/SystemCode/CoviDetector
(py36) $ pip install -r requirements.txt
(py36) $ python -m spacy download en
```

> Run migrations:

```bash
(py36) $ python manage.py makemigrations
(py36) $ python manage.py migrate
```

> You should now be able to run the project with Django's built-in
`runserver` command on port 8000 (or any available port).

```bash
(py36) $ python manage.py runserver 8000
```

>You should then be able to use the app in your browser at
`localhost:8000`.  Fill in form fields with test data and click button until the form is completed.


---
## SECTION 6 : PROJECT REPORT / PAPER

`Refer to project report at Github Folder: ProjectReport`

**Sections for Project Report / Paper:**
- Abstract
- Business Case
- System Model
- System Development & Implementation
- Challenge and Conclusion
- Appendix of report: Project Proposal
- Appendix of report: Mapped System Functionalities against knowledge, techniques and skills of modular courses: MR, RS, CGS
- Appendix of report: Installation and User Guide
- Appendix of report: Individual project report per project member

---
## SECTION 7 : MISCELLANEOUS

`Refer to Github Folder: Miscellaneous`

### corona_tested_20201115.csv
* Dataset of Covid-19 symptons and basic user info
* Insights derived, which were subsequently used in our system

### COVID_FAQ.xlsx
* FAQ list scraped from websites
* Insights derived, which were subsequently used in our system

### COVID_KNOWLEDGE.txt
* news or articles about Covid-19 scraped from websites
* Insights derived, which were subsequently used in our system
---


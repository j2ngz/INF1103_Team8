Project Initial Details (Team 8)

1. Problem Statement and Target Users 
What real-world problem does your application aim to solve?
Problem Statement: Job recruiters have to manually review large volumes of resumes, which is very time-consuming and sometimes inconsistent. Qualified candidates can sometimes be overlooked, and the evaluation criteria can vary between reviewers.

Our application aims to solve this by automating the first-pass screening step. From reading the candidate’s resume alongside a job’s requirements, it uses AI to extract and evaluate the candidate’s qualifications against a reference benchmark, then flags it out.

o Who are the intended users of the application?
Target Users: Companies and hiring managers/recruiters looking to screen job applicants 

2. User Inputs
What information or data will users provide to the system?
The user provides input only through a simple command line, selecting one of the following options in Menu/Command Line
—e.g.
Scan resume—reads all resumes from the resume folder and the requirements “.txt” file, passes it on to the AI manager
Exit—Exits the Program
View Summary, which generates a list of resumes that are scanned

Total Resume Scan: 10 
Score: /10
Outcome
Timestamp
Resume 1
8.4
Accepted
2026-09-10 14:02
Resume 2
2.1
Rejected
2026-09-10 14:05

Table 1—View Summary




3. Use of AI
How will AI be utilized within the application? 
After receiving the job title & requirements, AI will scrape the internet for the top resumes matching the request and extract the skills to be used by the logic manager as a benchmark against the company resumes.

What outputs, insights, or recommendations will the AI generate from the
user inputs? 
The AI will extract the top skills from the best resumes found online based on the user inputs, which mark out the criteria based on job title, experience, and description. It will also score the uploaded resumes based on how it compares to the best resumes found.
4. Business Rules 
What business rules, validations, or decision-making logic will be applied to the AI-generated outputs?
The “Logic Manager” applies threshold-based rules to the “AI Manager." Output (e.g., fit score to job, skill-match data) to determine an outcome for each resume:
Accept— (e.g. > 8 And all required skills are present)
Reject— (e.g. ≤ 4 or all required skills are not there)
Flag for review— (e.g. 5-7), the recruiter should manually check, as some required skills are there

After evaluating each processed resume’s score, skills, outcome, and timestamp are then saved in the database, so results can be reviewed later.


5. Misc
Github link: https://github.com/j2ngz/INF1103_Team8.git

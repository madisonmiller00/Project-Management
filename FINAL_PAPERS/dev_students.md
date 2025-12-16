Devon Reynolds 
IS 340 
Fall 2025


Student Retention Performance Tool
Abstract
This project paper proposes a hypothetical data science project designed to explore patterns in student retention and academic performance using project management elements such as a low-friction technical stack. Rather than prioritizing production-level deployment or predictive optimization, the project emphasizes interpretability, transparency, and sustainable project management practices. Using widely adopted tools such as GitHub, Python, and Jupyter notebooks, the project demonstrates how intentional technical debt can be incurred and managed across at least half the semester workflow. The project is situated within integrative project management and data science concepts, including workflow mapping, issue scoping, technical debt management, community feedback, and retrospectives.
Introduction
Throughout my time as a student, especially as a college student, we have recognized that it is extremely challenging to push oneself and complete college. There are years and generations of data showing that a chunk of students who go to college don’t even finish, or they flunk out. My personal evidence of this is within my male side of the family and peers around my age. With me on the verge of graduation, it makes me want to dive into the true disparity of weather students and their success in college as a potential project. 
The upper class of higher education collects decades' worth of data on its students. This includes student enrollment, performance, and progression. Progression can be defined by their grade point average (GPA) or individual letter grades. Although this data is frequently underutilized in ways that directly support academic advising and early intervention, it is frequently used to evaluate institutional effectiveness or compliance metrics. The fact that analytical tools are frequently unclear, inadequately documented, or constructed without considering the non-technical stakeholders who must interpret their results is one factor contributing to this gap.
Education analytics has a lot of research to back it up, and researchers do suggest that early in a student’s academic career, there are indicators such as first semester GPA, credit accumulation, and even if they dropped any courses, that are strongly associated with their long term retention outcomes. But, making these signals accurate and transforming them into insights does require a strong statistical background and analysis, but also good data quality, assumptions, and limitations. The project is motivated by what tools we need to understand the future model and not just making them automated. 

Target Audience
 
Figure 1
<img width="679" height="574" alt="image" src="https://github.com/user-attachments/assets/7ce563d4-a3cf-47d9-b130-b24e7a77c11a" />

 
Figure 2
<img width="625" height="600" alt="image" src="https://github.com/user-attachments/assets/d25edbd2-0adc-4b7b-ac93-18b07189acae" />


Both Figure 1 and Figure 2 show a national illustration of first-year college retention versus persistence. Retention reflects students who return to the same institution, while persistence includes students who remain enrolled in higher education at any institution. The gap between these measures highlights the complexity of defining student “dropout” outcomes. All data is from the National Student Clearinghouse Research Center. 

Academic advisors, institutional researchers, and administrators in higher education who oversee tracking student progress and creating retention plans make up the main target audience for the Student Retention & Performance Exploration Tool. There are quantifiable differences between students who stay enrolled at the same institution and those who continue their education elsewhere, according to national research that consistently demonstrates that student retention is still a difficult and ongoing problem for institutions (National Student Clearinghouse Research Center). These trends imply that retention is a complex process impacted by student engagement, institutional context, and academic performance rather than a binary result. Academic research also shows a strong correlation between persistence and graduation outcomes and student performance indicators like course outcomes, GPA trends, and instructional conditions (Heath, Darr, and Acharya). When combined with coordinated academic support and advising structures, comprehensive, data-driven interventions at the institutional level have been demonstrated to increase retention and graduation rates (Evans et al). However, a lot of current analytical tools put predictive automation ahead of interpretability, which limits their applicability to advisors who need to contextualize data in the context of specific student situations. This project is intended to assist stakeholders who need interpretable insights rather than opaque predictions by emphasizing exploratory analysis, transparent workflows, and documented assumptions. This aligns analytical outputs with the real-world requirements of advising and institutional decision-making.


Project Overview
The objective of the student retention & Performance tool is to promote comprehension rather than forecasting. Meaning that the project is intended for a “fictitious” audience of institutional researchers and academic advisors who need understandable analyses to support policy discussions and advising discussions. The project generates documented analytical artifacts that explain how conclusions are reached rather than providing a single metric or automated recommendation. 
Key objectives of the project include:
1.	Developing a reproducible exploratory data analysis of student performance and retention data.
2.	Emphasizing transparency in data cleaning, feature selection, and modeling decisions.
3.	Managing technical debt intentionally through careful scoping and staged refinement.
4.	Demonstrating effective project management through workflows, issue tracking, and retrospectives.

Potential Dataset
One of the most important aspects of this project is the data being used. For this project, we assume that the project is predicated on having access to an anonymous student dataset that includes enrollment and academic records for several terms. Variables like term GPA, attempted and earned credits, enrollment status, course outcomes, and a binary retention indicator would all be included in a realistic dataset. To lower the risk to privacy, demographic characteristics may be included in an aggregated or categorical form. Later in the model, it is highlighted that using a “group by” function in Python will also help clean this data. The dataset is purposefully flawed. Noisy indicators, inconsistent coding, and missing values are not viewed as preprocessing annoyances but rather as fundamental analytical challenges. This decision highlights the significance of recording data limitations and reflects actual institutional. Dataset sourced from either a government site or Kaggle, but preferred more realism throughout the analysis. 

Technical debt & Trade off
The project is anticipated to be 18–30 hours of initial technical debt over the course of the semester, despite careful tool selection. This debt results from deliberate trade-offs made in the early phases of the project, such as minimal continuous integration configuration, lightweight repository scaffolding, little automated testing, and succinct onboarding documentation.

The project presents technical debt as a managed constraint rather than an oversight. The project restricts the accumulation of high-interest debt by selecting established, well-documented tools and clearly defining project goals. This debt is partially paid off while maintaining project momentum by allocating time later in the workflow for testing, documentation, and refactoring. To be fair, also since this isn’t a foundation-type project where money is involved directly. 



Workflow & Timelines
The Student Retention & Performance Tool follows an eight-week workflow designed to balance and provide potential data for documenting and communicating feedback. 

<img width="975" height="613" alt="image" src="https://github.com/user-attachments/assets/78ab4a2b-06b1-493e-a1a5-d04aadcd1244" />

 
Week 1 – Project Scoping:
 Basic setup tasks are the first part of the project. The dataset schema, which includes variable names, data types, and anticipated formats, is defined this week. Concurrently, the GitHub repository is set up with a simple yet useful structure. Potential contributors are notified of the project kickoff after an initial README outlining the project's objectives, scope, and setup guidelines is written.

These early choices purposefully prioritize accessibility and speed over thoroughness. Although minimal automation and lightweight repository scaffolding lower onboarding friction, they also introduce known technical debt that must be resolved later in the workflow.

Week 2-3 Data Preparation & Feedback:
In Weeks 2 & 3, attention focused on data cleaning and validation. This is essential for a proper and more accurate model. The data team can address the missing values within the dataset, any inconsistencies, such as encoding or quality issues, to produce a dataset that is suitable for exploration analysis. While at the same time, receiving early feedback and having meeting discussion any time-intensive modeling, and when it would begin. Also, during this time, the idea is to have a clear and cut direction. Because cleaning decisions and assumptions are recorded as they are made, downstream tasks can move forward with a common understanding of data limitations. Before more time-consuming modeling work starts, early feedback lowers the chance of misalignment.

Week 4 – Exploratory Data Analysis (EDA) & Data Modeling:
The shift from preparation to analysis occurs in week four. Scripts for baseline exploratory data analysis are developed to visualize relationships, summarize distributions, and find possible predictors of student retention. To create a baseline understanding of performance patterns, a straightforward, comprehensible model is trained and assessed. To keep people informed about developments and discoveries, development updates are published. The project avoids premature optimization while producing insights that guide further refinement by giving interpretability and documentation top priority during this phase.

Week 5-6 Methods Refinement & Documentation:
The project concentrates on consolidation and clarification during Weeks 5 and 6. Data transformations, modeling decisions, and evaluation criteria are described in the methods documentation. Libraries/ programs would be used, such as Python, seaborn, and even NumPy, for any calculations. To enhance code quality and lower cumulative technical debt, unit tests and linting are expanded. This stage specifically allots time for debt repayment that was introduced earlier in the project. Improvements are made while the analytical context is still new, promoting reproducibility and ongoing maintainability, as opposed to retrofitting quality controls at the end.

Week 7 – Finalization and Documentation Sprint:
The project is getting closer to completion in Week 7. A docathon within GitHub is held to refine the README, methods section, and workflow explanations, and a final dataset snapshot is created to guarantee reproducibility. This focused documentation effort guarantees that analytical results are accompanied by a clear narrative context. The workflow supports the notion that communication and clarity are essential elements of project completion, rather than ancillary tasks, by allocating an entire phase to documentation and synthesis.

Week 8 – Feedback and Retrospective:
The potential last week of the project for any reflection, learning, and more feedback from stakeholders and any contributors, that are collected and reviewed. Also, a retrospective is made to represent what worked well, what didn’t work at all or caused trouble, what challenges happened throughout the week prior, and how this workflow can be improved in the future. This phase has different ways of being completed and can be viewed as a chance for institutional learning. Also, lessons and everything are all documented. 

Implementation Strategies
The first implementation pathway is supported by the project's design. An internal research prototype created by a small analytics team within an organization is one method. In this situation, the project continues to be an exploration and encourages policy debates rather than operational choices. The second project is positioned as an educational resource in a second implementation strategy. Students can experience the entire lifecycle of a realistic data project by using the workflow and technical stack as a teaching template in information science or data science courses. Lastly, the third tactic is incremental adoption, in which project results influence advisory procedures without being integrated into automated systems. This strategy is consistent with the course discussions about respecting organizational constraints and avoiding premature optimization.

Conclusion 
The Student Retention & Performance Exploration Tool demonstrates how structured project management practices, combined with a low-friction technical stack, can support meaningful and interpretable educational analytics. By emphasizing documentation, transparency, and intentional technical trade-offs, the project reframes success as clarity and sustainability rather than automation or predictive performance. Through its eight-week workflow, the project integrates data preparation, analysis, documentation, and reflection into a cohesive process that mirrors real institutional constraints. The intentional management of technical debt, paired with continuous feedback and retrospectives, highlights the importance of workflow-centered thinking in data-driven projects. This project illustrates that responsible data science in higher education depends as much on thoughtful project management and communication as it does on technical capability.

References
National Student Research Center: https://nscresearchcenter.org/persistence-retention/?utm_source
“Student Academic Performance, Retention, and Graduation: An Empirical Study.” Journal of College Student Retention: Research, Theory & Practice, 2022,
files.eric.ed.gov/fulltext/EJ1376716.pdf.
“Enhancing College Student Retention and Graduation Rates: Key Findings from a Five-Year Comprehensive Approach.” Cogent Education, vol. 12, no. 1, 2025, Article 2592388, https://www.tandfonline.com/doi/figure/10.1080/2331186X.2025.2592388?scroll=top&needAccess=true

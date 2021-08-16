After a short summer, I completed the study of software engineering and completed a project pair programming. After the course, I had some answers to my doubts before the course.

## Answers to doubts

After a short summer semester, I learned about software engineering development from many aspects of theory and practice. I began to have my own answers to some of the questions raised at the beginning of the semester. Here are my thoughts on these issues.

-  **The time cost of the personal development process itself? What are the boundaries of each stage?** 

This question is important for quantifying the software development process. But in my previous development experience, it's difficult to accurately time each phase of development -- a lot of the time in development is design, development, testing, and so on. This makes simultaneous timing cumbersome.

In pair programming, I specifically quantified the individual development process. According to the requirements of the course, it is necessary to estimate the time cost of each phase of the PSP at the beginning of development, and then work on each phase as planned. ** During development, due to the limitations of the PSP time schedule, I was able to control the time of each phase of pair programming with a certain purpose **. Try to complete the work within the estimated time. If the actual time used is different, it can be better analyzed afterwards.

Back to the question, how can we better define the boundaries of the phases and better quantify the time cost of development? Most of the time when I do pair development, it's driven by the plan I made at the beginning. That is, a specific period of time to complete a phase of work. If development stays on schedule (best case), then the schedule is the time cost of the final personal development. Of course, in the process of pair programming, my teammates and I also encountered many unexpected problems, and we did not complete the work in all stages according to the planned time. Such as spending less time on design than planned and slightly more time on development and testing. At this point, you only need to make fine tuning based on the planned time overhead.
In general, quantifying the time cost of the personal development process allows me to have more control over the overall progress and time during the development process, and also to reflect on my own problems at each stage according to the resulting deviations.

-  **timing of optimization and generalization.** 

When to optimize code? When to abstract generalized code? I still don't have a precise answer to these two questions, or it depends on the situation.
When I do pair programming, there is little generalization, more optimization. This is mainly because pair programming programs do not have to deal with many requirements changes; all requirements are set from the start. On top of this, the program for the running efficiency of high requirements, need to pay attention to the optimization of the code at the beginning, otherwise it will affect the final optimization effect.

-  **The division of labor and rotation efficiency of pair programming.** 

For this problem, I encountered in the process of pair programming. Due to the schedule of two people and the characteristics of the development of subproblems, my teammates and I adopted the way of pair programming combined with independent development. In the summary of pair programming, I gave my own views on the division of labor and the efficiency of rotation.

When the workload of tasks is large and the development tasks of each module can be decomposed into subtasks with high degree of parallelism, it is obvious that the efficiency of "multi-threaded" development will be higher. Based on the previous one, pair programming is likely to have difficulty in advancing development progress in the face of heavy workload tasks. In the early stage of pair programming, the efficiency of two-person programming was considerable, and the basic functions were quickly completed. But the accompanying tasks of testing, optimization, GUI-drawing, and so on make it difficult to advance the schedule of pair programming, which is not rich in time. In the end, we developed some tasks by division of labor to relieve the pressure of pairing tasks.

Pair programming is an approach to multiplayer development. However, not all cases are suitable for pair programming, and you need to make trade-offs based on the actual situation. It is necessary to estimate the cost when choosing the development method and deciding the division of labor. When the expected efficiency is not satisfactory, consider incorporating other development methods, or change the development strategy directly.

Summary of software engineering development

In this section, I will summarize my experience from the software engineering development stage.

### Requirements analysis - Use the NABCD analysis framework

For the stage of demand analysis, the book "The Method of Construction" puts forward NABCD analysis framework, which conducts project demand analysis from five aspects: original demand, practice, benefits to users, competitors and promotion methods. After the team project was approved, the team conducted a survey according to NABCD's five directions for the project requirements. This requirement analysis method comprehensively measures the goals, potential and possible obstacles of the project, and makes the focus of the project development more clear. For example, after analyzing my team's project, I found that the biggest difficulty lies in promotion. So the team needs to put more experience into promotion and user community building.

### Design - Document well before you do anything

After completing the requirements analysis, the most important thing is to form a complete and workable document based on the requirements.
In the design phase, the requirements are abstracted, detailed functional documents are written, and so on. These documents act as team members' contracts to the project, providing leadership for the later stages. In addition, the writing of the document also needs to be relatively concise, in order to avoid the deviation of the text understanding. It is important for the team to discuss and document the work before it starts.

### Implementation - Always follow the design document

After completing the requirements analysis and design, each member of the team must proceed with their respective tasks. During the implementation phase, it is difficult for each member to discuss the boundaries of their respective tasks frequently. Instead, the design phase documents are used to ensure that each self-task is integrated as a whole. Therefore, during the implementation phase, it is important to develop strictly according to the contract in the document.

### Testing - Complete testing is key

During the testing phase, I was mainly responsible for unit testing the back-end code. The Way to Build refers to a test-driven development approach in which unit tests are designed before code is written in the implementation phase. I tried this approach in development. This ensures that the code is correct as it is written. In addition, as described in the Book "The Way to Build", I also did coverage testing and other tests during the testing phase. Complete testing is the foundation of producing high-quality software. For each module in a project, you often need more code to test it.

Maintenance -- Respond to user feedback in a timely manner

After the release of the available version of the software, the maintenance team within the team needs to get feedback from users in a timely manner, monitor changes in the actual requirements, and change the software response part timely. Immediately after the software was released and put to user testing, a lot of user feedback was received, covering everything from UI to functionality. After summarizing the feedback, team members made trade-offs and quickly updated the software.
Timely maintenance based on user feedback can make the software more closely related to the actual needs of users. In addition, testing software irregularly during the maintenance phase can uncover and fix hidden problems, increasing the life of the software.

## END（My contribution）



1. Functional analysis（Further refine and improve each functional module）
2. Test plan
3. Database design
4. Project code
5. Unit test: This project uses JUnit + Mockito to carry out unit tests on the control layer and business layer of each module function respectively
   Manual test: This project uses Restlet Client to perform manual test on each module function, file upload function and payment function

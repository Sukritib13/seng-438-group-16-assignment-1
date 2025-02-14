>   **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group: Group Number      |
|-----------------|
| Student 1 name: Sahib Singh Thethi |   
| Student 2 name: Sukriti Badhwar |   
| Student 3 name: Rohan Lange |   
| Student 4 name: Wade Banman |   


**Table of Contents**

(When you finish writing, update the following list using right click, then
“Update Field”)

[1 Introduction	1](#_Toc439194677)

[2 High-level description of the exploratory testing plan	1](#_Toc439194678)

[3 Comparison of exploratory and manual functional testing	1](#_Toc439194679)

[4 Notes and discussion of the peer reviews of defect reports	1](#_Toc439194680)

[5 How the pair testing was managed and team work/effort was
divided	1](#_Toc439194681)

[6 Difficulties encountered, challenges overcome, and lessons
learned	1](#_Toc439194682)

[7 Comments/feedback on the lab and lab document itself	1](#_Toc439194683)

# Introduction

We knew the fundamentals of exploratory and manual functional testing before starting this lab. We knew that exploratory testing entails evaluating a system without pre-written test cases, enabling testers to actively investigate and find flaws using their knowledge and instincts. Manual scripted testing, on the other hand, is a structured approach in which the testing procedure is guided by pre-established test cases. However, we had little practical experience using these strategies in a real-world setting, and the majority of our knowledge was theoretical. Through real-world application, this lab gave us the chance to expand our understanding.

# High-level description of the exploratory testing plan

For our exploratory testing, we aimed to cover a broad range of functionalities within the ATM system while also attempting edge cases that could reveal potential defects. Our plan included the following steps:

1. Identify Key Functions: Focus on core operations such as login, withdrawals, deposits, balance inquiries, and fund transfers.
2. Vary Input Scenarios: Use valid and invalid card numbers, incorrect PIN entries, and extreme values for deposits and withdrawals.
3. Error Handling Verification: Check how the system responds to invalid transactions, multiple failed login attempts, and system restarts.
4. Consistency Checks: Ensure the correct updating of balances after transactions and verify if the system maintains state correctly.
5. Usability Assessment: Identify any UI/UX issues that could hinder user interaction or cause confusion.

With this method, we were able to investigate the ATM system methodically while still allowing for intuitive testing in response to unanticipated system behavior.

# Comparison of exploratory and manual functional testing

Exploratory and manual testing offered a variety of tradeoffs, creating environments where a given method may be superior to another and allowing for a wide range of coverage when employing both methods ona single artifact. 

In this instance, our group began with exploratory testing. When executing exploratory tests you're effectively testing the artifact blind, with only a brief understanding of it's overall workings and no knowledge of how any given function should behave. As a result of this blindness, exploratory testing creates the opportunity for developers to receive feedback upon whether or not their artifact behaves as a user might expect it too as opposed to how they imagined it during the creation process. Exploratory testing also opens the door to the discovery of bugs that may not be technical bugs or that where not considered during the creation of the scripted test. An examplpe of this occuring would be pins of a length > 11 digits crashing the program or that leading zero's were removed from pins. Despite the benefits of exploratory testing it comes with it's share of downsides aswell. The primary drawback of Exploratory testing is it's time commitment. As the tester doesn't know much about the program and is left to explore freely, it can take a long time to identify defects, especially in artifacts that are well put together and only struggle with the occasional edge case. Additionally, as the direction of testing is left to the tester there is no guarantee that all of the functionalities the developer wants tested gets tested. Considering all of these points, Exploratory testing is a relatively time inefficient method of testing that excels in detecting defects that developers may not consider and providing the poinit of view of a user as opposed to a developer.

Contrary to exploratory testing, manual scripted testing follows a specific line of tests provided by an artifacts developers to ensure specific functionalities are behaving as expected. These tests are very efficient to perform as the tester can follow the steps provided to test the requested feauture without any time spent searching for defects or testing functionalities that the developer believes work as intended. However, the rigidness of the scripted tests opens the door to defects in a functionality being missed as the provided tests don't cover their scope. Overall Manual scripted testing is very efficient and effective when it comes to testing specific functionalities but can miss several defects that are not covered in their scope. 

Combining the two methods allows for testers to cover a large variety of cases within the artifact giving them the liberty to detect defects that may have been overlooked by developers as well as ensure that specific functionalities are working as intended resulting in a thoroughly tested artifact.

# Notes and discussion of the peer reviews of defect reports

After each pair finished their work, comparison was relatively easy. Each pair was able to find unique defects along with defects both pairs found. Reports were well documented having relevent sections for each bug such as Steps to reproduce, functions tested, initial state and outcomes. Consistent categorization of reports resulted in easy identification of testing types, minimizing duplicate reporting. This organized approach enhanced the effectiveness of the peer review process for defect reports within the group.

# How the pair testing was managed and team work/effort was divided 

We separated our efforts into two roles in order to manage pair testing efficiently: one person performed the tests as the tester, while the other person recorded results and examined flaws. Two pairs were formed from our four-person group, and each pair worked on separate test cases. After completeing individual testing, we combined our findings to provide an extensive defect report. Effective lab collaboration and comprehensive testing coverage were guaranteed by this division of work. Through this experience, we learned the importance of effective communication and coordination in team-based testing. 

# Difficulties encountered, challenges overcome, and lessons learned
Difficulties Encountered:
Our group faced several challenges while navigating JIRA, which we used as our bug tracking system. Initially, we struggled to realize that a separate bug tracking project needed to be created in JIRA. This led us to first export our bug tickets from the existing project into a dedicated bug tracking project. Additionally, we encountered difficulties in creating custom fields and exporting them as an Excel file. Another challenge involved collaborating on our pair testing manuals, where we faced issues with identifying and resolving duplicate entries.  

Lessons Learned:
We learned that effective communication is crucial for productivity. At first, we faced delays due to a lack of clarity about what tasks were completed. However, once we started communicating regularly, we were able to complete our work more efficiently. Additionally, dividing tasks among team members proved essential for maintaining steady progress without overburdening anyone. By ensuring that each member had a manageable workload, we were able to minimize stress and work more cohesively as a team.

# Comments/feedback on the lab and lab document itself
This lab was useful in understanding exploratory testing, manual scripted testing and regression testing. It also helped us understand the bug tracking system. But at the same time the lab session itself felt a bit disorganized. However, the lab session itself felt somewhat disorganized. At the start, we were uncertain about the tasks and felt quite lost. The lab documents appeared overwhelming initially, but as we progressed and sought clarification during the session, our objectives became clearer. Some instructions in the lab document were vague, which led to uncertainty about how to proceed with certain tasks. We resolved this within our group by collectively interpreting the assignment to the best of our understanding.Additionally, the requirements document could have provided clearer guidance on managing bug reports in the tracking system. For instance, in regression testing, it was unclear whether we needed to create duplicate tickets or simply update the existing ones in JIRA. Overall this lab was helpful in practicing git, bug tracking tools, testing procedures, and building overall teamwork.

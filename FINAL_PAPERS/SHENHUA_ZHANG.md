## Building Life-Essential APP for UIUC students’ life
By Shenhua Zhang, Fall 2025, https://github.com/Susan000000

### Introduction

#### Background Information
As a student from University of Illinois, Urbana-Champaign, Illinois is widely known as one of the most popular apps that is used by students. Generally, the software includes many important features. For example, e-wallet, course list, dining check, groups, events, and so on. The Illinois app, developed by the ROKMETRO company, is based on the open-source platform named Rokwire that aims to create “a digital ecosystem that will stimulate innovation in smart technology to make society safer, foster better decision-making, and increase wellness” (Rokwire, n.d.). According to Salas and Chatterjee (2023), one of the principles in designing the app is to make minimal changes to the original software for the best adaptability. The app was originally created during the COVID-19 period, which was originally designed to respond with the hardship of the transition period from working in person to online. As an open source app, it not only involves designs from the ROKMETRO company, but also allows students and faculties at UIUC to modify. When new features are proposed, the company will check if there are any significant bugs and test the functionality, and then the updates will be made in the app in the end. 

#### Motivation
During my undergraduate life, I gradually noticed the frequency of using the app among the students is low. Let’s take the “My Course” section as an example - even though there is detailed information about the courses including instructor name, classroom location, time schedule and so on, most students are used to checking the course information in other schedule-planning apps (such as Calendar); there is no advantage on Illinois app for people to make notes, create schedule, etc. In this project, I am mainly focusing on the improvements of both “Groups” and “Events” sections for the best user experience. Looking for communal groups and friend circles is important for students’ social life after class; however, it is usually difficult for students to look for groups they are interested in to participate. The mainstream of getting into the RSOs (Registered Student Organization) is to attend the Quad Day when all RSOs have the opportunity to advertise for themselves, or to get introduced by a friend who has already taken part in the club. Even though the club is usually posted on social media, it will be hard for new members to find the information. If looking for a specific group of RSOs to join (such as the art clubs), it can take a lot of effort to filter them out from the list of more than 800 RSOs on the official website. Furthermore, the “Groups” and “Events” also have some significant weaknesses that prevent users from maximizing its best use (e.g. inefficient filters, out-of-date information, …) . 

Given the chance that the Illinois app is built on an open-source platform and the gap of demand, I decided to innovate the design of “Groups” and “Events”. In the project, I will break the project plan into several parts: preparation, identifying the weaknesses, designing groups and events functionality, and evaluation. 

### Preparation
To gain the best overall understanding of design, the preparation stage is crucial and inevitable for the program developers. We will have two parts of the preparation stage, including making questionnaires for the current users and exploring the functionality for the current Illinois app. 

#### User Questionnaire
To understand the gap between users and the app design, developers need to collect and analyze the demand from users’ experience. Thus, creating a questionnaire is necessary. Developers are able to design the questions on their own to best reflect the knowledge. In the survey, users will be asked questions from the following aspects: 

1. What is your frequency of using the app / each section?
2. What is your satisfaction level of the app / each section?
3. Why do you think this app / section is satisfied / not satisfied?
4. What do you think is the biggest advantage / disadvantage of each section?
5. How would you suggest improving the functionality? 
After creating the questionnaire, it is important to make sure the questionnaire is spread among users. One good way to ask users to fill in the questionnaire is to send reminders to them via app notifications. Besides, the development team can also ask the university to send emails (which is more commonly accessed) to all students and faculty. Potentially, adding incentives such as random reward will also motivate users to fill out the form. 

#### Explore current functionalities of Illinois app
Except for the answers from users, developers can also explore the app directly by installing the Illinois app and trying all functions out. The home page displays the user-customized combination of favorite functionalities, and there is a list of all sections next to it (Figure 2.1) For users who are interested in groups and events, they need to scroll down to click on them. Inside the functions, events and groups are displayed in a dropdown menu format. By default, all events are sorted by time. If looking for anything specific, users can tap on the filter or search for the keywords (Figure 2.2). 

Other features that are parallel to the home page are map, wallet, and assistant (AI), which are not the main theme of our project. 

<img width="236" height="512" alt="2 1" src="https://github.com/user-attachments/assets/b4a38fa4-2370-48ac-84f8-7e8919b9c109" />  <img width="236" height="512" alt="2 2" src="https://github.com/user-attachments/assets/e656ff04-0a13-43c4-9392-5b91c5338e6a" />

_Figure 2.1, Home page of Illinois APP; Figure 2.2, Events section of Illinois APP._

### Identifying the weaknesses
In this stage, we will summarize the collected data from the preparation stage. Main problems will be discussed below to help the development team to design the interface better. 

#### Limited Information
As we dive into the functionality, we discovered that the information is not complete and up-to-date. In Figure 3.1, even though we are checking for “All Groups” as shown on the top of the screen, there are only 40 groups campus-wide. This is considered as extremely low frequency of use, especially given the statement from the official website of ISSS, “at the University of Illinois Urbana-Champaign, there are more than 800 registered student organizations (RSOs) and many international RSOs are active on campus” (International Student and Scholar Services, n.d.). What’s more, as shown in the Figure 3.2, a large number of labels in the events section are not fully utilized. For instance, under the “College, School & Unit” category, most of the subcategories are not labeled with any events at all. This can be caused by the ignorance of adding essential labels when creating the events, or these labels are not necessary to add into the events. Thus, the developers should aim to optimize the data collection and labeling to better extract the useful information for users to view. 

<img width="236" height="512" alt="3 2" src="https://github.com/user-attachments/assets/fb5724a8-fb50-4e5e-9c12-5ba03b6bc542" />  <img width="236" height="512" alt="3 2" src="https://github.com/user-attachments/assets/b92452af-fa59-4ae2-88e4-14c90774352d" />

_Figure 3.1, All Groups Page in Illinois APP; Figure 3.2, Event Filter of College, School & Unit in Illinois APP._

#### Poorly-Designed Interface
Another significant issue for the Illinois app is the inefficient design of the interface. One of the most important components of the app is the UI-design, which is originally constructed for the purpose of interacting between users and the software functionality. Due to the lack of consideration on design, it could possibly lead to the failure or inefficiency of achieving users’ goals of using the app. In Figure 3.3, the overall event categories are shown. Across all the labels, it is clear to see that some of the labels have several hundred events, while some have no event at all. This may bring inefficiency to use the filters when users are looking for a specific group of events - using Google instead will be much more efficient if most events are not shown in the app. In Figure 3.4, we simulate users who are searching for art events, so we put “art” in the searching box. However, the returning results are confusing. It is not just art-related events that are not shown, but also giving the users a list of irrelevant events. The first result, “AE Commencement Celebration 2026”, is for the celebration ceremony of the Aerospace subject; the second result focuses on Artificial Intelligence. Both of these returning results do not match with the desired results of art-oriented events, which means the quality of the search engine is quite low. Ideally, programmers are supposed to get rid of the unnecessary modules in the interface design and make breakthroughs in the UI-design to increase the usability of the app while maintaining the original purposes to use. 

<img width="236" height="512" alt="3 3" src="https://github.com/user-attachments/assets/49f6b864-bd44-495f-9700-34baac55c5a5" />  <img width="236" height="512" alt="3 3" src="https://github.com/user-attachments/assets/76d1a797-bce4-40fa-8986-8139b5a59120"  />

_Figure 3.3, Event Category of Events in Illinois APP; Figure 3.4, Search Engine of Events in Illinois APP._

### Rebuild the Groups & Events Functionality
In the fourth section, we will discuss how to rebuild the Groups & Events functionality in detail. To break down this section, we need to implement the reconstruction in 3 important steps: reconstructing the data collection, redesigning the interface, and finalizing the design by adding connections. 

#### Construct the Data Collection Phase
To rebuild the whole functionality of Groups & Events, we are required to redesign the way of data collection from the beginning. First, we need to reconstruct the database structure to overturn the original way of storing data (which can be inefficient if we keep the structure for new design). The development team can draw a sample ER diagram (Figure 4.1) to brainstorm the required attributes for the data collection stage. By connecting the entities together and modifying the attributes, programmers will have a general idea of which information is important to the later development stage. In this step, it also contributes to getting rid of redundant attributes as much as possible.

<img src="https://github.com/user-attachments/assets/dfeb223a-890e-4f08-bfff-039c49a96f3c" width="350">

_Figure 4.1, Sample ER Diagram of new Groups & Events database._

Getting beyond the database, it is also important to determine the data source to ensure the diversity of data. We encourage mainly 2 ways of uploading the groups and events data:
1. Posting the events ***manually*** with registered account (as a group) from the Illinois app; 
2. ***Automatically*** synchronizing the data from the trusted websites. 
For the first way, it is important to strictly ask every group to register one account and verify the identity to avoid missing groups / unverified wrong accounts to be registered. For the second way, programmers need to spend more effort to ask the official website from the university to create an automatic system of synchronizing the events posted on websites and on the Illinois app. With careful check on data input, we are able to guarantee the data quality while increasing the size of data to a great extent. 

#### Redesign the interface
As mentioned before, one of the most serious problems of the app is the interface design. Therefore, we will go through the following sample interface designs gradually and envision the possibilities of future breakthroughs to enhance the performance of groups and events functionality. 

In the original app design, only users within the same group are able to share posts with each other. For the new design, the posts will be posted in public for better spread. On the main page, we will create a “Trending” list of events that are happening on campus (Figure 4.2). The main page is similar to the summary of interesting events campus-wide, with one cover image, post date, brief title and concise labels to catch users’ eyes at once by images and keywords in text. There are mainly three segments of the Trending page: 
1. (Recommended) for you
_ Based on the big data and recent activities, events of your possible best interests will be generated in this segment. 
2. Editor pinned
_ Events promoted by the university, such as important academic seminars and professional career fairs for student development opportunities. 
3. Popular on campus
_ The most popular event with the highest attention by a lot of students and faculty. Usually determined by the number of views, likes, and comments of the post. 

In the new design, each event is formatted into posts.For instance, the UI-Con event is posted with pictures and descriptions (Figure 4.3). In the new Event page, we are able to see the original posted account (group / organization), the event pictures, detailed post time, text introductions and labels of the events. To further encourage the communications among users, we also implement the social interaction functions (likes, comments, collections). At the bottom of the page, comments of different users can be viewed. In this way, we aim to build a community at U of I to improve the effectiveness of exchanging ideas with the official and trustworthy app, Illinois. 

<img src="https://github.com/user-attachments/assets/dc3c1bf2-caf1-4f35-8680-c03077548177" width="350">  <img src="https://github.com/user-attachments/assets/51f2fcf1-c402-4bf3-8cba-10f9f6433282" width="350">

_Figure 4.2, Sample interface design of Trending as the main page; Figure 4.3, Sample interface design of Event as the post._

For each group, the interface design is changed to fit with the users’ preferences. For example, there will be the self-introduction for the club, registration date, and related ongoing and past events for people who are interested in exploring them to find out. Clicking on the event pictures or descriptions will lead the user to the event posting page. This will be a good joint to merge all desired information in the group page. If possible, the group leader can also add external links, such as discord links to welcome new members to join the group and chat with each other. 

In the Figure 4.5, we have the innovative design of the search engine to replace the old one. Rather than using the traditional text search engine, we choose to design a new search engine with the help of AI. Namely “Illinois Smart AI”, the goal of creating the AI is to assist with the users’ experience. In the Groups & Events sections, they are expected to return the best results based on the users’ demand (which corresponds to the original filter function). Users will type in their requests in plain English text, such as “tell me some art-related events next week”. Then, the AI will receive the message and break down the meaning with the help of Natural Language Processing, and extract the keywords from the sentences. The next step is to align the keywords with the posts. As mentioned before, we include all detailed descriptions, event label, time and location in each post. Thus, with careful processing of the text, it will be easy for the AI to extract the necessary information and provide the best answers for the users. Results will be turned back with AI’s text message and links to the events and groups. Since more efforts are made behind the screens, the page will have a neat design but reaching the goal effectively. 

<img src="https://github.com/user-attachments/assets/f6aa8748-da14-429e-8186-fc9a2dfec72e" width="350">  <img src="https://github.com/user-attachments/assets/90119393-465f-4ea2-9c9f-015b4ab31779" width="350">

_Figure 4.4, New groups design page; Figure 4.5, New Smart Search AI page._

#### Finalizing Our Design
To wrap up our project, we need to add communications between the interface and database to “speak” with each other to make sure the software is working properly in a circulation. Below in Figure 4.6 is a sample workflow diagram of frontend and backend in the software. By adding server and connections between the web app and database, the whole software is complete. Programmers should test whether this will work and debug if any errors occur. 

<img src="https://github.com/user-attachments/assets/e1c86b04-30bc-4620-bbf9-ffdc219d3fe5" width="350">

_Figure 4.6, Workflow Diagram of Frontend and Backend (Javinpaul, 2024)._


### Evaluation
At the final stage of the process, the development team needs to evaluate the whole project as a whole. If they ensure the following steps are made and repeated in the future for maintenance and updates, then the project reaches its goal of improving the functionality of groups and events in the Illinois app:
1. Run the program and check if there is any error
2. Make sure the designed fits with the original purpose
3. Test the new functions with users and ask for feedback
4. Evaluate the convenience and quality of the app
5. Update the app if necessary

### References
* Javinpaul. “Top 10 Free Frontend and Backend Development Courses in 2024.” Medium, 14 May 2024, medium.com/javarevisited/top-10-free-frontend-and-backend-development-courses-in-2024-ad9f681a95fe.
* “Registered Student Organizations.” International Student and Scholar Services, isss.illinois.edu/training-programs/rso/. Accessed 11 Dec. 2025.
* Rokwire, rokwire.illinois.edu/. Accessed 10 Dec. 2025.
* Salas, Lillien, and Rohit Chatterjee. “Rokwire: The Open-Source Platform behind the Illinois App and More.” The Daily Illini, 4 Dec. 2023, dailyillini.com/special-sections/technograph/2023/11/29/rokwire-illinois-app/.

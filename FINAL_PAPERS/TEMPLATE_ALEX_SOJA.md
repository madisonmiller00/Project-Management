# Spotify Listening Dashboard
Alexander Soja, Fall 2025, https://github.com/alexsoja/SpotifyDashboardProject

# Abstract
This paper explores the possible routes for implementing a Spotify Listening Dashboard, a project designed to help users better understand their personal music habits through interactive data visualization. The dashboard aims to provide listeners with clear insights into their top artists, albums, genres, and long term trends by using tools such as Spotipy, Python, Pandas, and Streamlit. Drawing on project management principles from Professor Alicea’s 2025 slides, the paper outlines a structured development process that includes defining user needs, designing workflows, building interactive features, gathering community feedback, and iteratively refining the platform. The project is grounded in research that connects music preference with personality traits, demonstrating the psychological value of allowing users to explore their listening data in meaningful ways. Together, these elements illustrate how a thoughtful technical design combined with community focused governance can transform a personal idea into a scalable and educational data driven tool.

# Introduction
## Background
Music serves as a central part of identity formation, emotional regulation, and daily life for many people. Streaming platforms such as Spotify have further transformed the way people engage with music by collecting detailed listening histories and generating personalized recommendations. However, users rarely have access to transparent interpretations of their own music data. Although platforms release annual summaries such as Spotify Wrapped, there is a clear gap for tools that help listeners explore their tastes throughout the year in a detailed and interactive manner.

Research also shows that music preference reflects stable and meaningful psychological patterns. Rawlings and Ciancarelli found that the personality traits openness and extraversion strongly predict preferences for specific genres such as classical, rock, electronic, and popular music. Their findings demonstrate that listening behavior is connected to deeper aspects of personality, motivation, and emotional style. This relationship strengthens the purpose of a tool that visualizes music data because it allows users to gain insight into themselves through their listening patterns. Music becomes a window into identity, and data becomes a method of understanding that window.

As noted in Professor Alicea’s slides, the first step in project development is identifying the community and the motivation behind the work. This project is grounded in a desire to empower everyday listeners to understand the patterns that shape their musical lives.
In addition to individual identity formation, music also plays a broad cultural role. Listeners often use music to signal social belonging, form friendships, and navigate transitions in their lives. During adolescence and early adulthood especially, musical identity becomes part of how people articulate values, aesthetics, and emotional experiences. These cultural dimensions further support the importance of a tool that does more than display statistics. A dashboard capable of revealing how habits shift across semesters, seasons, or major life changes can help users see how their evolving tastes mirror their personal growth. Because streaming data is continuous and dynamic, it allows for a form of reflection that traditional music categorization never could.

## Project Vision and Community

The aim of the Spotify Listening Dashboard is to create an interactive and personalized tool that helps users explore their top artists, albums, songs, and long term trends. The dashboard functions as an ongoing music journal that displays how a listener’s tastes evolve across short term, medium term, and long term time spans. By providing transparency and visibility into one’s own data, the project enhances self reflection and strengthens musical engagement.
The dashboard also supports users who enjoy connecting their musical identity to psychological or emotional meaning. Since listening preferences are associated with cognitive and personality traits, users can interpret their own data in ways that deepen understanding of who they are and how they change over time.
Target Audience and Benefits

The project serves a broad community of Spotify listeners. Its primary audiences include the following.

- First, casual music listeners who enjoy visual summaries of their habits and want to understand how their preferences shift over time. For these users, the dashboard acts as a continuously updated version of Spotify Wrapped that they can check at any moment rather than once a year.
- Second, highly engaged music fans who take pride in analyzing their listening data. These users benefit from customizable filters, detailed breakdowns, and interactive charts that reveal nuanced patterns in listening behavior.
- Third, individuals interested in the connection between music and personality. Because research shows strong correlations between traits and genre preferences, the dashboard can provide insights that help users reflect on their personality, mood, and sense of identity.
- Fourth, educators or researchers in fields such as psychology, data science, and digital humanities may also benefit from the dashboard as a tool for demonstrating how personal data can be translated into meaningful visualizations.
  
Beyond these core user groups, the dashboard also appeals to individuals interested in digital self tracking. As personal analytics tools become increasingly common in wellness, productivity, and fitness, there is growing interest in understanding behavioral data across domains. Music is an accessible and emotionally resonant entry point into this trend. By positioning the dashboard within the broader self, this project can become part of a larger shift toward reflective technology that helps people make sense of their daily lives.

# Technology Involved in Dashboard Development
## Spotipy for Spotify Data Retrieval
Spotipy, a Python library for accessing the Spotify application programming interface, enables the dashboard to retrieve a user’s top artists, albums, tracks, and audio features. It supports secure authentication and provides structured data that can be transformed into interactive visualizations. The use of Spotipy allows the dashboard to operate without requiring users to manage complex technical steps.

Spotipy also makes the dashboard scalable. As Spotify updates its application programming interface or adds new analytics features such as mood scores or listening contexts, the dashboard can incorporate these fields with minimal restructuring. This adaptability is important because one of the long term goals of the project is to support more complex interpretations of listening behavior, such as correlations between audio features and time of day or comparisons between energy level and mood preferences. By beginning with a robust data collection foundation, the dashboard remains flexible enough to accommodate future research connections.
## Python, Pandas, and Altair for Data Processing and Visualization
Python serves as the primary language for collecting, cleaning, and organizing user listening data. Pandas supports data manipulation, comparison between time ranges, and the creation of structured data tables. Altair provides interactive and aesthetically pleasing visualizations such as bar charts, distribution graphs, and ranking comparisons. Together, these tools allow users to explore their listening habits in real time.

These tools also allow for reproducible workflows. Because the transformations from raw listening data to visual outputs can be scripted, tested, and version controlled, contributors can review, correct, or expand the logic behind how insights are generated. For educational contexts, this reproducibility provides an opportunity for students to learn data cleaning, feature engineering, and exploratory visualization in a real world application.

## Streamlit for Dashboard Interface
Streamlit is used to build the user interface of the dashboard. It creates a clean and responsive webpage where users can interact with their data without needing technical skills. Streamlit integrates seamlessly with Python code, making it possible to update graphs instantly when data changes. Streamlit also supports modular design, allowing expansion into multi page layouts such as artist overviews, genre summaries, personality interpretation pages, and more.

## GitHub for Version Control and Collaboration
GitHub functions as the collaborative space for maintaining and improving the dashboard. Version control ensures that the development process remains organized and that changes are well documented. GitHub Issues, Kanban boards, and branches facilitate planning, testing, and reviewing updates. As the project grows, contributors can suggest features or improvements through public discussion boards, reflecting the community governance principles described in Professor Alicea’s slides.

# Contributors
## Team Structure
While the current version of the dashboard is an individual project, its long term vision supports the involvement of multiple contributors. Future collaborators may include data science students, user experience designers, and psychology researchers interested in linking listening behavior to personality theory.

In a community driven model, contributors would collaborate through GitHub, sharing improvements, adding new visualizations, and refining data interpretation features.

We could also include artists, who want to showcase different images or videos if they appear on the top of a user’s page.

## Talent Recruitment
Establishing a community space, such as a Discord server or a Registered Student Organization at the University of Illinois, could help recruit contributors interested in data analytics and music technology. The dashboard project can attract students who want practical experience in building interactive applications and working with real world data.
## Impacts of Student Involvement
Students who participate in the project can practice skills in Python, visualization, application programming interface integration, user experience design, and project management. They gain experience working on an open source project and learn to document and present their work. This type of engagement reflects the principles of experiential learning and collaborative problem solving.

The project also aligns well with interdisciplinary collaboration. Music students may contribute insights about genre classification, listening psychology, or cultural theory. Business students may explore how music data relates to consumer behavior or brand interaction. Information science students may analyze user behavior patterns or interface usability. This collaborative potential highlights the dashboard not only as a technical artifact, but as a shared space for students across disciplines to study music as a social and analytical subject.

# Community Governance
## Controlled Vocabulary
To maintain consistency across contributors, the project would benefit from a controlled vocabulary that defines terms such as top artist, audio feature, popularity score, time range, and genre classification. A shared vocabulary ensures clarity in both documentation and communication across the project.

## Code of Conduct
A code of conduct would establish expectations for collaboration, communication, inclusivity, and professionalism. Contributors would commit to respectful dialogue, transparent decision making, and clear documentation practices. These principles support a healthy project community and encourage positive participation.

Governance structures are especially important for projects that may evolve into open source communities. Without clear norms, contributions can become inconsistent or fragmented. A shared code of conduct, documentation standards, and vocabulary guidelines ensure that new contributors can enter the project smoothly. These structures also reflect real world software development practices, where governance determines the long term sustainability of a tool or platform.

# Future Pathways and Extensions
Looking beyond the core implementation of the Spotify Listening Dashboard, there are several promising directions in which the project could evolve. These future pathways build on the foundation of personalized data visualization and extend the dashboard into a more social, interactive, and community driven experience. By expanding both functionality and user engagement, the dashboard can transition from a personal analytics tool into a platform that connects listeners with one another in meaningful ways.

One potential extension is the introduction of social features such as personalized leaderboards. These leaderboards could allow users to compare their listening habits with friends by ranking top artists, albums, or songs across a shared group. For example, users could see which friend listens to a particular artist the most or how their own listening frequency compares to that of others. This feature would bring a sense of friendly competition while strengthening music based social connections. It also mirrors the natural role that music already plays in relationship building, communication, and identity expression.

Another possible pathway involves integrating collaborative playlists or shared listening summaries. Users could generate group statistics that reflect collective preferences, discover artists that are popular within their friend group, or create playlists based on overlapping tastes. These features would support not only individual reflection but also community discovery, encouraging users to engage with music as a shared cultural experience.

Future iterations could also draw on psychological or behavioral models. Since research indicates that music preference aligns closely with personality traits, the dashboard could explore connections between user behavior and the broader insights found in studies like Rawlings and Ciancarelli. Such integrations could offer reflective features that help users understand how their preferences shift during different life phases or emotional contexts.

Finally, the dashboard could expand into a public facing platform through optional profile pages where users showcase their top artists, listening streaks, or long term trends. This would allow the project to grow beyond a private data tool into a community hub for music enthusiasts.

Together, these extensions illustrate the long term potential of the Spotify Listening Dashboard. While the initial version focuses on personal insights, future pathways can transform it into a collaborative and socially engaging ecosystem that deepens how listeners connect with music and with each other.

In the long term, the dashboard could even expand beyond strictly Spotify based data. As music platforms diversify and users interact with multiple ecosystems such as Apple Music, YouTube Music, and Bandcamp, a cross platform dashboard would allow for a more comprehensive understanding of listening behavior. Such an extension would require significant development but would position the project as a truly universal music analytics tool capable of capturing digital listening as a whole rather than within the boundaries of one company.

# Working Phases
The project can be built and refined through a cyclical five phase workflow.

### Project Workflow Diagram
<img width="589.61" height="300.00" alt="Screenshot 2025-12-08 at 6 26 41 PM" src="https://github.com/user-attachments/assets/ba8d2ee6-dcb3-44f4-888c-27c4a2a10b89" />

(Alicea, slide 6).


## Phase One: Initial Definition
This includes defining the purpose, outlining user needs, and collecting early feedback. Documentation such as the project vision, user stories, and feature outlines would be stored on GitHub.
## Phase Two: Design and Prototyping
Wireframes and data flow diagrams are created to map out user interactions. Mockups of dashboard pages would be developed in tools such as Figma or Streamlit’s preview mode.
## Phase Three: Development
This phase includes implementing the core functionality using Python, Spotipy, Pandas, and Altair, followed by building the interactive interface in Streamlit. Code is tested and reviewed on GitHub.
## Phase Four: User Feedback Analysis
Users test the dashboard and provide feedback. Feedback is stored in GitHub as issues or discussion posts. Patterns are analyzed to determine improvements.
## Phase Five: Iterative Refinement
Based on user feedback, features are adjusted, new visualizations are added, and bugs are fixed. The cycle then returns to Phase Two as the project grows.

These phases mirror real world software development life cycles used in industry, such as agile sprint cycles and iterative release models. By framing the dashboard’s development within this structure, the project serves as a practical example of how planning, testing, community feedback, and refinement guide the production of digital tools. Students who engage with any of the phases gain practical experience in managing complexity, prioritizing features, and communicating across technical and non technical roles.

# Documentation
GitHub hosts clear documentation that describes how to install the dashboard, how to authenticate with Spotify, how the code is structured, and how contributors can participate. It also includes a roadmap of planned features such as personality based insights, genre clustering, and cross year comparison tools.

High quality documentation ensures that the project remains accessible beyond its original creator. For long term sustainability, documentation acts as the memory of the project. It allows new contributors to understand the logic behind decisions, prevents repeated mistakes, and provides transparency about how user data is processed. Good documentation is also essential for ethical reasons, especially when working with sensitive personal data. Users deserve clarity about what information is collected, how it is stored, and how it is used within the dashboard.

# Licensing
The project can adopt a Creative Commons Non Commercial Share Alike license. This license allows others to learn from and build upon the project for educational purposes, while preventing commercial use without permission. It encourages collaboration while protecting the integrity of the project’s mission.

Choosing an appropriate license also signals the project’s commitment to open knowledge. By permitting adaptation while restricting commercial exploitation, the license encourages educational use and collaborative improvement. It also aligns with the ethos of community driven development described in the readings and lectures.

# Conclusion
The Spotify Listening Dashboard represents an intersection of personal data analysis, music psychology, and user centered design. By applying the project management principles presented in class, the project moves from an idea into a structured and scalable interactive tool. Research on personality and music preference provides a theoretical foundation that gives the dashboard deeper meaning beyond simple data visualization.

Through community involvement, open documentation, and iterative development, the dashboard can evolve into a valuable resource for listeners who want to understand their musical identity. It can also serve as a practical learning platform for students who wish to build real world data applications. This project demonstrates how technology can enrich everyday experiences by transforming personal data into insight.

Ultimately, the Spotify Listening Dashboard demonstrates how personal data, when handled responsibly and interpreted thoughtfully, can enrich self understanding and community interaction. In an era where data collection often feels opaque and one sided, this project returns control to the user by transforming raw information into meaningful insight. It shows that technology can deepen rather than diminish human connection, especially when built with intention, transparency, and collaboration.

# References

Alicea, Bradly. (2025). Integrative Project Management: Mid-term Check-in Slides. University of Illinois at Urbana-Champaign. https://canvas.illinois.edu/courses/58940

Rawlings, D., & Ciancarelli, V. (1997). Music preference and the Five-Factor Model of the NEO Personality Inventory. Psychology of Music, 25(2), 120–132. https://doi.org/10.1177/0305735697252003


Spotipy Documentation. (2024). https://spotipy.readthedocs.io


Streamlit Documentation. (2024). https://docs.streamlit.io


# Milestone 3

## A: User Experience Requirements

**Decomposed Milestone 2 Solution as User Stories**

### Physical limitations
* As an instructor teaching a class in a large lecture hall, I want the seating arrangement of my students to not impact their ability to follow my lecture, so they can focus on core concepts.
* As a student who is in a large lecture hall, I want to see the list of commands that my professor types on my own computer because the commands are too small on the projector screen. 
* As an instructor in an in-person class setting, I want to ensure that my students can clearly see the concept of the lesson, regardless of where they are seated.
* As an instructor teaching in a large lecture hall, I want students to be able to see everything I’m projecting to the screen regardless of seating, so they don’t need to ask me editor specific instructions.

### Textual Representation
* As an instructor teaching a programming class, I want to record the list of commands that I type so that students can review my commands after class whether it is to review commands or because they missed class. 
* As a student who is new to programming, I want to see the list of commands that my professor types into the text editor so that I can focus on the concepts being taught instead of memorizing keystrokes. 
* As a student who is new to programming, I want to see the list of commands that my professor types into the text editor so that I don’t fall behind if I miss a command. 

### Student Proficiency Level
* As an instructor teaching an intermediate class in a large lecture hall, I want to be able to display my commands to my students so that they can see what commands they need to use whether they are using the same text editor or a different one. 
* As an intermediate student who is not familiar with the text editor my professor is using, I want to see the list of commands my professor is typing and an explanation of the keystrokes so I can replicate the action on a text editor I am already familiar with.
* As a student who transferred in from another school that taught a different text editor, I want to be able to quickly assimilate into my new school’s instruction style. 
* As a student from a different degree path, I want to be able to understand the concept of the lesson without needing to implement it. 
* As a student new to a text editor, I want a quicker way to see what the shortcuts for a command are so I don’t need to look them up online or some other way.

### Falling Behind
* As a student who is new to programming, I want to see the list of commands that my professor types into the text editor so that I don’t fall behind if I miss a command. 
* As a student who had to miss a class, I want a list of the commands my professor typed so that I can follow along with what I missed from class.

**Most Relevant User Stories**

* As a student who is new to programming, I want to see the list of commands that my professor types into the text editor so that I can focus on the concepts being taught instead of memorizing keystrokes or falling behind in class. (falling behind)

  * We found this user story to be especially relevant, as it is the closest to our initial problem statement. In justifying it, it poses the question "Is it difficult to learn coding in a live setting where attention may be split" 
  
    A 2020 paper by Raj et al. compared the performance of students in the same class learning programming through either live-coding or static code examples, and found that there were minimal differences in performance. Additionally, they found that for students in the static code example version of the classroom, they had a higher extraneous load compared to students in the live-coding version of the class. They state:
    "Therefore, our experiment fails to show any differences between teaching programming using live-coding and static code examples with respect to student learning measured via paper-based tests. We found a statistically significant difference in the extraneous cognitive load imposed on the students in the two groups. 
  
    The extraneous load imposed on the students in the live-coding (experimental) group was significantly lower than the extraneous load imposed on the students in the static code examples (control) group." This shows that live-coding decreases the extraneous load on students’ working memory. One possible explanation could be that as code is developed in a step-by-step manner during live-coding, students know exactly which line of code to focus on, and therefore the extraneous cognitive load (i.e., load imposed on the working memory that is not directly helpful for learning) on the students is low and the students are able to use most of their working memory to focus on the learning task. On the other hand, in static code examples as the fully completed version of a code snippet is shown to students during a lecture, the students could feel overwhelmed seeing a full program (around 40 lines of code), and may be focusing on some unimportant elements in the program (e.g., include statements, function declarations) that might not directly help them with their conceptual understanding, which in turn increases their extraneous cognitive load.

    Their conclusion is that more study on the subject needs to be conducted to determine what the differences, advantages, and limitations of each style of teaching are. This ambiguity offers relevance to our user story, since in a future user study of our prototypes we can expand on the results of this research.

* As an instructor teaching an in-person programming class, I want the commands I type to be displayed so that the seating arrangement of my students does not impact their ability to follow my lecture and so they can focus on core concepts instead of text editor commands.

  * When drafting our user stories, we tried to keep all our stakeholders in mind and put ourselves in the shoes of an instructor. Most live-coding classes are taught by having the instructor share their screen on a projector for the rest of the class to see. With a high variance of classroom settings ranging from auditoriums to small rooms, we concluded that an instructor using a projector should not have to decide how to split screen real estate between a text editor and a prototype for our proposed problem, which would affect student's ability to see what is being done on the projector. Following this reasoning, we decided to keep this as a relevant user story.

* As a student who is not familiar with the text editor my professor is using, I want to see the list of commands my professor is typing and an explanation of the keystrokes so I can replicate the action in the same or a different text editor.
  * We kept this user story because it acknowledges the wide array of text editors (or even IDEs) that students have access to, and that due to personal preference students may decide to use an application different to the one an instructor uses during live in-person instruction. Using the empirical example of UGA computer science, first or second year students taking 1301, 1302, or 1730, among others, are typically expected to work in Emacs for their projects. This contrasts with data we presented in milestone 2 from a Stack overflow survey, which showed that there is a gradual transition away from text editors. Even among people who still use them, there is no clear favorite between Emacs, Vim, Nano, which means we can expect this to be a common scenario.

* As a student who has difficulties following along in class (due to visual or learning disabilities), I want the list of the commands my professor typed transposed into a format that I can access.

  * In the article *Rich Representations of Visual Content for Screen Reader Users* (2018) by Morris et al., they explore the limitations of alt text in screen readers for HTML and images, proposing 5 dimensions that could be used when designing alt text for screen readers (interactivity, stability, representation, structure,  and personalization). These dimensions guided the design of six initial prototypes from which they collected feedback in a user study, including the use of auditory cues or various drafts of alt text depending on the level of detail a user wanted. While feedback was collected for each specific dimension and varied in user reception, all participants found at least one of the prototypes to be an improvement over current interactions with alt text. 

    This demonstrates that our user story is initially viable because, when we consider how we will be translating text editor commands for students with a visual disability while in an in-person instruction setting, we will need to be mindful of the limitations of screen reader technology. Current standards for screen reader technology when accessing information is dated in some aspects, and when thinking about how we will create a solution for our problem accessible to all users these limitations will need to be addressed. But, in addition to proving our user story is initially viable, it helps guide our design process by providing a design framework we can use when deliberating representation of the text editor commands.

    Additionally, with the National Federation of the blind reporting in 2017 that 63,357 students from elementary to high school (up to the age of 21) and and approximation of 706,400 adults (age 16+) in 2016 identifying as visually disabled, accessibility to those with disabilities is a relevant user story for our problem statement.

 
*  Access to technology: Excluded for now, due to not being part of the problem statement.

   * While we considered the ability a student has to access the tools necessary for participating in class and the effect this could have on learning a text editor, we concluded that including this user story would deviate too much from our original problem statement. The problem we are hoping to solve is that of unfamiliarity with a text editor, which motivates students to try and learn a text editor at the cost of diverting attention from the lecture material. Some of our proposed solutions from other user stories may acknowledge the necessity to access text editor command sequences after a lecture, but this was not our focus. Additionally, with a lack of context derived from the lecture, these command sequences lack any meaning on their own and would require capturing more information than our other solutions currently demand.

## B: Ideation and Prelimary Designs

![Mural ideation board](https://github.com/jefferyjohn/hci4800/blob/main/images/ugahacks_mural.jpg)

### Class Size
* Display (on the student's screen) the last seven commands an instructor typed but allow students to scroll up to see more

* Display what the command is doing in addition to the command itself

### Textual Representation / Accessibility 
* Have commands be streamed to a platform that can read commands as audio for students if they use headphones

* Allow for night / light mode and color blindness filters

### Student Proficiency Level
* Plugin for natural language command typing. Instead of C + x s, type save

* Allow the student to access all commands, with the option to toggle / filter / translate / define the instructor's inputs

### Falling Behind
* Synced text editor that can just record the commands my instructor used and prompt me to activate them when ready

* Let students make notes/flag if they get confused somewhere so they can find their place later and notify instructors of these student interactions

### **Wireframes**

![Mural wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/ugahacks_m3_wireframes.jpg)

### Command Context
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D250%253A679" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/ugahacks_m3_display.jpg)

### Toggle Feedback

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D250%253A107" allowfullscreen></iframe>

[Link to wireframe - 1](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe.jpg)

[Link to wireframe - 2](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_1.jpg)

[Link to wireframe - 3](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_2.jpg)

[Link to wireframe - 4](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_3.jpg)

[Link to wireframe - 5](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_4.jpg)

[Link to wireframe - 6](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_5.jpg)

[Link to wireframe - 7](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_6.jpg)

[Link to wireframe - 8](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_7.jpg)

[Link to wireframe - 9](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_8.jpg)

[Link to wireframe - 10](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframe_9.jpg)

### Flag Commands
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D251%253A741" allowfullscreen></iframe>

[Link to wireframe - 1](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframeflag.jpg)

[Link to wireframe - 2](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframeflag_1.jpg)

[Link to wireframe - 3](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframeflag_2.jpg)

[Link to wireframe - 4](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframeflag_3.jpg)

### Color Accessible

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D251%253A932" allowfullscreen></iframe>

[Link to wireframe - 1](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor.jpg)

[Link to wireframe - 2](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor_1.jpg)

[Link to wireframe - 3](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor_2.jpg)

[Link to wireframe - 4](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor_3.jpg)

[Link to wireframe - 5](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor_4.jpg)

[Link to wireframe - 6](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframecolor_5.jpg)


### Display Last Seven Commands

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D251%253A1213" allowfullscreen></iframe>

[Link to wireframe - 1](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframelast7.jpg)

[Link to wireframe - 2](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframelast7-1.jpg)

[Link to wireframe - 3](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframelast7-2.jpg)

[Link to wireframe - 4](https://github.com/jefferyjohn/hci4800/blob/main/images/Wireframelast7-3.jpg)

### Natural Language Commands

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D251%253A1364" allowfullscreen></iframe>

[Link to wireframe - 1](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-14natural.jpg)

[Link to wireframe - 2](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-15natural.jpg)

[Link to wireframe - 3](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-16natural.jpg)

[Link to wireframe - 4](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-17natural.jpg)

[Link to wireframe - 5](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-18natural.jpg)

### Screen Reader

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D252%253A1418" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-19.jpg)

### Jumping Scroll

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D252%253A1427" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/Group-20.jpg)
## C: Detailed Designs

Many of our top ideas were chosen once we agreed on an assumption about how we want to implement our prototypes: aside from the instructor view of what's being projected on screen, there is a separate student interface which students can see on their local machine. 

To summarize our reasoning, we concluded that allowing students to interact with something on their local machines would provide more meaningful interactions through the affordances we could include and, in the case of accessibility ideas, it was necessary to provide a student interface to solve this problem. This also allows us to follow a key design principle we had not mentioned in Milestone 2: keep users in control. 

Since we put a lot of detail and effort into our low-fidelity mockups, the design changes we made for the high-fidelity mockup has little to do with the actual design of the application. Instead, the application was simply cleaned up and make more consistent with the other wireframes we have. We also provided notes to specify what each wireframe in the mockup is representing.
### Flag Commands

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D254%253A1440" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/flag-hf.png)

[Link to Figma source](https://www.figma.com/file/CSHkSKd5450K7fMmgOITnv/UGAHacks-Preliminary-Designs?node-id=255%3A1632)

We chose this as our top idea because it is helpful for both instructors and students. While it would be helpful for students to be able to ‘jump’ forward to where the professor is in the material, allowing students to flag commands and make notes is more beneficial to both the student and the instructor. 

Addressing student confusion is much more helpful than allowing students to press a button and skip past certian commands. Students using a text editor in class will most likely have to use a text editor outside of class as well. 

If students are able to make notes about a certian command and they are able to flag confusing commands, then these can be returned to at a later time and be addressed. 

### Toggle Commands

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D255%253A1634" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/toggle-hf.png)

[Link to Figma source](https://www.figma.com/file/CSHkSKd5450K7fMmgOITnv/UGAHacks-Preliminary-Designs?node-id=255%3A1633)

We chose this idea over the plugin because this idea includes the other one while also allowing for more user options. This idea best addresses our user story because it allows students to see the commands that they are most interested in. It also allows students to use the same text editor or a different one. 

In addition to the flexibility presented in this design, it is also better than the plugin because it allows a student to still view the commands the instructor is typing if they are attempting to learn the text editor commands. Our plugin idea takes away the opportunity for students to become familiar with the text editor keystrokes, and therefore the opportunity to learn these keystrokes over time. 

### Color Accessible

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D255%253A2205" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/accessible-hf.png)

[Link to Figma source](https://www.figma.com/file/CSHkSKd5450K7fMmgOITnv/UGAHacks-Preliminary-Designs?node-id=255%3A2205)

We chose this as our top idea because it serves to help more people in terms of accessibiliy when using the application. While it would be helpful for people to be able to easily use a screen reader with our application, there is a smaller pool of users this idea would apply to. According to colorblind.org, 3.7% Americans are colorblind. While this is not a majority of people, it is still a significant number of people who could benefit from an application that is sensitive to those with color blindness. 

According to the National Federation of the Blind, 2.4% of Americans have a visual imparement. This imparement does not include those who are color blind. These statics can be found on this page: https://nfb.org/resources/blindness-statistics. Since there are more people who are color blind than those with visual imparements that would require a screen reader, addressing the issue of color in our application is the idea we chose. 

Since we put a lot of detail and effort into our low-fidelity mockups, the design changes we made for the high-fidelity mockup has little to do with the actual design of the application. Instead, the application was simply cleaned up and make more consistent with the other wireframes we have. We also provided notes to specify what each wireframe in the mockup is representing.

### Display Last Seven Commands

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FCSHkSKd5450K7fMmgOITnv%2FUGAHacks-Preliminary-Designs%3Fnode-id%3D255%253A2488" allowfullscreen></iframe>

[Link to wireframe](https://github.com/jefferyjohn/hci4800/blob/main/images/seven-hf.png)

[Link to Figma source](https://www.figma.com/file/CSHkSKd5450K7fMmgOITnv/UGAHacks-Preliminary-Designs?node-id=255%3A2488)

We chose this as our top idea because it incorperates the best parts of the other idea into its design. This design lists the last seven commands the instructor typed. In the design it also displays both the command and the action it was associated with. By logging into the application with the student and instructor ids, there is more clear how an instructor and student are able to connect so that the instructor commands are displayed for students. 

## D: Summary Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/mvKQg_h_mT4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Link to summary video](https://www.youtube.com/watch?v=mvKQg_h_mT4)

## E: Citations

    Morris, M. R., Johnson, J., Bennett, C. L., & Cutrell, E. (2018). Rich Representations of Visual Content for Screen Reader Users. _Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems_. Published. https://doi.org/10.1145/3173574.3173633

    Adalbert Gerald Soosai Raj, Pan Gu, Eda Zhang, Arokia Xavier Annie R, Jim Williams, Richard Halverson, and Jignesh M. Patel. 2020. Live-coding vs Static Code Examples: Which is better with respect to Student Learning and Cognitive Load? In <i>Proceedings of the Twenty-Second Australasian Computing Education Conference</i> (<i>ACE'20</i>). Association for Computing Machinery, New York, NY, USA, 152–159. DOI:https://doi.org/10.1145/3373165.3373182

    National Federation of the Blind. (2019). _Blindness Statistics_. Retrieved November 7, 2021, from https://nfb.org/resources/blindness-statistics

    Medline Plus. (2021). _Color vision deficiency: MedlinePlus Genetics_. Retrieved November 7, 2021, from https://medlineplus.gov/genetics/condition/color-vision-deficiency/#frequency


#### [Back to Homepage](./)
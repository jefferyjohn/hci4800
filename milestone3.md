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
 
*  Access to technology: Excluded for now, due to not being part of the problem statement.

   * While we considered the ability a student has to access the tools necessary for participating in class and the effect this could have on learning a text editor, we concluded that including this user story would deviate too much from our original problem statement. The problem we are hoping to solve is that of unfamiliarity with a text editor, which motivates students to try and learn a text editor at the cost of diverting attention from the lecture material. Some of our proposed solutions from other user stories may acknowledge the necessity to access text editor command sequences after a lecture, but this was not our focus. Additionally, with a lack of context derived from the lecture, these command sequences lack any meaning on their own and would require capturing more information than our other solutions currently demand.

## B: Ideation and Prelimary Designs

![Mural ideation board](/images/ugahacks_mural.jpg)

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

**Wireframes**

[screenshot of all wireframes]

[each wireframe embed with justifications]

## C: Detailed Designs

[png of wireframe]

[justification of wireframe]

[download link to source of file]

## D: Summary Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/mvKQg_h_mT4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Link to summary video](https://www.youtube.com/watch?v=mvKQg_h_mT4)

#### [Back to Homepage](./)
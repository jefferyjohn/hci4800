# Milestone 2
### Group / Team Name: 
UGAHacks
### Group Member Names:

Calla Corder (calla.corder@uga.edu)

Jeffery John (jeffery.john@uga.edu)

Mathew Suarez (mathew.suarez@uga.edu)

## A: Task / Problem Definition

### Problem Introduction

**Describe problem of study (use terms like properties, affordances, signifiers)**

In a given classroom, virtual or in person, in which students are following along with a teacher’s coding instructions, there are often times in where the teacher saves and exits from a command-line text editor, like Vim or Emacs, using a command string that is obvious to themselves but may not be obvious to a given student who is unfamiliar to said editor. Unfortunately, due to the traditional convention of command-line text editors, there is an apparent lack of affordances, what the commands may do, and signifiers, what the commands can do. This may lead to students falling behind on the lesson and in turn becoming more worried on how to follow along as opposed to the material attempting to be taught. 

This is the problem that we hope to solve. More concretely, we hope to decouple a given action within a command-line text editor and the text editor itself. This will, in turn, allow understanding of the material being taught without the prior knowledge of a specific text-editor’s encoded actions. 

**Why is it a problem?**

The problem is a natural result of an overabundance of text-editors available for users to choose from. While Vim and Emacs are the most popular choices, there are a plethora of alternative options for developers to choose from to meet specific needs or wants. Nano, Tilde, Neovim, Vi, and Gedit are just a few examples of such alternatives. Each of these text-editors have their own list of commands which can number in the hundreds. This abundance of choice, coupled with the number of commands, naturally leads to a significant learning curve in learning or following along on a new text-editor.

**How is it theme-relevant?**

In both beginner and intermediate programming courses, command-line text editors are incredibly commonplace. Hence, students are often in scenarios where the instructor utilizes a text editor the student is not familiar with. By attempting to tackle this issue, face-to-face instruction in scenarios in which text editors are used can be more focused on the material being taught as opposed to the commands of the text editor being used.

**Typical interaction related to problem**

Often, the instructor will be teaching something independent of the text editor being utilized. For example, an instructor may be teaching the difference between the syntax of different types of methods within a given programming language. In order to better compare and contrast these types of methods, the instructor may split their text editor to showcase two screens at once, each showing a different method type. 

A student following along with the instruction may be confused as to how this action was done and pause instruction in order to inquire about how to do this action within their own environment. In this scenario, the action itself is not relevant to the material being taught, but the instruction was still paused to address the question at hand.

**7 Stages of Action**
* Goal - student completes an action that an instructor completed in class
* Plan - student ensures they have the same environment 
* Specify - student discerns what action the instructor has taken
* Perform - student executes the action
* Perceive - student examines the environment response to their action
* Interpret - student determines the result of their action
* Compare - student compares the result of their action to the result of the instructor

**How do we know this interaction is typical?**

We can conclude that following, and in turn learning, a completely new text editor can be difficult for novice users, the majority of whom can be found in entry and intermediate level programming courses, because of prior research on similar problems. For example, the paper “Effects of Experience on Learning, Using, and Evaluation a Text Editor” published in 1984 by Mary Beth Rossen, stated that “...the less sophisticated users were not as likely to rely on the manual or on experimentation for their initial exposure to Xedit, that they tended to rely to a greater extent on their friends than did the more sophisticated users. This implies that the availability of some interactive source of information may be critical for novice users.”

With the above statement in mind, we note that there are very few text editors which provide this interactive source of information. Nano does provide a source of information by displaying common commands at the bottom of its GUI, however this cannot be expected from a large majority of popular text editors such as Vim and Emacs. With that being said, we can safely assume that this lack of information leads to our aforementioned interaction being commonplace in programming classes in which novice users are prevalent.
### Potential Users

**What user population is affected by your problem of study?** 
	
The primary user population affected by this problem is anyone learning to use a new text editor. The users can range from college students to professionals, but each is a student learning an editor. It is evident that text editors must be learned according to a research done by Douglas and Moran (1983) as they state that, 


Learning begins with the learner putting together a rough problem space for text editing from the teacher's instructions. But, when confronted with editing tasks to do, the learner finds the rough problem space is not yet good enough to support effective problem solving. (207)

Students cannot just copy commands to learn them. Those beginning with a new text editor do not have all of the necessary background to be successful in using an editor. 
 
As text editors must be taught, there is a second population affected by this problem, instructors. Since the rough problem space instructors create is not sufficient for students to learn a new text editor, instructors must do more to teach how to use a text editor. Class time is taken up by instructors having to explain the steps they just completed and repeating commands. This allows students to learn the commands over time, but is time consuming, distracting from the concepts that instructors are trying to teach in the text editors. 

**What related tasks do they perform?**

In order to use a new text editor, a person needs to type in the text editor. Users must use shortcuts and keybindings to type and execute commands. Keybindings are different for each text editor. According to Walker and Olson (1998), "these special key combinations have a speed advantage...however the time advantage gained from fewer hand movements could easily be outweighed by slow, difficult memory retrieval or, worse yet, by an error" (p. 201). Each text editor has its own list of special commands and keybindings that a user must remember. Since, according to Shneiderman et.al (2017),  a person can only remember 7 +- 2 chunks of memory at a time, it is a struggle for students to remember more than 7 commands at a time. As a teacher shows students how to complete tasks with a text editor, they will likely type many more than seven commands in one sitting.
 
This problem affects both students and instructors in a face-to-face setting. Students must attempt to follow along with a teacher’s commands, whether they have a computer with them or not. If students do not have a computer with them, it can be challenging to write down all of the commands for the text editor in addition to the concept being covered. Even if a student has the text editor open in front of them, it is easy to get lost and be unable to catch up. If a student falls behind by their maximum short-term memory capabilities, they will be unable to catch up. They must either ask the instructor to stop class and review the necessary commands, or be unable to follow along with the rest of the lesson. 

**How would users benefit from a solution (not necessarily your solution) to your problem of study?**

Not all people have the same ability to learn a new text editor. According to Egan et. al (1982), "learning to use a text editor was strongly associated with reading skill, spatial memory, and age" (p. 339). By creating a tool for all users, the three characteristics of learning a text editor could be supplemented so that it is easier for all people to learn how to use a new text editor. This is essential for a face-to-face learning environment which is often fast paced. 

As students learn in a face to face setting, they would be able to complete tasks faster and would not fall behind in class due to a difference in learning capability. A solution would also allow students who did struggle to have a way to review commands without disrupting their learning or anyone else’s learning. By providing a solution to this issue, instructors would also benefit because they will lose less class time re-explaining material. Providing a solution also allows for both the instructor and students to focus more on the concepts being covered instead of details related to text editors. 

## B: Analysis of Existing Solutions


### Common Trends

We examined existing tools, and determined that many aimed to perform one or more of the following:
* Display platform-specific commands, real-time
* Unify platforms
* Provide inear walkthrough, platform-specific, static 
* Act as static resource
* Perform platform-platform translation
* Demo: [MIT’s Missing Semester](https://missing.csail.mit.edu/2020/editors/ )
 


### Existing Solutions

* [tarsius/keycast](https://github.com/tarsius/keycast)
    * Shows current command and its key in the mode line 
    * While keycast does display the current command and its key or mouse binding, it does not translate this across platform
* Standardized terminal environments
    * [Visual Studio Code Development Containers](https://code.visualstudio.com/docs/remote/create-dev-container)
    * [GitHub Codespaces](https://github.com/features/codespaces)
    * While they do eliminate platform-specific differences, they do not uniquely address in-person instruction needs.
* Walkthroughs
    * [CodeTour](https://marketplace.visualstudio.com/items?itemName=vsls-contrib.codetour&WT.mc_id=javascript-17914-aapowell)
    * [Vim Tutor](http://www2.geog.ucl.ac.uk/~plewis/teaching/unix/vimtutor)
    * While CodeTour and Vim Tutor do allow for users to be guided through commands, they are on a linear path, that is not effective for dynamic teaching environments or uniquely address in-person instruction needs
* [tldr-pages/tldr: 📚 Collaborative cheatsheets for console commands](https://github.com/tldr-pages/tldr) 
    * While useful for independent, individual users, tldr is not meant to serve as an automatic instructional aid running in parallel with live workshops
* [emacswiki.org/emacs/VimMode](https://www.emacswiki.org/emacs/VimMode)
    * While useful for independent, individual users, Vim Mode is not meant for ease of use in translating between instructions, only accessing Vim specific instructions and functionality
* Visualizing
    * [Git](https://github.com/git-learning-game/oh-my-git) 
    * [Data structures](https://addyosmani.com/blog/visualize-data-structures-vscode) 
    * Not applicable to text editors

**Surveys**
* [StackOverflow](https://insights.stackoverflow.com/survey/2019/#development-environments-and-tools 
)
    * Sentiment seems to imply that transitioning away from command-line interfaces toward text editors such as Visual Studio Code is the status quo. With little tools available for synchronous command line interface instruction, it seems that most users learned independently, outside of the classroom.

### Potential Guidelines and Solutions

After identifying the main functionality of these alternatives and the guidelines they adhere to, we have concluded that the main principles of the 8 Golden Rules we need to adhere to are:

* Seek universal usability. Student users with varying levels of familiarity with text editors should all be able to benefit from the benefits of a class that utilizes our solution.
* Prevent errors. Instructors are our other stakeholders, and in using our solution to compliment their existing teaching structure they should not have additional bugs to navigate. This also benefits our student users, who can focus on following along with the coding example without the stress of their application failing.
* Permit easy reversal of actions. Instructors can make mistakes when inputting a command sequence, and should be able to correct those mistakes so that their students don’t recreate them.

In addition to these guidelines, we will also follow the principles of understandability, operability, and perceivability, and robustness, which are outlined in the WCAG 2.0. Of these, the guidelines to keep most in mind are:
* Guideline 1.3 Adaptable: Create content that can be presented in different ways (for example simpler layout) without losing information or structure.
* Guideline 1.4 Distinguishable: Make it easier for users to see and hear content including separating foreground from background.
* Guideline 2.4 Navigable: Provide ways to help users navigate, find content, and determine where they are.
* Guideline 3.1 Readable: Make text content readable and understandable.

These will guide decisions leading to a universally accessible solution that can reach students with visual impairments and other disabilities.


### Existing Solution Review

In researching existing solutions we could not identify a mainstream option for addressing the problem we have zeroed in on. From the list we compiled, we identified common trends among these alternatives, which were: displaying platform-specific commands, real-time; displaying keyboard command inputs in an overlay; unifying different platforms to be contained in a single application; providing linear, platform-specific walkthroughs; utilizing static resources, like images; implementing forms of platform-platform translation. We narrowed down this list to those with feature sets we would initially consider most relevant, and identified if/what guidelines and principles they adhered to. 
Across these alternatives, the first question considered was whether they adhered to the standards needed to be considered universally accessible, or met the requirements needed to satisfy WCAG 2.0. This is relevant because based on a developer survey published by stack overflow in 2021 (cite), the most common disability among those who self-reported was blindness/visual impairment. Following this, many of the alternatives considered don’t seem to work in an in-person instruction setting for our problem statement if they aren’t running locally, since they require students to look at a projection of the instructor's laptop. 

Recognizing this limitation, we abstracted the most import principles of the 8 Golden Rules of Design used by  this list of alternatives:

* Tarius/Key Cast

    * As an Emacs package, this alternative does well by being consistent with how other Emacs packages are installed and downloaded by users, in addition to being a minimal addition to the existing Emacs interface. On top of this, the package prevents user errors since they main functionality is to display the name of the most recent command, but doesn’t include any additional affordances to the Emacs editor.

* Code Tour

    * This alternative allows users to remain in control of the interface, offering a wide range of affordances which are mapped to their appropriate signifiers, and stay consistent with the existing Visual Studio layout. While recording a tour, changes can be made without having to start from the beginning, ensuring that users can reverse and alter previous actions. Finally, the application uses dialog boxes to indicate what step of the tour recording users are on and how to move forward, and limit actions based on this. This design prevents errors by clearly expressing what is expected of a user and yields closure, since users know what the next step in finishing the recording is.

* Tldr-pages

    * As an external package to improve an existing feature (the man pages), this solution focuses on keeping users in control by not changing existing functionality, but rather enhancing the clarity of it. Another notable aspect of this solution is the ability users have to contribute to the project. Through this, universal accessibility can be reached as contributors add new translations for languages that haven’t been added or edit the simplified markdown files for a specific function.

* Vim mode for Emacs

    * Another Emacs package, Vim mode succeeds at keeping users in control by not making any changes to the interface, even when they’ve adding Vim key-bindings to the editor. 

* Misc. software for displaying key presses and mouse clicks

    * These software programs are diverse, but the most common thing is that they use an interface design that is consistent with other lightweight desktop applications for recording a screen or saving the commands to a text file. On top of this, these applications focus solely on displaying the most recent key commands and mouse clicks on screen, and reduce errors by having limited functional affordances alongside this. A lackluster aspect of these programs is their inability to reverse actions, since if the program is currently recording the inputted commands or key presses, any mistakes cannot be edited out for clarity.
## C: Proposed Solution


### Proposed Solution

Following all this information, our initial proposal for a solution is to implement an interface that can run parallel to a text editor of choice and record the name of the inputted command sequence and its key sequence. 

To accommodate students with disabilities, an affordance we can include is the ability to run a local student instance of the interface which can sync to the instructor’s, allowing for the use of screen readers, enlarged text, or other accommodating technology. For instructors, to allow them to edit their key sequences quickly during instruction, and additional affordance would be to always show them a list of their most recent actions, with the option to delete commands that they may have inputted incorrectly. 

Additionally, to be universally usable, we would want to try to include the affordance of translating specific commands from one text editor to another, so that a novice student using Emacs can still follow along with an instructor using a foreign command in Vim.

This would differ from existing solutions in that it would be able to act as a multi-platform tool, while allowing for dynamic response to instructions and provide additional afforances for students who may need them. Other multi-platform tools are limited in what conversions can be made, whereas ours would allow for students to intuitively understand the commands used, without an equal imperative for understanding associated keybindings.
### Measuring Success

To measure success of our solution, the use of surveys and bug reports would be our most effective ways of ensuring our design was a success. Through user surveys we can probe for overall satisfaction of our design and collect statistics regarding user disability and helpfulness of our product, and collect written feedback on how we could improve. By collecting bug reports, we can ensure that our program runs as smoothly as possible, emphasizing our desire to be an enhancement to live instruction rather than a detriment.

## D: Summary Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/6bMpsxV0UZk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## E: Citations
    Egan, D. E., Bowers, C., & Gomez, L. M. (1982). Learner Characteristics That Predict Success in Using a Text-Editor Tutorial. Proceedings of the 1982 Conference on Human Factors in Computing Systems, 337–340. Presented at the Gaithersburg, Maryland, USA. doi:10.1145/800049.801806

    Douglas, S. A., & Moran, T. P. (1983). Learning Text Editor Semantics by Analogy. Proceedings of the SIGCHI Conference on Human Factors in Computing Systems, 207–211. Presented in Boston, Massachusetts, USA.

    Rosson, M. B. (1984). Effects of Experience on Learning, Using, and Evaluating a Text Editor. Human Factors, 26(4), 463–475. https://doi.org/10.1177/001872088402600409

    Shneiderman, B., Plaisant, C., Cohen, M., Jacobs, S. M., & Elmqvist, N. (2017). Designing the user interface: Strategies for effective human-computer interaction (6th ed.). Pearson.

    Walker, N., & Olson, J. R. (1988). Designing Keybindings to Be Easy to Learn and Resistant to Forgetting Even When the Set of Commands is Large. Proceedings of the SIGCHI Conference on Human Factors in Computing Systems, 201–206. Presented in Washington, D.C., USA. doi:10.1145/57167.57201


#### [Back to Homepage](./)
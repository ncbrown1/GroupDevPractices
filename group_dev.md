# Group Programming Practices 

Let's say we want to start this new project (call it *Boomerang*, for all intents and purposes). Boomerang is a HUGE project and requires many different types of expertise (i.e. front end + back end + scripting + api work + ... ). Because of this, Boomerang cannot be completed by just one person; we must complete it as a _team_. Let's assume that you (the reader) have only programmed by yourself and do not know how to collaborate effectively with other programmers. Read the following carefully.

## Agile Manifesto (http://agilemanifesto.org/)

**_Individuals_** and **_Interactions_** over processes and tools.  
**_Working Software_** over comprehensive documentation.  
**_Customer Collaboration_** over contract negotiation.  
**_Responding to Change_** over following a plan.  

While there is value in items on the right, we value items on the left _more_.

## Scrum/Agile Meeting

"Since last meeting, I have worked on X, and made progress with Y. Until next time, I hope to work on Z so that we/I can V." 

Each team member should do this, then conclude with "Meeting Over. Break." or some other closing statement.

## Scrum

The first step is coming up with an **_idea_** (in our case, this is Project Boomerang). 

In order start doing scrum, we must break this idea down in ways that make it _actionable_ and _increment-able_. To do this, we create a list/stack of requirements and objectives (usually user stories) ordered by their priority level (i.e. most important ones will be higher in the backlog, less important but desirable ones will be lower). This list/stack of requirements is called the **Product Backlog**, and must be completed before even starting on the project and starting to do Scrum.

Now that we have our product backlog, we can start organizing our team. The team is comprised of the following:
* Product Owner
  * Represents the interests of the business, customers, or users to the team. 
  * A lot like an investment manager. 
  * Maximizes overall end-product return value. Makes sure the team is always working on the most _valuable_ things.
  * May instruct team to defer or cancel certain objectives in favor of objectives that the stakeholders deem more prioritizing.
  * Makes sure that each team member fully understands each task and what it is comprised of. This ensures we are creating the _right_ thing. (This may involve asking for outside help)
* Scrum Master
  * Helps the team becomes a _high-performing_ team. In other words, the Scrum Master gets the team in their "groove".
  * Removes impediments from current and future work.
  * The local Scrum expert, who knows the most about Scrum.
* Team Member(s)
  * Helps the team deliver stories.
  * Don't do "my job", do **the** job.

Okay, now we have the product backlog and our team to help complete it. Now how do we go about actually completing the work? Usually, this is done in cycles of **_sprints_**. A sprint is a fixed amount of time, usually 1 or 2 weeks (sometimes but rarely 4), in which the team quickly fulfills user stories and removes them from the backlog. The process of doing so is as follows:

1. Sprint Planning Phase
  * What - which stories off the top of the backlog can the team commit to delivering during this sprint?
  * How - how is the team actually going to do the work to deliver these stories?
    * Usually involves breaking down stories into **_tasks_**.
1. Now we have a list of Stories and a longer list of Tasks. 
  * Some tasks may not connect directly to any of the stories committed to during this sprint cycle.
1. The Daily Scrum
  * A daily meeting where we inspect and adapt for the **_sprint_**.
  * For the team to identify in what ways we are off track in terms of delivering stories.
  * Discuss ways to adjust. Might be immediately decided or may be discussed after the daily scrum and announced to the team later.
  * No more than 15 minutes.
1. The Sprint Review
  * This is the public end of the sprint where we inspect and adapt for the **_product_**.
  * Invite all stakeholders we can to the meeting and show them what was accomplished during the sprint.
  * Transparency is key: What did get accomplished? What _didn't_?
  * Shows how the product has evolved since the last product.
1. The Retrospective
  * Takes place immediately after the sprint review where we inspect and adapt for the **_team_**.
  * This is private, and the stakeholders are no longer present in this meeting.
  * For the team to look back at the sprint and figure out what we learned as a team and what we want to try differently going forward.
1. Repeat from the beginning.

Sometimes the team may take time away from the sprint and do a smaller, informal meeting called **_"story time"_**, where the team inspects the current state of the product backlog. At this time, we can put estimates on stories that do not have estimates yet (in terms of difficulty), refine acceptance criteria, or break big stories up into smaller stories. This is so that the top of the backlog is in good shape for the next sprint cycle.

<!-- !sprint-cycle.jpg! -->
![alt tag](https://raw.github.com/ncbrown/GroupDevPractices/master/sprint-cycle.jpg "Sprint Cycle Diagram")

If you want to read more on this, check out the following webpage: http://www.agilelearninglabs.com/resources/scrum-introduction/

## Kanban

A newer alternative to Scrum is Kanban, which is continuous and incremental as opposed to broken down and distributed. In most cases, using Kanban will be extremely similar to using Scrum. Since we've described a lot of Scrum already, we will just summarize Kanban in terms of Scrum and how it differs.

The Kanban process starts the same: come up with an **idea** and break it down into a list of **stories** (optionally organized by priority). Then, the team is formed.

In Kanban, the team is exactly the same, except the Scrum Master is be replaced with a Kanban Master. The Kanban Master is the same, except they are experts in Kanban and would be in charge of organizing and documenting each section of the Kanban board.

The biggest difference Kanban makes from Scrum is in the workflow. Instead of having a cycle of sprints, there is a continuous flow of stories across the board (usually from left to right, or "not started yet" to "done"). There are many ways to configure a Kanban board, but the following is a typical configuration:

1. Icebox
  * Sometimes referred to as "Ice Box", "Long Term", "Goals", "Desired".
  * This is an optional section where you may place stories which are not immediately required to complete the product.
1. The Backlog
  * Sometimes referred to as "Backlog", "New", "To Do", "Not Started", "Important".
  * These stories can be broken up into smaller stories, which also get placed in the "To Do" section.
  * Stories are taken from here and placed into an "in-progress" section.
1. Prioritized
  * Sometimes referred to as "Prioritized", "Hotfixes", "Urgent".
  * This is where stories that need immediate attention are placed.
  * Stories in this section take precedence over anything in the Backlog.
1. In Progress
  * Sometimes referred to as "In Progress", "Development", "Ongoing".
  * Stories in these sections are being actively worked on by their assignee.
  * This section can be broken down into subsections to describe status of progress, such as "Working", "Stuck", or "Needs Review".
  * Once a story is completed, it is moved to the next section, which may be "Done" or "Ready"
  * Usually, a VCS commits are tagged in the comments before moving them on.
1. Ready
  * Sometimes referred to as "Ready", "Ready for Test", "Test", "Review".
  * Stories in this section are currently in somewhat working condition. The product is tested by a supervisor or peer before moving to "Done".
  * If the progress on this story is not up to par, problems should be listed as necessary in the comments and the story will be moved back into "In Progress".
1. Done
  * Sometimes referred to as "Done", "Release", "Ready for Production".
  * Stories in this section have been vetted and tested thoroughly and are ready for the next release.
  * Once a release takes place, all stories in this section corresponding to that release are tagged with that release number or archived.
1. Archive
  * Sometimes referred to as "Archive", "Old", "History".
  * This is where stories from previous releases are placed. These stories are only for reading purposes. They should not be acted on.
  * If a bug is found or a hot-fix is needed for a story in this section, a new issue must be created that references that story.

You, as a developer, are responsible for doing work to move stories from the beginning of the board to the end. As you complete or make progress on stories or tasks, you should document that progress in comments on that particular story. Also, you must "limit your work in progress". Work at each stage is limited, as there should only be a small amount of work in progress at any given time. This ensures a fast, smooth flow of stories across the board. If you are stuck without work when the WIP is high, utilize the slack time to relieve any bottlenecks in the system, learn and innovate, or maintain other systems.

Similar to Scrum, there are meetings at the beginning of every work day or shift. However, that is mostly it. These meetings will be between certain members of the team and the product owner (typically your manager), and facilitate the full understanding of the current tasks at hand in the development phase. There may be occasional meetings between the product owner, stakeholders, and team members to update everyone on the overall progress of the product. At this time, proper adjustments are made in the form of tasks and user stories.

<!-- !Kanban-board.png! -->
![alt tag](https://raw.github.com/ncbrown/GroupDevPractices/master/Kanban-board.png "Kanban Board Example")

## Git/VCS

In most cases, each git commit will correspond directly to a story or a task defined in a sprint. Each commit should be reviewed and vetted in a local branch before pushing to the master repository. Once a commit is made, paste a link to the commit onto the issue/story/task entry in the project's issue tracker and if the task has been completed, mark it as so. For an example of a successful git model, read the following article and diagram.

http://nvie.com/posts/a-successful-git-branching-model/  

<!-- !git-model.png! -->
![alt tag](https://raw.github.com/ncbrown/GroupDevPractices/master/git-model.png "Git Branch Model Diagram")
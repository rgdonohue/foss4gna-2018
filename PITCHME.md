# New maps in<br> the new medium

## Teaching web cartography<br> for a distributed workforce  
<br><br>
[Rich Donohue](https://twitter.com/rgdonohue)  
[Matthew W. Wilson](https://twitter.com/wilsonism)

---

## Rich Donohue

@div[left-40]
![](assets/images/donohue.jpg)
@divend

@div[right-60]
@ul
- PhD in Geography from the University of Wisconsin-Madison
- from a small town in Southwest Colorado
- teaches web cartography for New Maps Plus
- is currently introducing this talk
@ulend
@divend

---

## Matthew W. Wilson

@div[right-40]
![](assets/images/wilson.jpg)
@divend

@div[left-60]
@ul
- PhD in Geography from the University of Washington
- from a small town in northwest Missouri: Pumpkin Center
- new book [New Lines: Critical GIS and the Trouble of the Map](https://www.upress.umn.edu/book-division/books/new-lines)
- learned Markdown and Git for this presentation
- <i>and obviously not very well</i>
@ulend
@divend

---?image=assets/images/storytime.jpg

### Story time

---?image=assets/images/harvard-divinity.jpg

### Story time

---?image=assets/images/harvard-memorialhall.jpg

### Story time

---

### Story time: SYMAP?

---

### CARD MAPPING --> SYMAP

@div[left-50]
<br>
<br>
<br>
![](assets/images/horwoodmap.jpg)
@divend

@div[right-50]
![](assets/images/fisher-benson-symap.jpg)
@divend

---?image=assets/images/symap-map.png

### Map produced from SYMAP, ca. 1967

---?image=assets/images/symap-assignment.png

### Assignment from SYMAP<br> correspondence course, ca. 1967

---?image=assets/images/symap-coding-form.png

### SYMAP correspondence<br> coding form, ca. 1967

---?image=assets/images/nmp-website.png&size=auto

### [New Maps Plus<br> at the University of Kentucky](https://newmapsplus.uky.edu/)

---

### [New Maps Plus<br> at the University of Kentucky](https://newmapsplus.uky.edu/)

@div[right-60]
![](assets/images/nmp-website.png)
@divend

@div[left-40]
@ul
- began in Fall of 2015
- offers 12+ courses per year
- nearly 170 students have completed coursework
- 56 students have graduated with a certificate
- around a dozen more currently taking 'post-certificate' courses
@ulend
@divend

---

### New Maps Plus learning objectives

@div[right-60]
![](assets/images/web-mapping-workflow.png)
@divend

@div[left-40]
<br>
@ol
- apply traditional cartographic principles to web mapping
- employ open source tools for geospatial processing and data analysis tasks
- master web design and development using open standards to make maps
@olend
@divend

---?image=assets/images/tools.png&size=auto

### Some of our favorite tools

---?image=assets/images/tools2.png&size=auto

### What we're talking about today

---?image=assets/images/tools2.png&size=auto

### What we're talking about today

@div[left-40]
<br>
**Wait, but what is Git?**
<br><br>
@ul
- distributed version control system
- open source de facto standard integrated with GitHub
- works well with text-based information like code and Markdown
@ulend
@divend

---?image=assets/images/tools2.png&size=auto

### What we're talking about today

@div[left-40]
<br>
**What is GitHub, then?**
<br><br>
@ul
- for-profit company hosting Git-enabled repositories
- provides additional web services (Issue tracking, project Wiki)
- offers (free) web-hosting ... great for student maps and portfolios!
@ulend
@divend

---?image=assets/images/tools2.png&size=auto

### What we're talking about today

@div[left-40]
<br>
**Okay, and what is Markdown?**
<br><br>
@ul
- lightweight syntax written in plain text
- used for rendering text content, images, code snippets, and URLs in a web document
@ulend
@divend

---

### Where this talk is heading?

@div[left-60]
<br>
@ol
- Using Git and Markdown for course development and management
- How using Git improves the learning process
- The role Git in collaboration and community building
@olend
@divend

@div[right-40]
![git tree](assets/images/git-tree.png)
@divend

---?layout:center

#### Part I. How we use Git and Markdown for<br> <b>course development</b> and management

@div[left-50]
![git and markdown](assets/images/git-markdown.png)
@divend

@div[right-50]
![npm certificate program](assets/images/certificate.png)
@divend

---?image=assets/images/course-master-repo.png&size=80% auto

### All content created in a<br> course "master" repo

---?image=assets/images/course-module-repo.png&size=80% auto

### Individual modules contain drafts of lessons, labs, and solutions

---?image=assets/images/markdown-lesson.png&size=80% auto

### Lessons are written<br> using Markdown

---?image=assets/images/lesson-readme.png&size=80% auto

### Content is immediately ready for deployment and digestion

---

### Animated GIFs embedded in lessons are useful

![gif](assets/images/markdown-gif.gif)

---?image=assets/images/lesson-solution.png&size=80% auto

### Repositories hold all files and (most) data

---?image=assets/images/lesson-dev-tracked.png&size=80% auto

### And changes in content<br> are tracked through Git

---

### If we want to get fancy, npm and Node scripts are used to automate course management tasks

```javascript
const markdownpdf = require("markdown-pdf");
const fs = require("fs");

// read course syllabus in Markdown
fs.createReadStream("./syllabus.md")
    .pipe(markdownpdf())

    // create PDF version to file with Uni bureaucracy 
    .pipe(fs.createWriteStream("MAP_673_Syllabus.pdf"));
```
---
### Using Git and Markdown<br> for course management?

@div[left-40]
![management question](assets/images/course-question.png)
@divend

@div[right-60]
@ul[icon-list]
- @fa[thumbs-up fa=5x fa-green] centralized workflow for course creation and maintence
- @fa[thumbs-up fa=5x fa-green] easy to share course repo with other schools/instructors (builds community)
- @fa[thumbs-up fa=5x fa-green] format for writing and editing content ready for course deployment
- @fa[thumbs-down fa=4x fa-red] using Git is complicated
- @fa[thumbs-down fa=4x fa-red] is difficult getting all faculty buy-in
- @fa[thumbs-down fa=4x fa-red] doesn't do much for Geospatial data stored as binary
@ulend
@divend

---

#### Part II. How using Git improves<br> the learning process

---?image=assets/images/hello-world.png&size=90% auto

### New Maps Plus begins with students creating a GitHub account

---?image=assets/images/github-repo.png&size=90% auto

### GitHub repos are <br>new de facto resume

---?image=assets/images/github-classroom.png&size=90% 90%

### Highly recommended:<br> Use GitHub Classroom!

---?image=assets/images/starter-template.png&size=80% auto

### Starter template for each<br> course module

---?image=assets/images/github-classroom-lessons.png&size=80% auto

### GitHub Classroom creates invitation links from starter templates

---

### Student repos created<br> from starter template

@div[left-50]
![starter template](assets/images/starter-copied.png)
@divend

@div[right-50]
<br>
@ul[icon-list]
- @fa[thumbs-up fa=5x fa-green] Repos are private and part of the NMP GitHub account
- @fa[thumbs-up fa=5x fa-green] Instructor already has admin and collaborative rights
- @fa[thumbs-down fa=4x fa-red] Module not hosted on student's account
- @fa[thumbs-down fa=4x fa-red] Difficult for student peers to help each other
@ulend
@divend

---

### Student process for each weekly module

@div[left-50]
<br>
@ol
- accept invitation link and clone repository
- read lesson within README.md file
- create files and edit code
- add, commit, and push changes using Git through progress
@olend
@divend

@div[right-50]
![github desktop](assets/images/github-desktop.png)
@divend

---

### When students need help

@div[left-50]
<br>
@ol
- student adds/commits and pushes changes up to their repo.
- instructor then clones student repo to local (or pulls down recent changes)
- instructor branches and examines/tests/edits code
- instructor pushes up branch for student to examine (or to potentially merge with their master)
@olend
@divend

@div[right-50]
![git feedback](assets/images/git-feedback.png)
@divend

---

### Instruction facilitated by <br> the latest tools of the trade

@div[left-50]
<br>
@ol
- Slack interface allows for fast back and forth feedback
- screensharing and video conferencing compliment Git process
- very few emails!
@olend
@divend

@div[right-50]
![slack](assets/images/slack.png)
@divend

---
 
 ### Assignment evaluation and feedback

![eval pull request](assets/images/eval-pull-request.png)

--- 

 ### Assignment evaluation and feedback

![eval pull request](assets/images/feedback-code.png)

--- 

 ### Assignment evaluation and feedback

![eval pull request](assets/images/quiz-answers.png)

---

### Evaluation commits are many and specific 

![eval pull request](assets/images/feedback-commits.png)

---

### Highlights of learning process

@div[left-50]
<br>
@ol
- an efficient Git workflow facilitates fast responses to students
- GitHub Issues helps track needs 
- 
@olend
@divend

---?image=assets/images/git-branches.png&size=auto 90%

### Part III. How using Git promotes<br> collaboration and builds community

---?image=assets/images/turf-repo.png&size=auto 90%

### Collaborative repositories share web mapping solutions

---?image=assets/images/turf-voronoi.png&size=auto 90%

### Web mapping solutions accompanied by documentation

---?image=assets/images/student-pr-turf.png&size=auto 90%

### Students contributing back to wider community


---
## Some conclusions...

<br><i>Your mileage may vary.</i>

---?image=assets/images/computer.jpg&size=90% 90%

### Intentionality

---?image=assets/images/computer-fade.jpg&size=90% 90%

### Intentionality

@div[left-40]
<br><br>
![](assets/images/symap-errors.jpg)
@divend

@div[right-60]
<br>
@ol
- Then and now: educators must be intentional in choosing tools and platforms to support learning
- Then and now: students should be immersed in an environment where errors are opportunities for learning
- Then and now: there is always more to learn
@olend
@divend

---?image=assets/images/mcluhan.jpg&size=90% 90%

### The Medium is the Message

---?image=assets/images/mcluhan-fade.jpg&size=90% 90%

### The Medium is the Message

<br>
@div[right-40]
<br>
![](assets/images/course-question.png)
@divend

@div[left-60]
@ol
- No one will ever use course management systems after they leave the university
- <i>No one really wants to use these systems while IN the university</i>
- The systems of communication and feedback should mirror the systems used in the profession
@olend
@divend

## Conclusions
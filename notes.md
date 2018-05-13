# New maps in the new medium: <br> Teaching web cartography for a distributed workforce

<!-- TOC -->

- [New maps in the new medium: <br> Teaching web cartography for a distributed workforce](#new-maps-in-the-new-medium--br-teaching-web-cartography-for-a-distributed-workforce)
  - [Opener  (3 minutes)](#opener-3-minutes)
  - [Overview of New Maps Plus (4 minutes)](#overview-of-new-maps-plus-4-minutes)
  - [Using Git for course development and management (4 minutes)](#using-git-for-course-development-and-management-4-minutes)
    - [Highlights of benefits of using this Git process as a teacher:](#highlights-of-benefits-of-using-this-git-process-as-a-teacher)
  - [Using Git within the learning process (8 minutes)](#using-git-within-the-learning-process-8-minutes)
    - [Course content form and delivery](#course-content-form-and-delivery)
    - [Helping students](#helping-students)
    - [Assignment evaluation](#assignment-evaluation)
    - [Challenges?](#challenges)
  - [The role Git in collaboration and community building (6 minutes)](#the-role-git-in-collaboration-and-community-building-6-minutes)
  - [Conclusions and Discussion (2 minutes)](#conclusions-and-discussion-2-minutes)

<!-- /TOC -->

## Opener  (3 minutes)

Poetic gesture toward historical distance GIS education ... the hook.

## Overview of New Maps Plus (4 minutes)

* Rich Donohue and Matt Wilson teach geography and mapping at UK Geography
* Recently designed, built, and now instruct courses in a new program called New Maps Plus
* New Maps Plus: 
  * specifically focuses on web-based cartography and GIS using open source software
  * is applied and practical (with some more critical/historical elements) aimed at training web map developers
  * curriculum focuses on:
    1. applying traditional cartographic principles to web interfaces, drawing upon user-centered design, usability engineering UX/UI practices
    1. fundamental geospatial processing and data analysis tasks using QGIS, GDAL/OGR, Node.js (and other misc tools: Mapshaper, Simple Statistics)
    3. web design and development using HTML/CSS/JavaScript. Uniquely offers an introduction to programming aimed at non-Computer Scientists/Engineers, often entirely new to coding
* to date we've offered X courses over X terms, instructing 168 students, 56 who have graduated with a Graduate Certificate in Digital Mapping, and X more who are taking additional courses toward an eventual MS degree
* to quickly showcase some of the student work coming out of the program ... 
  * example
  * example
  * example
* the curriculum it's intended to support is technically demanding and challenging, particularly as students have little background in web design and coding: HIGHLIGHT that many students come in with little to no background in coding, command line, web development, using web technologies like Git
* beyond these challenging aspects, the courses are taught asynchronously and completely online to a geographically distributed student body: HIGHLIGHT distance learning aspect (refer back to intro Symap hook?)
* Question: how are we able to do this?
* Answer: Among the string of various technologies, libraries, and tools instruction, Git and its integration with GitHub has been instrumental in our evolution and success.
* Overview: talk will cover the following topics and address the strategies and recommendations we've learned along the way, as well as some enduring challenges
  * Using Git for course development and management
  * Using Git within the learning process
  * Reflections upon the role Git plays in a wider goal of collaboration and community building

## Using Git for course development and management (4 minutes)

* NMP course development started from scratch: terrific opportunity to experiment with new creative ways of doing things (also terrific opportunity to make mistakes)
* decision made to avoid proprietary formats for encoding information (Word, Google Docs, etc)
* instead, all material drafted in Markdown and hosted within private GitHub repositories
  * Markdown easily embeds images, animated GIFs
* **benefits:**
  * avoidance of emailing zips back and forth
  * tracking progress of content development
    * written explanations
    * scripted examples
    * resources/links
  * multiple authors can work synchronously or asynchronously
  * easy to share with other instructors with simple invite to repository (but ... segue to ...)
* **challenges:**
  * the Git learning curve is challenging (make crack at teaching old dogs new tricks and Profs having meltdowns with merge conflicts)
  * Git doesn't track binary formats such as Shapefiles (so not suitable for all GIS teaching needs)
  * Geo data can be large. need to be careful with pushing large files to GitHub repos and use alternative solutions 
* **recommendations:**
  * teacher training to include use of Git and GitHub
  * start with Git GUIs such as GitHub Desktop or SourceTree

### Highlights of benefits of using this Git process as a teacher:

* Teaching web cartography and web GIS is technically and time demanding; instructors need ways to maximize efficiency, and speeding up the transmission, management, and editing of student work (either help or evaluation) through command line and scripted Git processes serves this need.

## Using Git within the learning process (8 minutes)

* While we do use the traditional Canvas system for structuring learning modules and assignment deadlines, providing the GitHub Classroom links to lessons and assignments, and grade recording, Git and GitHub sits at the core of our learning process:
  * course content form and delivery
  * helping students
  * assignment evaluation

### Course content form and delivery

* First step of NMP curriculum is to establish a GitHub account and profile
* Lessons written in Markdown and hosted on GitHub (emulates documentation of industry standard for hosting code library repositories)
* Use of GitHub Classroom for deploying weekly lessons and assignments
  * Classroom allows use to use "starter templates" and provide students with URL invitation link
  * Classroom then automatically creates a copy of this starter template on our GitHub account with student's username
  * Bonus: enrollment in GitHub Classroom upgraded our account to have unlimited private repositories (advice to teachers: apply to GitHub classroom, but be mindful)
* Once student has accepted the assignment and the new individual repository is created:
  1. Students works on master branch (this is a debatable approach)
  2. Add/commits progress at local level and pushes up to remote repo periodically (the days of students losing a USB drive or their computer being eaten by their cat are over)
  3. Final submission is pushed up to repo

Questions about whether better to host student repos on our newmapsplus account vs the students account:

### Helping students

* When students need help:
  1. Student adds/commits any recent changes and pushes up to their repo. Then ping instructor via email or Slack chat.
  2. Instructor clones student repo to local (or pulls down recent changes)
  3. Instructor branches (e.g., `git checkout -b help-1`)
  4. Instructor examines/tests/edits code
  5. Pushes up branch for student to examine (or potentially merge with their master)
* Help can be accompanied by Slack chats or online screen sharing when necessary
* Highlight: an efficient Git workflow facilitates quick responses to students, allowing them to make it past a potential roadblock (and the instructor to continue updating the next module)

### Assignment evaluation

* Evaluation follows the same proceedure 
* Git used to help give concise feedback of written answers to quiz questions
* Git used to track editing of written prose as well, demonstrating the potential for the use of Git and Markdown in writing courses beyond a more technical curriculum

### Challenges?


## The role Git in collaboration and community building (6 minutes)

Beyond the benefits to course development, management, student gains, and teacher sanity, using Git helps facilitate greater collaboration within the classroom and, ultimately, with the broader community extending beyond our online learning environments. We can talk about these in terms of both the the workforce and the open source community (which we know are mutually intertwined).

Examples:

* MAP675 explicitly uses Git for pairing up students as course team members for assignments (facilitates async remote work between them while demanding a greater competency with branching, merging, etc.)
* NMP is also beginning to use shared GitHub repos to produce solutions to be shared among and beyond our students (e.g., the Turf examples repo)
* With student knowledge of Git, greater potential for them to work with and contribute back to the community (example of students doing Pull Requests on existing libraries)

## Conclusions and Discussion (2 minutes)


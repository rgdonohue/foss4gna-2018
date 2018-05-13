<!-- .slide: data-background-image="assets/images/dust_scratches.png" data-background-size="20% 20%" data-background-repeat="repeat" -->

# New maps in<br> the new medium

## Teaching web cartography<br> for a distributed workforce  
<br><br>
[Rich Donohue](https://twitter.com/rgdonohue)  
[Matthew W. Wilson](https://twitter.com/wilsonism)

---?image=assets/images/symap-assignment.png

### Assignment from SYMAP<br> correspondence course, ca. 1967

---?image=assets/images/symap-map.png

### Map produced from SYMAP, ca. 1967

---?image=assets/images/symap-coding-form.png

### SYMAP correspondence<br> coding form, ca. 1967

---?image=assets/images/nmp-website.png&size=auto

### [https://newmapsplus.uky.edu/](https://newmapsplus.uky.edu/)

Note:


---

### New Maps Plus learning objectives

<!-- .slide: data-background-image="assets/images/dust_scratches.png" data-background-size="20% 20%" data-background-repeat="repeat" -->

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

---?image=assets/images/tools.png&size=100% 90%

### Some of our favorite tools

---?image=assets/images/tools2.png&size=100% 90%

### What we're talking about today

---

### Where this talk is heading?

@div[left-60]
<br>
@ol
- How we use Git for course development and management
- How using Git improves the learning process
- How using Git promotes collaboration and builds community
@olend
@divend

@div[right-40]
![git tree](assets/images/git-tree.png)
@divend

---

## Part I. How we use Git for course development and management

---?image=assets/images/gitlogo.png&size=90% 90%

### But... what is a 'Git'?

@div
<br>
@ol
- Classrooms are composed of little learning events
- Students receive feedback on their ability to demonstrate learning
- In a distributed, asychronous classroom, Git provides a system for managing feedback, iteration, and documentation of learnin 
@olend
@divend

---?image=assets/images/markdownlogo.png&size=90% 90%

### And, wait... we also write in 'Markdown'?

---

### Node scripts used to automate course management tasks

```javascript
var markdownpdf = require("markdown-pdf"), 
    fs = require("fs")

fs.createReadStream("./syllabus.md")
    .pipe(markdownpdf({

    }))
.pipe(fs.createWriteStream("MAP_673_Syllabus.pdf"))

console.log('PDF syllabus written to file')
```

---

## Part II. How using Git improves the learning process


---

### Highly recommended! Use GitHub Classroom

![GitHub Classroom](assets/images/github-classroom.png)




---?image=assets/images/starter-template.png&size=auto 100%

### Starter template for each course module

<!-- ![starter template](assets/images/starter-template.png) -->


---

### Student repos created from starter template

<!-- .slide: data-background-image="assets/images/dust_scratches.png" data-background-size="20% 20%" data-background-repeat="repeat" -->

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

## Part III. How using Git promotes collaboration and builds community


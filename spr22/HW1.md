*This is the public posting of the assignment. See Blackboard for the invite link to make your submission in your own repository in the class organization*

# Homework 1: Course Setup and RCR

**Due:** Tuesday, January 18, 2022 by 11:59pm 
 
This assignment will cover the necessary steps to get set up for the semester and will have you complete training required for all ODU graduate students.  Read over the entire assignment before starting and make sure to read the information in the linked webpages.

*For this assignment only -- you may ask others in the class for help with these setup tasks.  Please use our Blackboard Discussion Board Q&A Forum for these questions so that others may benefit from the answers.*

## Reports

Each HW assignment this semester will require you to write an accompanying report. Unless specified otherwise, these reports must be written in Markdown.

### Formatting Reports

I've provided a template file ([`HW1-report.md`](HW1-report.md)) that can be edited for this assignment. (This will be the only assignment where a template will be provided. For future assignments, you'll need to create a new file for your report.) All reports must include your name, HW number, class, and due date.   

The questions appear in *italics*, and your answers should be in non-italic text.  (There is a section on Markdown formatting below.)

All reports must have a section labeled "References" for listing any outside resources you consulted.

### Submitting Reports

We will be using [GitHub Classroom](https://classroom.github.com/) for submitting HW assignments. Each HW assignment will have an invitation link available in Blackboard. When you accept the assignment, a new GitHub repository (repo) will be created for you.

Usually the new repo will only contain a README.md file with the assignment instructions. ***Do not edit this file, `README.md`.*** For some assignments, the repo may also contain data files needed to complete the assignment. 

Before you submit your assignment, view your report at GitHub.com to make sure that it is formatted properly and all needed files have been included in your repo.  Your GitHub repo should contain all scripts, code, output files, images, etc. needed to complete the assignment and your report.

Each assignment will have a [Submission](#submission) section with instructions on how to submit the assignment in Blackboard.  There are two steps to submission:
1. Include "Ready to grade @weiglemc" in your final GitHub commit message.
2. In Blackboard, submit the URL of your GitHub repo generated by GitHub Classroom.  I want an `https://` URL, not a `git://` URL or anything ending in `.git`. This should be something like   
https<nolink>://github.com/odu-cs800-research/spr22-hw1-*username*/ 

## Git, GitHub

Git is a version control system for tracking changes in source code, used in the popular [GitHub](https://github.com) code hosting platform.  To become familiar with the basics of Git, read [git - the simple guide](https://rogerdudler.github.io/git-guide/).

If you do not have one already, you must create a GitHub account.  I recommend a username that incorporates at least part of your actual name (e.g., mine is [weiglemc](https://github.com/weiglemc)). If you already have a GitHub account, you do *not* need to create a new one for this class.

***Q1.** What is your GitHub username?*

In this class, you should be able to do most work with GitHub through the web interface, but we will cover some of the command-line commands and other features during the semester as well.
 
## ODU-CS Linux

During this course and throughout your time in ODU-CS, you will need to use the [ODU-CS Linux systems](https://systems.cs.odu.edu/Unix_and_Linux_Services).  If you do not already have an account, request one at https://accounts.cs.odu.edu/grad. *This is different than your ODU MIDAS account.*
 
The [ODU-CS Systems Group](https://systems.cs.odu.edu/Main_Page) maintains ODU-CS computing services, including Windows desktops and Linux servers in the CS department.
 
***Q2:** How can you contact the Computer Science help desk?*

If you are not familiar with Unix/Linux systems, I strongly encourage you to read the materials from [CS 252 - Unix for Programmers](https://www.cs.odu.edu/~zeil/cs252/latest/Directory/outline/index.html).

Follow these steps to set up an initial webpage on the cs.odu.edu server and include the answers to the questions in your report:  *If you already have a webpage set up, you can skip the steps, but you must still answer the questions.*

1. Connect to the [CS VPN](https://systems.cs.odu.edu/VPN_Services).
 
2. Login to the ODU-CS Linux system using ssh, Putty, or an appropriate ssh client.
 
***Q3:** What hostname should you use to connect to the ODU-CS systems?*

3. Review the information about [Web Services](https://systems.cs.odu.edu/Web_Services) on the ODU-CS Systems wiki. 
 
***Q4:** In what directory will your webpages reside?*
 
4. Create the `~/secure_html` directory using `mkdir ~/secure_html`  
 
5. Create an initial home page in your `~/secure_html` directory named `index.html` using the following content (replace MYNAME with your name):

```{html}
<!DOCTYPE html>
<html xmlns="https://www.w3.org/1999/xhtml" lang="en">
<head>
<title>My Home Page</title>
<meta charset="UTF-8"/>
</head>
<body>
<h3>Welcome to MYNAME's home page!</h3>
</body>
</html>
```

6. Set the access permission for your website, so that the web server can access its contents, using  
`chmod -R o+rX ~/secure_html`

The `-R` flag on chmod will apply the command to all contents of the directory, i.e., your entire website. The `o+rX` option gives read and directory listing permissions (on directories only) to the "other" user set.  This command should be repeated for each new directory and file that you add to your website. It can be applied recursively at the top level (using `-R`), or it can be applied individually to each new item in the website.

7. Use a web browser to access your newly created webpage and take a screenshot.
 
***Q5:** What is the URL of your new webpage?*

## Markdown

Markdown is a lightweight markup language that is widely used in GitHub, especially for README pages.  Here are some useful guides:
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [GitHub's Basic Writing and Formatting Syntax guide](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)

In the HW1-report.md template that I've provided, there is a fenced code block.
 
***Q6.** Replace the code in the fenced code block with another block of code. You can use some Python code, or you can insert code from a different language -- just change the language indicated so that syntax highlighting still works properly.*
 
There is also a table in the report template.
 
***Q7.** Edit the table so that it matches the first 3 weeks of our class schedule, as given in our [syllabus](https://github.com/odu-cs800-research/public/blob/main/spr22/syllabus.md#summary-schedule).*
 
## LaTeX and Overleaf

LaTeX is *the* markup language for academic publication. [Overleaf](https://overleaf.com) provides an online setup for writing and compiling LaTeX into PDF.  

Sign up for a free [Overleaf](https://overleaf.com) account.

Walk through [part 1](https://www.overleaf.com/learn/latex/Free_online_introduction_to_LaTeX_(part_1)) of this [LaTeX introduction](https://www.overleaf.com/learn/latex/Free_online_introduction_to_LaTeX_(part_1)). In Overleaf, work the Typesetting Exercise 1 on slide 11.  Then click 'Share' and turn on Link Sharing.  
  
***Q8.** What is the link to view your newly created project? (Under "Anyone with this link can view this project")*

## Responsible Conduct of Research

All graduate students must complete the Responsible Conduct of Research (RCR) training before completing 12 credit hours of graduate work. Read the information at https://www.odu.edu/impact/responsible-conduct-of-training and follow the instructions to complete your RCR training.  The "Responsible Conduct of Research for Engineers" option is the most applicable for CS.

Once you have completed all the required modules, you will be able to print out and/or take a screenshot of a completion certificate on the "CITI RCR Course Completion Page".

If you have previously completed the RCR training at ODU, you should have an indication of this in [Degree Works](https://degree.odu.edu) under "Doctoral Milestones". Take a screenshot of the RCR requirement and checkmark.

Upload the image/screenshot of your certificate or a screenshot of the RCR completion in DegreeWorks to your GitHub repo.  
 
***Q9.** Include the image in your report in place of the "Growth of the Early Web" image. Make sure to change the description of the image in the report.*

## References

Every report should include a References section.
 
***Q10.** Replace the references with three webpages that you've visited so far this semester related to this class. These should include both the title of the webpage/article and the URL.*
 
## Submission

Your repo should include at least `README.md` (this file), `HW1-report.md`, and any image files you've included in your report.  Include "Ready to grade @weiglemc" in your final commit message.

Submit the URL of your repo in Blackboard:

* Click on HW1 under Assignments in Blackboard.
* Under "Assignment Submission", click the "Write Submission" button.
* Copy/paste the URL of your repo into the edit box
  * should be something like https<nolink>://github.com/odu-cs800-research/spr22-hw1-*username*/
* Make sure to "Submit" your assignment.

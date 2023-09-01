---
layout: project
type: project
image: img/TapisSquare.png
title: "Tapis File Checker"
date: 2023
published: true
labels:
  - Python
  - GitHub
summary: "A modular file checker designed to interact with servers using Tapis framework. It is intended to be run in a server workflow to ensure that scheduled automated uploads have occurred."
---

I created this program during my 2023 summer internship at UH Manoa working for Dr. Cleveland. The goal of this project is to create a file checking program utilizing the Tapis API that will check if scheduled research data has been uploaded and send a notification of any errors or missing files. As a starting point, I utilized a simple python script written by a former team member that accessed a Tapis server and listed all files. 

I modified the script so that it would check the server for all files listed in a template upload schedule. I added a name changer which used the system time and date to automatically modify the file name on the template, eliminating the need to pass a list of uploaded files every run. To account for changes in the file upload schedule, a link to a new template can be passed to the application. Next I created a messaging script, which used SMTP to email a list of any missing files or errors encountered. 

I changed all many variables to environmental variables that would be passed to the container when it is run. This allows server login details to be more secure. In addition it allowed other things like email addresses, subject lines, and servers to be changed without having to update the code. Finally I utilized Docker containerization for portability and scalability with easy integration with server workflows.

I learned quite a bit working on this project. It was my first experience with Docker and it showed me how powerful containerization can be. I ran into many problems with the SMTP email portion of the project, but my advisor Dr. Cleveland and other team members provided very helpful advice.


Source: <a href="[https://github.com/UH-CI/file-tester-tapis]"><i class="large github icon "></i>UH-CI/file-tester-tapis</a>

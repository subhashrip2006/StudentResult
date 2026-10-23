Student Result - Jenkins CI Practical

Files:
- StudentResult.java : sample Java program
- Jenkinsfile       : Jenkins Build and Test pipeline

Run locally in VS Code terminal:
    javac StudentResult.java
    java StudentResult

Expected output:
    Student Mark: 85
    Result: PASS

GitHub + Jenkins:
1. Upload StudentResult.java and Jenkinsfile to a GitHub repository.
2. In Jenkins, create a Pipeline job.
3. Set Definition to "Pipeline script from SCM".
4. Set SCM to Git and enter your GitHub repository URL.
5. Set Branch Specifier to */main.
6. Set Script Path to Jenkinsfile.
7. Save, then click Build Now.

Note:
This Jenkinsfile uses Windows commands (bat) and requires a Windows Jenkins agent
with Java JDK installed and javac available on PATH.

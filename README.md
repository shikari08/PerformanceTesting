## Project Description:
1. The Framework consists of one or more script that are defined as a test plan. 
2. A Test Plan can be viewed as a container for running tests. It defines what to test and how to go about it. 
A minimal test will consist of the Test Plan, a Thread Group and one or more Samplers, where a complete test plan consists of 
one or more elements such as thread groups, logic controllers, sample-generating controllers, listeners, timers, assertions, and configuration elements.

## How To run it ?

1. You’ll start by installing JMeter latest version, this project is using apache-JMeter-5.6.3.
2. You can download it from here https://jmeter.apache.org/download_jmeter.cgi
3. Go to the binaries section and download the Zip file.
4. You can open Jmeter in GUI/non-GUI mode.

**Opening JMeter in GUI mode:**

1. Once it's downloaded, go to the bin folder.
2. Open Jmeter file of type Windows Batch File, wait few seconds the JMeter IDE will be opened.
3. Click on file --> Open --> select the .jmx file that you need to run and it will be opened.
4. Click on the play green icon displayed in the header bar.
5. Navigate to "View result tree" to verify the results.


**Run the whole flow from local to Jenkins:**


1. Click on file --> New.
2. Right Click on Test plan -->Add --> Threads --> Thread Group.
3. Right click on Thread Group --> Add --> Sampler --> HTTP Request.
4. Give it a name (recommended to be related to the API name or scope).
5. Add value "https" to Protocol http field.
6. Add the Env variable in server name or IP field.
7. State the type of the request (get or post ..etc).
8. add the path of the API without the first common part of the env. (ex: \api\...etc).
9. Start add either a body or query parameters as shown in the demo video.
10. Right Click on Test plan --> Add --> Listner --> View Results tree and Summary report to verify the results.
11. Save the test plan file in any local folder on your machine.
12. Copy this file and paste it in the performanceTesting repo folder locally on your machine.
13. Navigate to sourcetree or through the terminal,and commit your changes to your branch (create a new one if you don't have) and push it to your remote branch.
14. Create a PR to merge to Jenkins2 branch (the main branch on Jenkins Job).
15. Merge the PR.
16. Add the file name to choices path placed in Jenkins file of Jenkins2 branch to be reflected on Jenkins Job.
17. Navigate to Jenkins Job click on Build now button.
18. When the job is paused, Click on run tests window and select the file you want to run.
19. Click on proceed button and wait the job to be finished so you can verify the results.



## Clone a repository

Use these steps to clone from SourceTree, our client for using the repository command-line free. 
Cloning allows you to work on your files locally. If you don't yet have SourceTree, [download and install first](https://www.sourcetreeapp.com/). 
If you prefer to clone from the command line, see [Clone a repository](https://confluence.atlassian.com/x/4whODQ).

1. You’ll see the clone button under the **Source** heading. Click that button.
2. Now click **Check out in SourceTree**. You may need to create a SourceTree account or log in.
3. When you see the **Clone New** dialog in SourceTree, update the destination path and name if you’d like to and then click **Clone**.
4. Open the directory you just created to see your repository’s files.


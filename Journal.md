First Time Commit
The first step was to create a repository and clone it to my work station. I used Github and Gitlab. Next, I created a LabVIEW Project and saved it to my repository, as well as included a main.vi for testing. In my project properties I set the compiled code to store in a separate cache and marked the main.vi.
![Image of LabVIEW VI](/images/VI.png)
 
Creating a Branch
Created a branch called FunctionalTest. In this branch I intended to implement a unit test for the main.vi that I can use in my integration. I created a VI called TestMain.vi the quickly tests the add function in main.vi
![Image of LabVIEW VI for UnitTest](/images/UnitTest.png)
 
Merging the Branch
I went to the Github page for the repository and selected “Branches” tab. In this tab I found the feature branch I created and saved. I selected, “New Pull Request” and selected that I wanted to pull FunctionalTest.
This brought me to the forum page where I was able to comment and tag people to comment before I requested the pull. I submitted the request.
Next, the pull request forum page came up. Since I am the admin I see this:
![Merge Pull Request Admin Screen](/images/MergePullRequest.png)
 
I can click the Merge pull request to pull the feature into the main branch. Several apps are available links to this: https://github.com/marketplace/category/continuous-integration
I merged the pull request. There were some problems with that, do I am trying again. I’m not certain what went wrong.
Researching Integration
This looks like a good guide:
https://resources.github.com/whitepapers/practical-guide-to-CI-with-Jenkins-and-GitHub/



Had to install Git on the VM containing Jenkins and use this page to https://stackoverflow.com/questions/8639501/jenkins-could-not-run-git point to git.exe (java.io.IOException: Cannot run program "git.exe" (in directory "C:\Users\OpalRTDev\.jenkins\workspace\JenkinsExample_master"): CreateProcess error=2, The system cannot find the file specified
)

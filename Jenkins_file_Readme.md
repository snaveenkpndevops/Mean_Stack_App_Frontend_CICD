1. Create a Jenkins pipeline Project.
2. In Manage plugins --> Install `Generic Webhook Trigger` plugin
3. Read this Document for Github Webhook Configuration -->  `https://www.geeksforgeeks.org/what-is-webhooks-in-jenkins/` (or) `https://medium.com/@sangeetv09/how-to-configure-webhook-in-github-and-jenkins-for-automatic-trigger-with-cicd-pipeline-34133e9de0ea`

4. Install ngrok in your local machine.  --> Because to trigger localhost:8080 from github it needs some addditional configuration. 
5. Ngrok Installation Commands:

    * Open ngrok official website --> sign in and open the commands and run it in powershell terminal (Admin mode)
      --> 

### Images:

![Jenkins Logo](./images/jenkins_image/ngrok%20installation.png)

![Jenkins Logo](./images/jenkins_image/ngrok%20installation1.png)


6. copy the ngrok url and paste that url along with "//github-webook/" in github webhook settings.

### Images:

![Jenkins Logo](./images/jenkins_image/Github%20webhook%20config.png)

![Jenkins Logo](./images/jenkins_image/Github%20webhook%20config4.png)

![Jenkins Logo](./images/jenkins_image/Github%20webhook%20config5.png)

7. Jenkins Pipeline Configuration:

  * Configure Github and Docker Credentials in Manage Jenkins under credential manager.

  ### Images:

  ![Jenkins Logo](./images/jenkins_image/Dockerhub%20credentials%20jenkins.png)

  ![Jenkins Logo](./images/jenkins_image/Github%20credentials%20jenkins.png)

  * Configure Global Variable in Manage Jenkins Under Settings.

  ### Images:

  ![Jenkins Logo](./images/jenkins_image/Global%20Variable%20jenkins.png)

  * Pipeline Configuration.

  ### Images:

  ![Jenkins Logo](./images/jenkins_image/pipeline1.png)

  ![Jenkins Logo](./images/jenkins_image/pipeline2.png)

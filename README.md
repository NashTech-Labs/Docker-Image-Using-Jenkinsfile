**Build and Push a Docker Image using JenkinsFile**

## Why do we need Jenkins-Pipeline?

You can reuse everything you’ve done and paste your Jenkins code into your git project. Changes to the pipeline appear in Job History Changes.

Now one should have a seperate directory and under that directory create one file 

Now, let’s create a sample python app :

```
app.py
```
you can run the python app using the command:

```
python3 app.py
```
Now, create a dockerfile to dockerize the project

Once you have the Jenkinsfile created, create a Github repo and push the entire project to the repo.

Now you can start working on Jenkins and building your project. It is assume that the Jenkins server is already install and running. First, let’s add Dockerhub credentials to Jenkins. These credentials are used to log in to Dockerhub. Click Manage Jenkins, then click Manage Credentials.

Click global, then Add Credentials to add a new credential with a Global Scope.

Add your Dockerhub username and password. The ID is used in the Jenkinsfile and stores the credentials. You can see this used in the Jenkinsfile.

Now the pipeline is ready to be created. Go back to the dashboard and select New Item. Now, Enter a name for the new item, select Pipeline, and click OK.

Enter a Display Name for the pipeline.

Under Pipeline leave the default Jenkinsfile because this will look for the Jenkinsfile in the cloned repo.

That’s it, click save and the project should begin running immediately.
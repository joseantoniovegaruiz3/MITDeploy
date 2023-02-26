Deploy Your Application (60:00)
Due Tuesday by 9:29am Points 1 Submitting a file upload Available Feb 20 at 5pm - May 23 at 9:29am
 Module 22: Introduction And Instructions (5:00) (Completed)
 Video 22.1 (0:49): Working With The Three Tiers (Completed)
 Video 22.2 (8:25): Initialize Data Store (Completed)
 Initialize The Server (60:00) (Completed)
 Knowledge Check 22.1: What Is Middleware? (30:00) (Completed)
 Video 22.3 (5:28): HTTP POST (Completed)
 Body Parser (5:00) (Completed)
 Knowledge Check 22.2: Identify Middleware (30:00) (Completed)
 Video 22.4 (4:55): Add Bootstrap Navigation And Serve Static Files (Completed)
 Video 22.5 (8:38): Generate User Data With Faker (Completed)
 Video 22.6 (6:20): Read And Display Faker Data (Completed)
 Common Development Tools And Packages (30:00) - Section B (Completed)
 What Is DigitalOcean? (5:00) (Completed)
 Things To Consider When Selecting A Cloud Service Provider (5:00) (Completed)
 What Is Heroku? (2:00) (Completed)
 Video 22.7 (12:29): Set Up A Virtual Machine With DigitalOcean (Completed)
 What is Cross Origin Resource Sharing (CORS)? (5:00) (Completed)
 Video 22.8 (8:53): Move App To The Cloud (Completed)
  Deploy Your Application (60:00) ((Must submit the Assignment))
 Test Your Deployed App With Postman (90:00) ((Must submit the Assignment))
 Common Deployment Issues (30:00) - Section B ((Not yet completed))
 Q & A Discussion With Learning Facilitators (30:00) - Section B ((Not yet completed))
 Module 22: Additional Resources (Completed)
 Module 22: Feedback Survey (5:00) ((Must submit the Quiz))
module outcomes.pngLearning Outcome Addressed
 4. Deploy an application to the cloud

You may use a cloud-computing service of your choice to practice deployment. Below, you will see instructions for DigitalOcean and Heroku. 

DigitalOcean
DigitalOcean Droplets are virtual machines you can use to host your applications. Each droplet is a server that you can manage through the DigitalOcean platform.

Your task in this activity is as follows:

Create a DigitalOcean account.
Create a Droplet.
Connect to your newly created droplet using SSH. You can refer to the official DigitalOcean documentation Links to an external site.for more information.
Open port 3001 within the droplet.
Create a new application by making a folder at the root level and running npm init inside that folder.
Heroku
If you are using Heroku, use the starter code.Links to an external site.  You will need to make a few adjustments to your application code, as follows:

Within your app’s “package.json” file, add the following scripts (this should be added under the “scripts” tag):

    "build": "npm install",

    "start": "node http_server.js",
Specify the node version in the package.json file by adding the following tag:
"engines": {

    "node": "14.x"

  },
Add the following lines to your .gitignore file to keep application artifacts out of GitHub: 

/node_modules

npm-debug.log

.DS_Store

/*.env
Note that the starter code for Heroku includes some small changes to allow it to work in both local and deployed environments. It will start the application on the port specified by the process.env.PORT which will be dynamically assigned by Heroku. If running locally, it will use port 3000. 
Commit your code changes to your GitHub repo.
Next, go to HerokuLinks to an external site. and create an account or log in to your existing one:

Select New and then Create New App on the Heroku dashboard.
Go to the Deploy tab and select GitHub, which can be found under Deployment Method.
Follow the instructions on the page to connect your GitHub repo.
Use the Deploy Branch feature to deploy your app.
Select Open App at the top-right corner of the page to access your app.
Submission Instructions:

After you verify that your application is up and running, upload a screenshot showing the IP address and your application running in a browser.

Note: You can refer to the following resources while working on this task:

What Is Heroku?
Set Up A Virtual Machine With DigitalOcean
Move App To The Cloud 

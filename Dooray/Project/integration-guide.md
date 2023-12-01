## Dooray! > Project > Link Service Guide 

### Link Service 

Dooray! provides outgoing web hooks which notify Dooray! project events to other external services to work with them and incoming hooks which allow linking various external services with Dooray! Incoming linking is a method of linking frequently used tools, such as development, distribution, source management and performance management tools, to Dooray! in order to store various changes from external services to Dooray! projects or Dooray! messenger chatrooms. Dooray! supports incoming linking with Jenkins, GitHub, Gitlab, Trello, NewRelic, JIRA, Bitbucket, IFTTT, Grafana, and Dooray! 

For incoming hook, go to Dooray! Setting > Link Service > Add Service and select the services to link. This means that you will receive the notifications and events from the services via Dooray! and the linking URL should be added on WebHook Settings of each service. The following shows how to register the push events from the GitHub project to the Dooray! project.   
#### Linking with GitHub 

Dooray! Go to Settings > Link Service > Add Service > GitHub and click the ‘Add Link’ button. Select the Dooray! service to link with when a GitHub event is triggered. Select one of the Dooray! projects to receive the Git event as a selected project comment. When you select a linked chatroom, the event will be received as a message in the chatroom.  

Name the Bot, copy the linking URL to the clipboard, check the project box to connect, and then click the Save button. 

![Link](http://static.toastoven.net/prod_dooray_project/01_project_integration.png)
<center>[Figure 1]Setting Dooray! Service Link Settings</center>

After copying the Bot linking URL, webhook this to the service to link. Go to the Settings page of Github. Click the Webhooks & Services menu to add the webhook.  

![Link](http://static.toastoven.net/prod_dooray_project/02_project_integration.png)
<center>[Figure 2]Github Settings</center>

Type the copied Dooray hook linking URL to the payload URL, and click the Save button. 

![Link](http://static.toastoven.net/prod_dooray_project/03_project_integration.png)
<center>[Figure 3]Adding Web Hook</center>

If the commit message includes "fix #my-dooray-project/1234" text when pushing commit to Github, the push notification is added as a comment to #my-dooray-project/1234. If it is merged due to a pull request, the task is automatically completed with a notification comment.

#### Linking to GitLab 

Dooray! Go to Settings > Link Service > Add Service > GitLab and click the ‘Add Link’ button. Select the Dooray! service to link with when a GitLab event is triggered. 

![Link](http://static.toastoven.net/prod_dooray_project/043_project_integration.png)
<center>[Figure 4]Dooray! Service Link Settings</center>

Paste the copied Dooray hook linking URL in the GitLab Settings > Integration page and select Trigger. For Trigger, the blue items checked below are linked. Select triggers to link and click the Add webhook button. 

![Link](http://static.toastoven.net/prod_dooray_project/05_project_integration.png)
<center>[Figure 5]Adding Web Hook</center>

If you enter the text "fix#my-dooray-project/1234" in the message when pushing commit, a push notification is added as a comment to #1234 task of my-dooray-project. If it is merged due to a pull request, the task is automatically completed with a notification comment. 

During commit, if you use the following words, auto writing of comment and process completion are activated. 
- fix, fixes, fixed
- close, closes, closed
- resolve, resolves, resolved
- Resolved, Completed 




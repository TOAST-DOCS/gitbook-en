## Dooray! > Project > Service Detailed Guide  

## Create a Project

### Create a Private Project

Private project is the most general type of project, which can be read and written by invited members only. If a person is listed as an owner or a CC or mentioned for a task, the person can read and write for that specific task even if he or she is not invited. Click the [+] icon next to 'My Project' to add a project. When adding a project, set the persons to show the project to Project Members Only.

![Add a Project](http://static.toastoven.net/prod_dooray_project/detail/01_pjt_detail_addpjt.png  )
<center>[Figure 1] [+]</center> Next to My Project

![Members](http://static.toastoven.net/prod_dooray_project/detail/02_pjt_detail_member.png)
<center>[Figure 2]Add a Project &gt; Project Members Only</center>                                                                               
#### Organization
- Determine the organization where the project to create will belong when a member belongs to several organizations. If the project belongs to Organization A, the member can collaborate with the members of Organization B.
- However, the member is managed by the manager of Organization A. If the member belongs to only one organization, this "Organization" item is not shown.

#### Project Name
- Project Name is used to indicate the work included in the project. For example, if the project name is 'Shopping mall improvement', the #56 work of the project is displayed as ‘Shopping mall improvement/56’.

#### Description
- Write the contents freely by using markdown or WYSIWYG. From a short message to a long paragraph with images, you can freely write just about anything.

#### Open to
-  The default value is ‘Project Members Only’. This is a private project that only members invited to the project can read and write. If you want all tenant members to read and write freely, change this setting to 'All Members in Organization'. This project with this permission is called 'Open Project'.


### Create an Open Project

In general, most projects are run in private mode. However, open project can be more convenient for a startup with a small number of employees and for a specific purpose such as sharing.
All tenant users can read and write in an open project even if they are not members of the project.

> For example, open project can be a replacement of a board, such as 'Notice' or 'Sharing Technology'. If you have set a project as private rather than open, you should add a new member to 'Notice' or 'Sharing Technology' project whenever a new member signs up.

When one tenant has several organizations, you can also disclose the project to a specific organization. Choose ‘All Members in Organization' and then the 'Choose Organization' option appears next. Click this to view the list of all organizations of the tenant. You can select an organization for the project.
 

The open project is open to all organizations of the tenant; however, the tenant guests cannot access the project. Any tenant guest must be a member of the open project or an owner or a CC of the open project to access the project.

### Create a Write-only Open Project 

Write-only Open Project is an open project, but only the issues you have written can be available if you are not the project member. It means you can create an open project to allow non-project members to register tasks. However, if you want to restrict the non-project members from viewing tasks registered by others, an open project will not work. 
> For example, patent review and legal review can be very sensitive. In these cases, Write-only Open Project can be a convenient solution.

#### Open For

- The default value is ‘All’. In this case, a tenant member can read posts written by not only himself or herself but also others. However,
 if the setting is changed to ‘Write Only', non-project members can read and write the work registered by them only.

> If your organization have any internal services to review patent or report sexual harassment, you can create a projected project for that. A large service can be replaced with a small feature of Dooray!
Project.

 

## Project Settings for Project Manager

Dooray! Project allows for assigning more than one manager to a project. Difference in permissions between a project manager and a member is nearly negligible. However, only a project manager can touch 'Default Settings' and 'Web Hook' as these settings can have significant effect when settings are changed.

### Default Settings

#### Status
- When the project status is changed to 'Close', any new work cannot be registered and no comment can be added.

#### Project Calendar
-  Set this to ‘Enable' to view the work of the project by completion date on Dooray! Calendar.

#### Project Mail
-  Set this to ‘Enable' to give an email address to the project. When an email is sent to the address, the email is registered as a work to the project.

#### Project Drive  
-  Set this to ‘Enable' to create the drive for the project in Dooray! Drive and members can share and manage files together.


### Webhook

Dooray! supports the Outgoing Webhook function. Dooray! When a work or comment is registered to the Dooray! Project or a work is changed, the URL with the changed status is sent to users. Since this function allows sending the project contents to any external services, an Outgoing Webhook can only be set by a project manager due the security risk. This can be set via the [Webhook] menu under the Project Setting. On the following Add Webhook screen, the supported message formats for outgoing Dooray! events are Dooray! and Slack formats. On this screen, you can register a Webhook URL to receive notifications.

#### Webhook URL

- Send a task or comments registered to a task to the destination of the Webhook URL entered.

#### Outgoing Message Formats

- Currently, Dooray! and Slack formats are supported.

####  Select Alert Event

-  Select the alert events you want to receive.

####  Enable or Disable

-  To stop using a Webhook for a while, do not uninstall it but click ‘Edit’ on the Webhook list you are using and set it to ‘Disabled’.
  
![Project Setting](http://static.toastoven.net/prod_dooray_project/detail/07_pjt_detail_add_webhook.png)
<center>[Figure 7]Adding Webhook Screen</center>   

#### Log 

-  To view the history of the registered Webhook, click the ‘Log’ button of the Webhook.

## Register Task

### Register a task without a project

Unlike common issue trackers or project management tools, Dooray! allows you to register and manage a short task without a project. Click the 'New Task' button. Select ‘(None)’. Enter the title and the owner to register. For now, there is no function to collect and show tasks registered as ‘(None)’; however, you can lookup the tasks in the Sent Task Box.

### Quick Write

Sometimes you need to register a task which has only a title but its owner, body and completion date have not been filled in yet. Although you can register tasks through the steps described earlier, there is an easier and faster way to do this. Click the [+] icon next to the project name. You can see a very simple Write window instead of a large one.

![Quick Write Window]( http://static.toastoven.net/prod_dooray_project/detail/08_pjt_detail_w.png)
<center>[Figure 8]Quick Write Window </center>   

In this layer popup, the first line is for the title and the next lines are for the body. To enter a title only, fill in the first line only and then click the 'Register' button. To register more tasks in a consecutive way, click ‘Save and Keep Registering’. You can do this faster by using the shortcut key. On the task list screen, type 'fw' for shortcut. A Quick Write window appears. Type the title and press \[Ctrl\]+\[Enter\] (for macOS, \[Cmd\]+\[Enter\]). It works in the same way as clicking ‘Save and Keep Registering’. To also assign the owner at this time, add ‘-&gt;@Hong_Gildong’ to the title.

### Register Mail as Task

Dooray! Dooray! Mail can be registered as a task. This has been described in Mail Service in detail. Sometimes you may need to register a mail body as a task while communicating via email with external parties. In this case, there is no need to copy and register the body as a task of the Dooray! Project. Just click the \[…\] menu on the Read Mail screen and select the 'Register as Task' menu.

### Register Sub Task

It is a efficient way to bind related task as a sub-task. Dooray! Project provides two ways of registering a sub-task. You can register an existing task as a sub-task or register a new task as a sub-task.

#### Register an existing task as a sub-task

- Search for a title and specify a task as sub-task.
- It is not available to specify all tasks as sub-task. As a sub-task of a sub-task is not supported, a task which already has a sub-task cannot be specified as a sub-task. 

![Add Sub-Task](http://static.toastoven.net/prod_dooray_project/detail/09_pjt_detail_addtask.png)
<center>[Figure 9]Add Main/Sub-Task</center>   

#### Register a new task as a sub-task

-  For the task (Main Task) to which a sub-task will be added, select ‘Add/New Sub-Task’. 
- Please note the following regarding relationship between main and sub-tasks. Even if all sub-tasks have been 'completed', the main task is not automatically 'completed'. Even if not all sub-tasks have been 'completed', the main task can be 'completed'.

### Collaborate with External Users

To collaborate with external users via Dooray! Project, you don't have to add the external users as your members but can still work together. 

#### Add external emails to Owner and CC 

- Add external email addresses (e.g. .gmail.com) to send the body of the task to the external users as an external email. When the users of the external emails reply, the replied messages are registered as comments; thus, the task history can be managed in one task. 
- <Span style="color:#FF0000">※ Note: At this time, the task body sent to the external email cannot be edited. </span>

![Add External Email](http://static.toastoven.net/prod_dooray_project/detail/pjt_detail_external_mail.png)
<center>[Figure ]Add External Email</center>  

#### Send the comment as external emails 

- If you have something to inform to external users while communicating with members via comments, you can directly send them your comments in an email. 
- <Span style="color:#FF0000">※ Note: When sending a comment via email, the comment is marked in a different way from other comments and it cannot be edited, like the task body, as it has been sent as an email.</span>

If you have an external mail in To or CC, you can send the mail by clicking the arrow to the right of the Save Comments button.
![Send Comment as Email](http://static.toastoven.net/prod_dooray_project/detail/pjt_detail_external_mail02.png)
<center>[Figure]Select the Sender's Name and Send Email</center>  

- [Caution] If there is no external mail in To or CC, the arrow does not appear because you cannot send mail.
![save comment](http://static.toastoven.net/prod_dooray_project/detail/pjt_detail_save.png)
<center>[Figure] Save comment button if no external mail is available</center> 

![Comment Sent as Email](http://static.toastoven.net/prod_dooray_project/detail/pjt_detail_external_mail021.png)
<center>[Figure]Comment Sent as Email</center>  

#### Set the Sender's Name 

- If you need to change the sender's name when sending a comment as an external mail, go to Project Setting> Task > Link Mail and set the sender's name. After that, you can select the sender's name when sending a comment as an email.
 
![Set the Sender's Name](http://static.toastoven.net/prod_dooray_project/detail/pjt_detail_external_mail04.png)
<center>[Figure] Set the Sender's Name</center>  

### Specify Multiple Owners

It is recommended to make the responsibility of a task clear by assigning only one owner for any one task. However, sometimes several persons have to do one task. With the existing tools, It's a quite cumbersome to register a task to a person one by one. Dooray! Project allows you to assign several members as owners just like Email does. In addition, it allows you to manage workflow for each person listed in the owner field.

#### Check the progress of owners and CCs 

- When several persons are assigned as owners, it is possible to figure out the progress status by looking at the color of each owner's name.
  Registered: black, In progress: blue, Completed: gray.

![Owner Status](http://static.toastoven.net/prod_dooray_project/detail/10_pjt_detail_add_npeople.png)
<center>[Figure 10]Specify Multiple Owners and CCs</center>   

#### Change Owners and CCs 

- While writing comments you may need to change the owners and CCs.
  When typing in -&gt;@Hong_gildong and entering the comment, 'Hong_gildong' is assigned as the owner of the task and the existing owner is replaced as a CC. Type in "-&gt;&gt;@Hong_gildong
  in the comment..." and 'Hong_gildong' is added as another owner of the task.
- Persons who are not project members can also be assigned as owners or CCs. In this case, the persons have read/write permissions only for the task.

## Format of Body and Comment

### Create a Markdown

 See the Markdown help at https://nhnent.dooray.com/htmls/guides/markdown\_ko\_KR.html. 
 You can try writing right on this page. The left screen is the Markdown Editor and the right screen is the result screen.

### Task Reference

You can insert a link of another task in the body or comment. You can copy and paste the browser URL from another task read screen to the body (or comment); however, it makes the link invalid if the task has been moved to another project. In the editor, enter ‘\[‘ and then select ‘Task Reference’. The list of recently viewed tasks is displayed. Select a task to insert using the arrow keys or the mouse. If there is no task you want to insert, you can search for a title by entering its keyword.

![Reference]( http://static.toastoven.net/prod_dooray_project/detail/11_pjt_detail_ref_task.png)
<center>[Figure 11]Input in the [Editor</center>   

![Reference 2](http://static.toastoven.net/prod_dooray_project/detail/12_pjt_detail_ref_task_select.png)
<center>[Figure 12]Select a Task to Refer</center>   

### Mention

Type ‘@’ and enter a person's name or a member group to call for a specific person or member group. This function is called mention. When a user is mentioned, a notification is sent to the user regardless of the user's setting. In addition, the user is added to the CC of the mentioned task and has the read/write permission for the task. Depending on who is mentioned (Member, You, or Guest), a different color is used to visually express the target. The default color of mention is light blue. When you are mentioned, it is displayed in dark blue to show clearly that I am mentioned. If a guest is mentioned, it is displayed in light black to express that the guest is not an official member of the tenant.

![Mention](http://static.toastoven.net/prod_dooray_project/detail/13_pjt_detail_mention.png)
<center>[Figure 13]Three Cases of Mention</center>   

## Project Settings for Project Member

### Member

You can invite members and manage member groups.

#### Member Group

-  Click the ‘Add Group' button.

![Member Group](http://static.toastoven.net/prod_dooray_project/detail/14_pjt_detail_add_group.png)
<center>[Figure 14]Project Setting &gt; Member &gt; Add Group</center>   

- Enter the group name, choose the members for the group, and click the ‘Create’ button.
- All projects has a member group ‘/all’, which refers to all project members.
- One project has several persons with various jobs. It is easier to collaborate with them when you create a member group per job. 

> For example, once you have created a member group of ‘Shopping mall improvement/Design’, you don't need to remember every designer's name when allocating the tasks to the design part. Enter 
> ‘/Design’ in the owner field and you can select ‘Shopping mall improvement/Design’ from the AutoComplete list easily.
> Like this, creating various member groups by job in a project allows you to find the owner exactly when discussing tasks between projects. In most cases, project names are known. So typing the project name in the owner field will reveal and display the member groups of the project. It is easy to find and select ‘/Design’ from the list.
> It used to be hard to find designers of relevant projects, but Dooray! Project makes it much easier by providing this member group function. It is more efficient to collaborate if the tenant administrator provides a guide of member group naming convention.

### Milestone

You may specify the completion date by task to set the target date of the task. Even if you have specified individual completion date, you may need to manage the task based on the release date when a product and service is released on a specific date. Milestone helps you in this case. Click the ‘Add Milestone' button to add a milestone. And then you can filter milestones with the added milestone and view a specific one from the task list.

![Milestone](http://static.toastoven.net/prod_dooray_project/detail/15_pjt_detail_add_milestone.png)
 <center>[Figure 15]Project Setting >  Add Milestone</center>   
![Milestone](http://static.toastoven.net/prod_dooray_project/detail/16_pjt_detail_milestone_filtering.png)
 <center>[Figure 16]Project Setting >  Filter Milestone</center>   

#### Milestone name

- A milestone name.

#### Period

- You can specify the period or not. If you specify a period, a burndown chart is created in the Dashboard during the period.

### Tag

This is used for classifying tasks. Click the ‘Add Tag' button to add a tag.

 ![Tag](http://static.toastoven.net/prod_dooray_project/detail/17_pjt_detail_tag.png)
 <center>[Figure 17]Project Setting > Tag</center>  

#### Tag name

- Input  “:” in the tag name, such as “Type:Issue”, the word before “:” is recognized as a group to group tags.
- When a tag group is created, you can specify tag name as a required value, or make it mandatory to select only one group from multiple groups. It is useful when a formulaic input is used.

![Tag group](http://static.toastoven.net/prod_dooray_project/detail/18_pjt_detail_tag_group.png)
<center>[Figure 18]Set a Tag Group</center>  

### Template

Template helps you to predetermine owners, CCs, title, body, tag, milestones, and priorities. It allows you to register tasks in an easier and faster way when registering tasks repeatedly. 

#### Use of Template

- There are two ways to register tasks by using a template. To register a task, you can open a Write window and then select 'Template'. Or you can click a desired template link from the template list in the Project Dashboard. 
- In addition, you can forward the link to another services (e.g., Mail, Wiki) for easier registration of the task.

> For a Human Resource (HR) project, you can create a template such as holiday application and purchase request. For an ITSM (IT Service Management) project, you can create templates such as equipment application and network ACL request. Template is the feature most widely used in Dooray! Project.

![Template](http://static.toastoven.net/prod_dooray_project/detail/19_pjt_detail_template.png  )
<center>[Figure 19]Select a Template in the Write Window</center> 

![Template](http://static.toastoven.net/prod_dooray_project/detail/20_pjt_detail_template_list.png )
<center>[Figure 20]Project Dashboard > Template List </center>   
                                             
####  Default Template

- With a given template from the project, you can quickly use a set of values to a certain extent. However, if a user who registers a task does not select any template, others might not be able to get the necessary data, resulting in a cumbersome process of leaving comments to ask and answer questions. To reduce this cumbersome process, Dooray! Project provides the 'Default Template' function.
- To set the template, go to Project Setting &gt;, select the Template tab, and &gt; click Add Template to open the Set Template screen.

![Template](http://static.toastoven.net/prod_dooray_project/detail/21_pjt_detail_setting_add_template.png)
<center>[Figure 21]Project Setting > Template </center>   
 
- When setting a template, check the ‘Default Template' box. Then the template is automatically applied when the Write window opens in the project.
  
![Default Template](http://static.toastoven.net/prod_dooray_project/detail/22_pjt_detail_default_template.png)
<center>[Figure 22]Set Default Template</center>   

#### Macro 

- Use the following macros while creating a template. Macro allows you to display data automatically.
> If today's date is 2018/03/29, use the following macro. Then, the macro will be automatically converted into the corresponding data.
> ${year} Displays the year (e.g. 2018). 
> ${month} Displays the month (e.g. 3).
> ${today} Displays in yyyy/mm/dd format (e.g. 2018/03/29).
> ${day} Displays the date (e.g. 29).
> ${month2} Displays the month in a different format (e.g. 3). 
> ${weekNum2} Displays the "n"th week. March 29, 2018 is the 5th week of the month.(e.g. 5). 

- When the department set in the profile is Dooray Planning, the macro will be automatically converted into the corresponding data.
> ${department} Displays the department (e.g. Dooray Planning). 

#### Example of Template

- An example of template is given as follows. As shown in the following figure, add and use templates.
- Add the items which are always used in the meeting minutes in the template and you can load and use the document of the same format more easily. Use the ${today} macro to include today's date in the meeting minutes automatically.  

![Example of Template](http://static.toastoven.net/prod_dooray_project/detail/22-1_pjt_detail_template1.png)
<center>[Figure 22-1] Meeting Minutes Template</center>   

- Create a weekly meeting template as specified in the following description. You don't need to waste time preparing for a meeting and summarizing the meeting minutes. 

![Example of Template](http://static.toastoven.net/prod_dooray_project/detail/22-2_pjt_detail_template2.png)
<center>[Figure 22-2] Weekly Meeting Template</center>   

- Service QA Items template is used for creating a checklist in the body to test key features of the service. 

![Example of Template](http://static.toastoven.net/prod_dooray_project/detail/22-3_pjt_detail_template3.png)
<center>[Figure 22-3] Service QA Items Template</center> 

- It is useful to create Bug Registration templates by service. You can specify the owner or group of each service easily. Also, you will miss nothing if you gather all information that must be known to be able to verify bugs in the body. Especially, it is very convenient if you create a tag group along with the attributes of the group (required; select only one).

![Example of Template](http://static.toastoven.net/prod_dooray_project/detail/22-4_pjt_detail_template4.png)
<center>[Figure 22-4] Bug Registration Template</center> 

### Shared Link

Use this to share a task with users who are not in the same tenant. To prevent others from sharing the task registered by you, only you who registered the task or your project manager can share the task. Select ‘Share Additional Task &gt;’. Click 'Add Link'.

![Share]( http://static.toastoven.net/prod_dooray_project/detail/23_pjt_detail_share_task.png)
<center>[Figure 23]Share</center>   

#### Share Period

- Share the task until the specified date. After the period, the link is not valid.

#### Share Range

- Set whether to share the attachments or not.

 ![Share Setting](http://static.toastoven.net/prod_dooray_project/detail/24_pjt_detail_share_setting.png)
 <center>[Figure 24]Share Setting</center>   

When a specific task is shared, Shared is marked at the top of the task. The project manager can view the shared tasks within the project from ‘Project Setting &gt; Shared Link’ at once. The organization administrator can also view the list of all shared tasks within the organization from 'Shared Link' under &gt; Manage Organization &gt; Service Settings on the left side of the screen. 

![Shared Task](http://static.toastoven.net/prod_dooray_project/detail/25_pjt_detail_share_task_list.png)
<center>[Figure 25]List of Shared Tasks </center>   

## Task Status

### Change the Status

Tasks status is either ‘Registered’, ‘In Progress’, or ‘Completed’. A member or guest listed as an owner can click the 'Proceed' button to change the status to 'In Progress'. When it is changed to ‘In Progress’, the 'Proceed' button is changed to the 'Complete' button. Click the ‘Complete' button to change the status to 'Completed'. Whenever the status is changed, the color of owner is changed. The name colors of the task statuses ‘Registered’, 'In Progress', and 'Completed' are black, blue, and gray, respectively.  Therefore, you can view the status of each owner easily even if several persons are specified as owners.

### Distinguish the task status from the owner status

There is one thing you have to know. Dooray! Unlike other issue trackers, Dooray! Project allows you to manage not only task status but also status for each task owner.
When there is only one task owner, the owner status and the task status are identical. However, if there is more than one owner, the statuses may not be the same.

> For example, if there are Owners A and B for Task #56, the task statuses and statuses of both Owners A and B are
> ‘Registered’. However, when the Owner A changes the status to ‘In Progress’, the status of Owner A is 'In Progress' but the status of Owner B is still 'Registered'. And the status of Task #56 is changed to ‘In>  Progress’. This is because one of the owners has made a progress. Even if the Owner A changes the status to ‘Completed’, the status of #56 is still 'In Progress’. This is because the Owner B has not completed his part yet. When the status of Owner B is changed to ‘Completed’ and the status of all owners is changed to ‘Completed’, the status of Task #56 is finally changed to 'Completed'.

When all owners are in ‘Registered’ status, the task status is 'Registered'. When all owners are in ‘Completed’ status, the task status is 'Completed'. Other task status is 'In Progress'.

### Change/Revert the Owner Status

In some cases, you might know that a task has been completed even if you are not the owner of the task. Then, you can ask the owner to change the task status to 'Complete' via Mail or Messenger, but it is an additional chore. In this case, Dooray! recommends the person who discovered the inappropriate task status to change it appropriately. Anyone who has the permissions for the task can change the status of each owner, even if he or she is not the owner. Click the task status to change the task status to Registered / In Progress / Completed. As permissions are granted to anyone, all history of the actions are logged. Therefore, no one will change the status arbitrarily without consideration.

## Change the Task Attributes

#### Change with the ‘Edit' button

-  Click the ‘Edit' button to enter or modify all items of a task in a new window. It is useful when two or more items should be modified.

#### Edit Owner and CC in-Place

- To change the owner and CC only, click the \[Figure\] Pencil icon of the Owner and CC.

 ![Edit](http://static.toastoven.net/prod_dooray_project/detail/26_pjt_detail_edit_to.png )
 <center>[Figure 26]Edit the Owner</center>   

- Hover over the Owner area to display the 'Be Mine' button. Click the button to move the existing owners to the CC field and only you are left in the Owner field.
- It is useful when you allocate a task to a member group and a member who will do the task makes the owner clear by clicking the 'Be Mine' button.

 ![Be Mine](http://static.toastoven.net/prod_dooray_project/detail/27_pjt_detail_edit_to_me.png)
 <center>[Figure 27]Change the Owner by Using Be Mine</center>   

#### Edit the Title In-Place

- Hover over the title and click the \[Figure\] Pencil icon to edit the title only.
  
  ![Edit the Title](http://static.toastoven.net/prod_dooray_project/detail/28_pjt_detail_inplace_title.png)
  <center>[Figure 28]Edit the Title</center>   

#### Edit the Body In-Place

- Click the \[Figure\] Pencil icon in the task reading window to edit the body only.

 ![Edit the Body](http://static.toastoven.net/prod_dooray_project/detail/29_pjt_detail_inplace_body.png)
  <center>[Figure 29]Edit the Body</center>  

-  Click ‘Save’ to save the changes and the screen is switched to the read screen. However, clicking 'Save and Continue' to save changes and keep the edit mode. Since ‘Save and Continue’ does not save changes temporarily but completely on the server, remember that someone else can view the changes.

#### Edit the Completion Date In-Place

- Click the completion date on the top right of the task to edit the date.

 ![Edit Completion Date](http://static.toastoven.net/prod_dooray_project/detail/30_pjt_detail_inplace_duedate.png)
 <center>[Figure 30]Edit the Completion Date</center>  

#### Edit the Tag In-Place

- Click the \[Figure\] Tag+ icon under the title to edit the tag.
- Depending on the attribute, you can or must select a tag from the grouped tags.
  
  ![Edit Tag](http://static.toastoven.net/prod_dooray_project/detail/31_pjt_detail_inplace_tag.png)
  <center>[Figure 31]Edit the Tag</center>  

#### Edit the Milestone In-Place

- Click 'Milestone' at the top to edit the milestone.

 ![Edit Milestone](http://static.toastoven.net/prod_dooray_project/detail/32_pjt_detail_inplace_milestone.png)
 <center>[Figure 32]Edit the Milestone</center>  

#### Move to Another Project

Select - ‘Additional Task &gt; Move to Project’ to move to another project. When moving, you can specify and change the tag and milestone of the project to move to at once.

 ![Move to Project](http://static.toastoven.net/prod_dooray_project/detail/33_pjt_detail_move_project.png)
 <center>[Figure 33]Move to Project</center>  

### Write a Comment

#### Write a general comment

- You can add a comment as feedback for a task. You can add a long comment as well as a short one. The formats of the body, comment, and document are the same.

#### Change the Owner Using Mention

- In many cases, when changing an owner, people tend to leave a comment that the task owner has been changed to someone while forgetting to actually change the owner. With Dooray!, you can easily handle this kind of issue.
- Just add the ‘-&gt;’ symbol before the mention. Then, the mentioned member or guest will become the owner and the previous owner will be relocated into the CC field. Think of the symbol as a finger pointing at the
 owner.
- Dooray! A project can have a multiple owners. To add an owner, add ‘-&gt;&gt;’ before the mention.

#### My Comment 

- We discuss with others using so many comments and replies in a task. When this happens, it is often hard to track all the comments you've made. In this case, click the ‘My Comments’ box above the Project Task box to view all of your comments. This is Dooray!'s unique function which is not provided by any other services, which allows you to manage your comments in a simple way.

### Change History 

#### Show Changes in Task 

- All changes related to a task are provided as a history. As well as changes in the task, such as task title, owner, schedule, body text, and file attachments, you can check the changes in comments by checking the 'Include Changes' box at the bottom right of the task body. You can view all changes in the body and comments.

  ![Change History](http://static.toastoven.net/prod_dooray_project/detail/34_pjt_detail_edit_history.png)
  <center>[Figure 34] Change History</center>  

### Adjust Window Size

#### Open new window

- On the Read screen, click the \[Figure\] New Window icon at the top right to open the current task in a new window. The shortcut is vn (ViewNew).

#### View in Wide Window

- The Read screen may be narrow in the split view mode. In that case, click the \[Figure\] Expand Body icon for a wider view. The shortcut is vw (ViewWide). To return to the normal view from the expanded view, click the icon again or enter vw again.

### Change the Screen Mode 
 
#### Meeting Mode

- In some case, you may open the Dooray! screen through the beam projector during a meeting. If it is hard to read the screen as the font size is too small, ‘Meeting Mode’ is helpful.
Click the - \[Figure\] View Body icon and then select ‘Meeting Mode’. The Meeting Mode removes any other areas except for the task body and increases the task body font size. Press \[ESC\] or click the ‘Close’ button at the bottom of the screen to exit the 'Meeting Mode'. The shortcut is vm.

#### Presentation Mode

- Presentation Mode generates a task created with Markdown as a presentation document. You can switch the task body to the presentation mode without creating a presentation document separately.
Click the Figure-  View Body icon and then select ‘Presentation Mode’. The shortcut is vp (View Presentation).

  ![Presentation Mode](http://static.toastoven.net/prod_dooray_project/detail/35_pjt_detail_vp_mode.png)
  <center>[Figure 35] Select Presentation Mode</center>  

- Select the desired skin for the presentation screen and click 'OK' to change the screen to the presentation screen. To move to the next screen or effect, press \[\] key on the keyboard.
- If there are too much content and it is difficult to view all of them in one screen, click \[\] to scroll automatically to view the next hidden content.
- Press the Shift key during presentation to display the spotlight. Press the Shift + Ctrl keys to use the magnifier feature which magnifies the spotlight.

### Set Notification

#### Set notifications for Project, Mail, and Calendar 

- Dooray! You can set the notifications of Project, Mail, and Calendar services. You can select a project to receive the notifications per owner, CC, and task sent as well as the notifications for new tasks and comments. 
- You can select a mail box to receive all mails or notifications as well as notifications for new mentions. 
- There are three notifications types: notifications via mobile app, messenger, and external email.

 ![Set Notifications ](http://static.toastoven.net/prod_dooray_project/detail/36_pjt_detail_setting.png)
 <center>[Figure 36] Set Notification</center>  

## Shortcut 
- Dooray! Service's shortcut are as follows.  

| Type   | Shortcut  |  Features |
|--------|---------|-----------------------------| 
|Read Task screen | vn | View New window |
|   | vp | View Presentation mode |
|   | vm | View Meeting mode |
|   | vw | View Wide | 
|   | cu | Copy the permanent address to Clipboard (Copy Url)  |
|   | cb | Copy the body to Clipboard (Copy Body) |
|   | cn | "(Query)Dooray/56" copies the task string to Clipboard (Copy Number) | 
|   | cs | Copy the task subject to Clipboard (Copy Subject) | 
|Write screen | ww | Write window (Write task for Project, Write mail for Mail, Write calendar for Calendar) (Write Write) | 
|   | fw | Fast task write window (Fast Write) | 
|   | cc |  Focus to Comment window (Comment Comment) | 
|   | wt | Write task window (Write Task) | 
|   | wm | Write mail window (Write Mail) | 
|   | we | Write event window (Write Event) | 
|   | wk | Write contacts window | 
|Go to Service | gs |  Open the stream (Go Stream) | 
|   | gp |  Project tab (Go Project) | 
|   | gm| Mai tab (Go Mail) | 
|   | gc |  Calendar tab (Go Calendar) | 
|   | gd | Drive tab (Go Drive) | 
|   | gk |  Contacts tab | 
|Calendar| cd | Calendar daily view | 
|   | cw | Calendar weekly view | 
|   | cm | Calendar monthly view | 
|   | c2 | Calendar 2-week view | 
|   | c3 | Calendar 3-week view | 
|  Register  | Ctrl(Cmd) + Enter | Register Windows (Mac) Editor | 
|  Save as Draft  | Ctrl(Cmd) + s  | Save as Draft in Windows (Mac) |
|  Select a drive folder to reference  | Alt + Enter | Select a drive folder to refer to in Editor with [ | 
|  Others  | ms  | Toggle to mark a star (Mark Star)  | 
|  | Alt + Up/Down  | Go to line (also available when selecting multiple lines in Editor)  | 




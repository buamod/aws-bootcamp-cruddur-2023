# Week 0 — Billing and Architecture

- Finished Watching all the videos in the TODO checklist 
- Finihsed all the pre-requested stuff
- The Conceptual diagram

![napkin](https://user-images.githubusercontent.com/2315602/219843562-ba614fc6-908a-41e8-a27e-b4346a153b89.jpeg)

- The Logical diagram [Link](https://lucid.app/lucidchart/8d1838b5-251d-43b8-ade2-55b52fc0d665/edit?view_items=mjfyb.n0phJe&invitationId=inv_6a5c63ab-abfd-4a77-b8c9-16d22712c2aa)

![Cruddur Logical DIagram](https://user-images.githubusercontent.com/2315602/219843711-6d01da6e-e57c-44ea-ba61-434aa0d528fb.png)

- I have created the AWS budget, Billing alaram and SNS topic using AWS CLI on the gitpod 
 
 ```
 aws budgets create-budget \
    --account-id ACCOUNT \
    --budget file://aws/json/budget.json \
    --notifications-with-subscribers file://aws/json/notifications-with-subscribers.json


    aws sns subscribe \
    --topic-arn="arn:aws:sns:us-east-1:254057183117:billing-alarm" \
    --protocol=email \
    --notification-endpoint=email@gmail.com
 ```



- I noticed that AWS has changed the way a user get created, wow I did that 7 years ago. 
- Also I noticed accessing the billing is not available on the admin user( will debug it futher ) 


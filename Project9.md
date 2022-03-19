## Project Workflow

Step 1 - Spin up 4 EC2 instances, one for the control node and 3 for the frontend and backend services.

![IMG_9351](https://user-images.githubusercontent.com/93732510/159123863-febbe04b-0030-43ba-b5fe-7dd9b1e091c1.jpg)

Step 2 - ssh into the control machine and install ansible.

![IMG_9342](https://user-images.githubusercontent.com/93732510/159124101-8dabca8a-68d2-4cf1-b311-04e5e11ebf13.jpg)

Step 3 - Create directory where the operation will be performed and cd into it. 

![IMG_9343](https://user-images.githubusercontent.com/93732510/159124505-090e956d-eb1f-4151-be79-21d814d896ea.jpg)

Step 4 -  Create an inventory file using vim, write the node details in the file to include, host name, IP address, ssh details etc.

![IMG_9347](https://user-images.githubusercontent.com/93732510/159124685-ccba25af-607d-4731-998a-7ea49ca52312.jpg)

Step 5 - Write the playbook using vim to define tasks that the control machine will deploy to the nodes.

![IMG_9360](https://user-images.githubusercontent.com/93732510/159124812-04cda92a-14bf-48fc-9bdd-5e65d8506911.jpg)

Step 6 - We can do syntax check to ensure no issues with indentation in the playbook.

![IMG_9356](https://user-images.githubusercontent.com/93732510/159125010-f9b7b7cd-e07f-4fe5-8779-490a3864635f.jpg)

Step 7 - Now we run the playbook using the playbook command.

![IMG_9358](https://user-images.githubusercontent.com/93732510/159125084-618dace3-c18f-45ea-a9c0-8c7cb7ff7e81.jpg)

Step 8 - Copy the public IP address of the instance for frontend server after enbling port 80 in the security group and check the deployment via browser.

![IMG_9362](https://user-images.githubusercontent.com/93732510/159125989-f6969ed3-b831-4864-ac16-b5cffa16525d.jpg)

Side Note, we can run the deployment using ad hoc commands as well from the command line. 

![IMG_9350](https://user-images.githubusercontent.com/93732510/159126111-cf11e5c4-e915-479a-8f2a-ba321bd6f171.jpg)

The ad hoc commands are repeated for all 3 instances and we can view the deployment in the browser.

![IMG_9361](https://user-images.githubusercontent.com/93732510/159126227-82ba39fb-c509-4285-9791-c83a6a8e9f7a.jpg)









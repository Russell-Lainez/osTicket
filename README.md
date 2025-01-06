<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>Resolving Help Desk Tickets through osTicket</h1>
In this demonstration, I will show how I used osTicket to address and solve imaginary help desk tickets. I will walkthrough how I launched the osTicket program, how I configured osTicket to properly work tickets, and how I resolved incoming tickets. 


<h2>Environments, Applications, and Services Used </h2>

- Microsoft Azure (Virtual Machines/Virtual Network)
- Remote Desktop
- osTicket
- Internet Information Services (IIS)
- Windows 10Pro (22H2)
  
![image](https://github.com/user-attachments/assets/c515076c-c86c-46ee-9388-cbd71a678138)



<h2>Demonstration</h2>

<h3>Launching osTicket</h3>
<p>
After creating a virtual machine and virtual network in Azure, I downloaded all the required dependencies and configured my computer to enable osTicket: 

  - Installed and enabled ISS with CGI

    ![image](https://github.com/user-attachments/assets/da13da80-d4ab-48ff-8dbf-47ec86dd12b7)


  - Installed PHP Manager, IIS Rewrite module, C++ Redistributable, and mySQL Server

    ![image](https://github.com/user-attachments/assets/5af370a6-b868-4e25-9f8c-ab1f63748d5e)
    ![image](https://github.com/user-attachments/assets/8565ff6a-9acc-44e7-a1e1-6e09fa86b6fa)
    ![image](https://github.com/user-attachments/assets/85a92347-995a-4c91-962d-6e9e5ff4229b)
    ![image](https://github.com/user-attachments/assets/2998525b-39e2-41f1-ba43-e584b4264f5b)

  - Registered PHP from within ISS and opened osTicket

    ![image](https://github.com/user-attachments/assets/f31b8f56-c2f8-4872-8627-339b72d8e259)
    ![image](https://github.com/user-attachments/assets/951d6ed7-38c6-4f0a-9d1f-62780c59f5c3)

  - Added the necessary extensions and configured Heidi SQL to create the backend database for osTicket 

    ![image](https://github.com/user-attachments/assets/18c173ce-b9ce-49a7-8d97-a8c5e70b03a7)
    ![image](https://github.com/user-attachments/assets/854b0d62-c81c-47b3-a9c2-d3777c7da69e)
    ![image](https://github.com/user-attachments/assets/1b4afc16-986a-42bf-81df-c9bd44eb185b)

<h3>Configuring osTicket</h3>

  - Before submitting help desk tickets, I created staff members to solve incoming tickets:
    - Jane Doe
    - John Doe
      
      ![image](https://github.com/user-attachments/assets/d78cc230-9066-4d11-9d77-51c1819fa44f)

  - I created end users, Bob and Karen, who would be able to submit tickets:

      ![image](https://github.com/user-attachments/assets/2c67ab83-f769-432e-815c-7e8f1ac23677)

  - I defined 3 types of SLAs to categorize tickets appropriately:
      - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
      - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
      - Sev-C (Grace Period: 8 hours, Business Hours)

        ![image](https://github.com/user-attachments/assets/5928aec6-9a5f-4ecf-a44b-ecac54e78443)
   
  - I created different teams and added each staff member to a team:
      - Online Banking - Jane Doe
      - Level I Support - John Doe

        ![image](https://github.com/user-attachments/assets/5faf5950-9f8b-4be1-aac3-5f8ed2f660cf)

  - I created different access for each staff member:
      - Jane Doe - Full Access Admin
      - John Doe - Limited Access

        ![image](https://github.com/user-attachments/assets/e27a7802-4962-4b1e-88e7-d7ec98d1b3b0)

  - I created one more department and added each staff member to a department:
      - Support - John Doe
      - SysAdmins - Jane Doe
        
      ![image](https://github.com/user-attachments/assets/ba744187-a00b-4c0e-9038-407678d89ef9)
   
  - I created different help desk topics, so the end user can appropriately categorize their inquiry:
      - General Inquiry
          - Equipment Request
          - Other

      - Report a Problem
          - Business Critical Outage
          - Password Request
          - Personal Computer Issues

      ![image](https://github.com/user-attachments/assets/4cced860-8519-4b2e-a64b-19d725b1f540)

<h3>Resolving Help Desk Tickets</h3>

  - As Karen, I submitted a help desk ticket asking IT to prepare an assigned laptop for a new staff member. As the admin, I assigned the ticket to John Doe and informed him to complete the request by end of the 2nd day. I then changed the SLA to SLA-C (Grace Period: 8 hours, Business Hours) because it is a timely request and not a high priority.
    
    ![image](https://github.com/user-attachments/assets/78ef4317-3d3a-42c2-8357-b7b6f3e124c7)

    As John Doe, I made an internal comment stating I can finish the assignment by noon tomorrow. Then, I sent a message to Karen asking for the employee’s name and ID number.

    ![image](https://github.com/user-attachments/assets/a5592a69-3858-4c40-aad3-6273ea6d2fea)

    I then resolved the ticket and added a follow-up note stating I delivered the computer.

    ![image](https://github.com/user-attachments/assets/10757f3d-cfc4-4f77-8e41-b1714ba34fac)

  - As Bob, I submitted a help desk ticket letting IT know the entire team’s Adobe is down and essential for everyday work. As the admin, I made an internal note saying the request is critical and needs to be solved ASAP then transferred the ticket over to the SysAdmins department. I changed the SLA to Sev-A (Grace Period: 1 hour, Schedule: 24/7) due to the high priority of the ticket. 

    ![image](https://github.com/user-attachments/assets/ad8affe7-4c19-4dab-a8e4-3d011944bcc7)

    As Jane Doe, I assigned the ticket to myself and added an internal note stating I would contact Bob shortly.

    ![image](https://github.com/user-attachments/assets/59a901c3-94da-48ae-874c-1eb308618efb)

    Continuing as Jane, I then messaged Bob to call me, so we could discuss more. I resolved the ticket and added a note stating Adobe needed updates, so I updated Adobe for Bob and the entire team.

    ![image](https://github.com/user-attachments/assets/231fa9f3-9931-4e82-b83b-10500e4ef1ea)

</p>
<br />

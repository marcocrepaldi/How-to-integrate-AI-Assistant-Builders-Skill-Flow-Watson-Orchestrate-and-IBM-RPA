How to integrate AI Assistant Builders, Skill Flow, Watson Orchestrate, and IBM RPA?




Repository: 

All the necessary files to replicate this content are available in the repository.

How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA




1. Introduction




Digital transformation is revolutionizing the way companies operate by integrating advanced technologies to automate processes and improve efficiency. One such innovation is the integration of virtual assistants, workflow orchestration, and robotic process automation (RPA). This article explores the integration between the AI Assistant Builder, Watsonx Orchestrate, and IBM RPA, demonstrating how these technologies can be used to optimize the registration process in the JK Automation system through a chat interaction.




2. Overview of Technologies




AI Assistant Builder

The AI Assistant Builder is a chatbot creation platform that allows companies to develop customized virtual assistants. With the ability to understand and respond to user queries, these virtual assistants enhance customer experience and operational efficiency.




Watsonx Orchestrate

Watsonx Orchestrate is a powerful IBM tool that enables the automation and orchestration of complex workflows. It integrates various applications and services, allowing seamless and automated communication between different systems.




IBM RPA

IBM Robotic Process Automation (RPA) is a solution that uses software robots to automate repetitive and rule-based tasks. It enables companies to increase efficiency and reduce human errors, freeing employees for more strategic tasks.




Benefits of Integration

The integration of these technologies allows for complete automation, from the initial user interaction to the execution of complex backend processes. This results in greater efficiency, reduced processing time, and a smoother user experience.




3. Project Scope




The scope of this project is to create a chat conversation in the AI Assistant Builder that collects registration data for the JK Automation system. During the user interaction, the necessary parameters will be collected and used to trigger a workflow in Watsonx Orchestrate. This, in turn, will trigger an IBM RPA bot to perform the required actions in the JK Automation system.




4. Implementation




AI Assistant Builder Configuration

Firstly, the AI Assistant Builder is configured to collect the necessary data from the user. This includes creating intents, entities, and dialogues to guide the user through the registration process.




Creating a Skill Flow in Watsonx Orchestrate

Next, a Skill Flow is created in Watsonx Orchestrate to manage the data collected by the chatbot and trigger the IBM RPA bot.




Integration of Watsonx Orchestrate with IBM RPA

The integration is achieved by configuring Watsonx Orchestrate to call the IBM RPA APIs, passing the data collected by the chatbot and executing the necessary actions in the JK Automation system.




Data Flow and Communication

Data flows from the AI Assistant Builder to Watsonx Orchestrate and then to IBM RPA, ensuring that each technology performs its role in an integrated and efficient manner.




5- Step by Step
![Screenshot 2024-06-18 at 16 46 10](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/f5ba1cd4-6ec5-4254-8280-b3ad50d71620)


5.1  - IBM RPA

First, let's develop a bot in IBM RPA that manipulates the JK Automation system and registers the records collected in the AI Assistant Builder. The following example illustrates a simple system where we register records with the following fields: First Name, Last Name, E-mail, Job Title, Company, Phone, Address, City, State, Zip Code, and Area of Interest.


![Screenshot 2024-06-18 at 16 46 32](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/aaa83878-8ef6-42a4-8001-8e2473aa023b)





5.2 - Variables output 

In your bot, ensure that the parameters are defined as input variables. When you download the OpenAPI, these parameters will be configured in the XML structure.

![Screenshot 2024-06-18 at 16 47 09](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/16b62109-0534-42c9-a5a9-168834d3a5b3)



5.3 - Download OpenAPI

Once the bot development is complete, it's necessary to publish the project so that we can download the OpenAPI, which contains all the input and output parameters of the bot.

![Screenshot 2024-06-18 at 16 46 46](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/3200c587-2514-4cb8-9bdf-488ec4f7491f)




5.4 - Acess Skills and apps Watsonx Orchestrate

You should access Watson Orchestrate, log in, and then navigate to "Skills and Apps".



![Screenshot 2024-06-18 at 16 48 20](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/aacd468a-6cb4-4233-a7e0-dcb9a57dcbec)




5.5 - Create a new skill app and publish.

You should add a new skill from a file. Drag the OpenAPI file that you downloaded earlier to import the skill file, Enhance this Skill and Publish.

 ![Screenshot 2024-06-18 at 16 48 57](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/c35328a3-ca0a-4bd3-9f1b-173d141b62bd)





5.6 - Connect your application and add it to the catalog.

Access the "Skill Catalog" and locate your new skill. Click on the skill and then establish the connection by clicking on "Connect App". Enter your IBM RPA Control Center credentials. If the information is correct, the app will be connected. Next, click on "Add Skill +" to add the skill.

![Screenshot 2024-06-18 at 16 49 14](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/3d06ab34-8dda-4841-b2eb-24aa5e1d5b31)



Now let's create our chat in Assistant Builders 



5.7 - Create a new Actions AI assistant builder

![Screenshot 2024-06-18 at 16 49 37](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/a87751aa-feb0-4972-991e-3a390e952938)

Now let's create our chat in Assistant Builders, access Ai Assistant Builder/ Action.

5.8 - Click on New Action
![Screenshot 2024-06-18 at 16 49 58](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/47ee26d9-7332-4f87-81ba-76021a0d761b)


5.9 -  Click on Custom-built-action
![Screenshot 2024-06-18 at 16 50 15](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/589b2a29-3f03-4af4-8172-914504cf430a)


5.10 -  New Action - What does your customer say to this interaction? 
![Screenshot 2024-06-18 at 16 50 36](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/6ca7928e-eab9-4eff-b97b-e9d68a8d550f)

You can add multiple triggers later to start your interaction. At this stage, we will insert just one initial trigger, and in the future, you can create various other triggers to start your interaction.

5.11 - First interaction
![Screenshot 2024-06-18 at 16 50 49](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/c5bcb8a1-460d-48e2-9d01-644fc21ac746)

In the first step 1, we will input the initial question directed to the user. Our goal is to collect all the necessary information for registration in the JK Automation system, so at each step, I will gather mandatory records.



5.12 -  Click on customer response

![Screenshot 2024-06-18 at 16 51 05](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/7a4f65d0-8572-4ede-b606-07496abd147d)



5.13 -  Select Free text  


![Screenshot 2024-06-18 at 16 51 22](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/336a4202-53e1-4a16-a625-0f9473790d16)



5.14 -  And Then

   And then, select continue to next step

![Screenshot 2024-06-18 at 16 51 41](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/88ac3ac4-cdc0-4d79-b27b-9d3890bc6afd)



5.15 - Remember to click the "New Step" button to continue with new interactions.

![Screenshot 2024-06-18 at 16 51 55](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/0c008636-b92d-4f84-aee9-27fd2cd51f04)



** You must repeat steps 5.11, 12, 13, and 14 to request information for all fields that need to be entered into the system (first name, last name, email, Job title, Company, Phone, address, City, State, Zipcode, Area of Interest) a total of 11 steps.

image01

![Screenshot 2024-06-18 at 16 52 13](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/4cbc5157-ef35-464f-a02f-8dcc90840314)



image02

![Screenshot 2024-06-18 at 16 52 27](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/fa38740e-1380-4427-9bb0-f511accebec2)



5.16 -  Created by you

In the Action menu/ variables, select "Created by you" and then click on the "New Action" button.

![Screenshot 2024-06-18 at 16 52 44](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/b574267d-288f-415d-8913-aa71b329e3d4)



5.17 - New variable 

You should define all the variables and types before clicking on the save button.

*** You must create a total of 11 variables (first name, last name, email, Job title, Company, Phone, address, City, State, Zipcode, Area of Interest)

![Screenshot 2024-06-18 at 16 53 53](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/4c399323-4c01-42ae-a242-fe3bbecae225)



5.18 -  Set Variable Values 

Return to Action/ Created by you / JK Automation Skill Flow 

![Screenshot 2024-06-18 at 16 54 08](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/182b5163-cfeb-4631-ba73-d69f2e6a6656)

let's create a new step 12, where we will enter the values ​​entered by the user and present them in a summary

In this step, we will assign the values entered by the user to the variables we have created during the Assistant interaction.. These values ​​will be sent to the Skill flow through an API.


Click on the Set Variable Values 

![Screenshot 2024-06-18 at 16 54 29](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/9287d801-c9ad-4bde-b0f2-ea020770d3c3)


5.19 - Click on the Set New Value
![Screenshot 2024-06-18 at 16 54 53](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/bd135c53-8179-42fe-9310-2e69f0dd965a)

5.20 - Click on Session variables

![Screenshot 2024-06-18 at 16 55 08](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/de39b60b-53f4-49de-8de7-b006bf7a697d)

5.21 -  Select firstName variable


![Screenshot 2024-06-18 at 16 55 26](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/076e86ce-de1d-425e-8dd8-32fced564ce7)


5.22 -Variable Values TO

![Screenshot 2024-06-18 at 16 55 44](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/9c9f4e0e-71c2-4f7a-a568-4cbbe94db5ee)

We set the variable firstName with the value entered in step 1. Repeat steps 5.19-5.22 for all variables created in step 5.17.
![Screenshot 2024-06-18 at 16 56 17](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/561fb44e-765b-488b-af4c-730cba1cd579)


the result will be this


![Screenshot 2024-06-18 at 16 56 30](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/b132285b-e9da-4425-8d83-f7891e195fd8)



5.23 -  Tell the assistant what he will say

![Screenshot 2024-06-18 at 16 56 45](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/d118e028-c024-4512-959f-1e56a2614acd)



5.24 - Insert Variable 

Click on 'Insert Variable.' In this interaction, we will display the phrase provided in the previous step and the values of all the variables collected during the interaction with the user. 

![Screenshot 2024-06-18 at 16 56 58](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/30ba06cb-8084-4059-ac9b-0d3331a416a6)



5.25 -  Click on Session variables


![Screenshot 2024-06-18 at 16 57 09](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/d920b7f8-eb70-47fd-bfaf-5c713ba7fa5f)


5.26 - Select the first variable

![Screenshot 2024-06-18 at 16 57 27](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/0a4d3e05-fc15-4273-b400-a11fe1757708)



5.27 - Variables displayed in the dialog

Repeat steps 5.24 - 5.26 for all variables you want to display in the interaction.

![Screenshot 2024-06-18 at 16 57 42](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/50b48874-4d29-4556-9b5e-658b20bd3406)



5.28 -  Define customer response

  Click on Define customer response
  
![Screenshot 2024-06-18 at 16 58 04](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/23e3ba07-81bd-4077-860d-af02c12243c1)

5.29 - Select Confirmation 

![Screenshot 2024-06-18 at 16 58 29](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/1385d3c3-c559-48a6-b5d8-2eff723c6c88)


5.30 - Let's create a New Step(

Let's create a new step (13) and set the condition to "NO". If the user clicks the "NO" button, we will end the interaction.

![Screenshot 2024-06-18 at 16 58 47](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/0a9d64d1-df5d-4f18-ac72-6b5e833bc0cc)

5.31 -  Select no condition 

![Screenshot 2024-06-18 at 16 59 05](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/d3a192d2-88b1-480e-8194-959564038b5c)


5.32- end of interaction

![Screenshot 2024-06-18 at 16 59 52](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/42ee4b92-a8b3-46ea-bb3e-31e2da3f837d)



You can display a message to the user and select to End the action.




When you choose the "NO" option in the previous step, you are terminating the interaction with the user.




5.33 - let's create a new step (14) with the YES condition
![Screenshot 2024-06-18 at 17 00 14](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/50c9dea8-cfad-452a-8e33-673e4012e039)


5.34 -  You can display a message to the user who is going to register

![Screenshot 2024-06-18 at 17 00 30](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/0deabf99-c387-4c2d-a34e-31d88981aca1)

5.35 Click on save

![Screenshot 2024-06-18 at 17 00 50](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/6c483419-6155-4d8d-befd-a2512b66bff3)



Now, let's create a custom extension.

Get started


Create a custom extension to tailor the experience for your customers.
Steps to setting up custom extensions:
Provide an extension name and description that clearly explains what the extension accomplishes.
Import your OpenAPI document as a JSON file to start building your custom extension.
Select the environment (Production, Development, or Stage) to use your extension and the authentication type to complete the setup process.




5.36 -  Click on the integration on the left side
![Screenshot 2024-06-18 at 17 01 10](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/237ed729-ca69-4cf9-b3c3-1c5c744ed763)




5.37 - Click on Buld custom extension
![Screenshot 2024-06-18 at 17 01 28](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/53ae59e0-4e5c-4899-a2cd-7c7a5c342003)

5.38 - Click Next 

![Screenshot 2024-06-18 at 17 01 42](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/3dbfc1e4-9a73-4587-bed1-680e8689b772)


5.39 - Enter the name and description and click next

![Screenshot 2024-06-18 at 17 02 05](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/292bf3c1-bf19-4179-aed6-9eef4e52663f)



5.40 - import OpenAPI


![Screenshot 2024-06-18 at 17 02 18](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/413dbea9-0597-4659-98a3-0afb5f89eb13)





******To export the file, navigate to Skills and apps, select the three dots next to your skill, and choose Export this skill.

![Screenshot 2024-06-18 at 17 02 37](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/297a36b9-4062-4eab-8556-7722a809cc1e)


5.41 - when loading the file click next

![Screenshot 2024-06-18 at 17 02 56](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/e473dda5-74ae-4cf2-9abe-2a6053d50d55)


5.42-  Check the information and click Finish.
![Screenshot 2024-06-18 at 17 03 12](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/e92d8422-b457-4051-94f7-3d6c49d61344)



5.43 - Find your extension and click add
![Screenshot 2024-06-18 at 17 03 29](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/52917a1a-dbf5-4db4-a916-7f2123521fce)


5.44 - Click on Add
![Screenshot 2024-06-18 at 17 03 41](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/0f6d1c69-487a-480b-adda-53a947c376f1)

5.45 - Custo Extension

![Screenshot 2024-06-18 at 17 03 56](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/307b13ef-51c1-4eb8-b348-da405fa88d5d)



Click on Next




5.46 - Select Outh 2.0

![Screenshot 2024-06-18 at 17 04 13](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/c9a150c2-6559-49e6-b25d-4bbc5b938a43)

5.47 - Click with your IBM RPA control center information, the Client ID and Client Secret fields can be filled with fictitious values, the fields that will be validated are the username and Password, then click Next.


![Screenshot 2024-06-18 at 17 04 29](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/34735cfd-6662-4709-a064-2288033d3424)



5.48 - Click on Finish

![Screenshot 2024-06-18 at 17 04 45](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/7c7e664e-ec6e-42fd-90e0-c2744735175d)



5.49 - Return to step 14 and select 'Use an Extension' in the 'and then' option.

![Screenshot 2024-06-18 at 17 05 02](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/235930dd-0d3d-43d6-8b3e-2c0d6fe48901)



5.50 - Select the "JK Automation Skill and IBM RPA" extension, choose the "Jk AutomationSkillFlow" operation, map the parameters with the interactions step, and then click Apply.


<img width="911" alt="5 50" src="https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/be21a83b-e5b3-4a02-91c5-92684cb7c901">



5.51 - Don't forget to save

![Screenshot 2024-06-18 at 17 07 09](https://github.com/marcocrepaldi/How-to-integrate-AI-Assistant-Builders-Skill-Flow-Watson-Orchestrate-and-IBM-RPA/assets/9463175/93054c47-103a-450b-8f52-e46ba472b487)



Congratulations, you have completed this lab. 

If you are an IBM employee and have any questions, please contact me on Slack Marco Crepaldi ,If you are a business partner or from any other area, it will be a pleasure to help you, contact us via Linkedin 

 LinkedIn profile https://www.linkedin.com/in/marco-crepaldi/


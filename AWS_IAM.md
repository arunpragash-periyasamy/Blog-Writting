# IAM in AWS. How to create users in IAM. How to create Policies in IAM.
Hi everyone. In this blog post we can learn about what is IAM in the AWS. AWS (Amazon Web Service) is a cloud platform which provides the users IAAS (Infrastructure as a Service) and providing a various types of services. IAM (Identity and Access Management) is one of the service provided by the AWS. We are using this service for managing the users and groups of people to access the various AWS services in the single aacount.
# What is an IAM
IAM is an service offered by an AWS to create and maintain the users and groups. Which is the place to provide access to the services for the specific user or a specific group. Let's discuss what is user and group later in this post. 
AWS provides various web services(200+) for their customers for various purpose. Eg. EC2 (Elastic Cloud Computing) which provides you the virtual system with OS to access using internet from anywhere in the world. We are restricting the user or a group of people to use all the services and provide access to the some of the services who needed.
# Why IAM (Identity and Access Management)
In a real time scenario, a company or an organisation has their requirement to work on different projects. For our understanding we can take a single project, and discuss how does IAM works in the project will be looking into. Let's take e-commerce project and how IAM will come into the picture.
In that project there are multiple teams are working for the project like Development team who is developing a product. Then Testing team who can test the developed product is working fine or not, finding the bug. And the Operation team who can deploy the product and managing the application should not be down at anytime. In IAM we can create and maintain the users and groups.
# Why Users in IAM
In a project every person need the access to the AWS services. So we need to create a separate login to use AWS account. For that reason AWS provides IAM service to create multiple users and maintain those users. Not only for creating users and also provide access to user for accessing the necessary service and restricting the user from using the unwanted or unnecessary service.
Why we need to restrict the user from accessing various service. AWS is a cloud provider, which provides various services at affordable price to access the resources. But when we are using the service which is not really necessary or unintentionally created the service and forget to stop the service then it will be increase the billing cost of the AWS.
# Why Groups in IAM
In a e-commerce project there are multiple team working as we seen before. These teams are using the AWS for developing the product. Each team need access for specific services and varies for team to team. We need to give access to the necessary services for all the person who are all working in a team. Instead of going to each user and provide access to the each services what they need. We can create a group and map the people in a group and give access to that group will applied to the persons who are all in the group.
Where a single place to update the access and policy. In AWS normally mentioned policy which defines the rules that which services are accessed by the whom.

# How to Use IAM
Login with your Root user credentials
![Screenshot 2024-04-11 215540](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/14c61298-8ef2-4410-8bf4-39d4a12f87f4)
Root user login in the AWSAfter entering your root mail id then it will redirect to a page and asks you to enter the password. After you provide your credential then it navigate to the dashboard of AWS.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/d400c7f3-ecbe-4282-a033-a2a38d6235d3)

Dashboard of the AWSHere you can see the "Recently Visited" widget which showing that recently used services in the AWS by ourself. Here I used IAM and EC2 service before so it listed here. 
Now we are entering into the IAM service by clicking the IAM service which is listed in the recently visited. Don't worry if you are just logged in first time and not showing the service in the Recently Viewed, then you can click the services button on the top navbar near to aws logo or search in the search input as IAM.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/d79f526e-58d1-4a9d-9af0-97661afbc2a3)
Click the search button and type IAM it will list the service, and select the IAM service.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/d82783a8-eecf-4566-b256-961016abaac7)
IAM service listing in the searchwhen you click the IAM service it will redirect to the IAM dashboard.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/04568abf-4898-4ced-b69b-6691df62be5e)
IAM dashboardIn the IAM dashboard you have given the account id which is shown in the right side of the IAM dashboard. Which will be used in the IAM user login, you need to provide account id or account alias. 
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/d54deb03-d0c6-4e70-8d9f-b21b68e91115)
Your AWS Account IDIt's quite hard to remember or made a mistake while login using this lengthy number. To avoid this AWS offers us to create an alias which is alternative for Account Id. Wait Wait! What is this Account ID? What is Account Alias? Why we need to create this?. Just remember this we can see where it is used later in this post. 
One more important thing in AWS is we can use each service in any region where we need to create near by server. But IAM is global region that mean user from any where can access and common for entire AWS region. Don't frustrated with these terms Account Id, Alias and Region. We can cover it in the post later.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/3306ae1c-f8bc-44bd-8b31-a7c6e54d41aa)
Create a account aliasHere you can create account alias by clicking a create. And this should be unique one by using small alphabets (a-z), numbers(0–9) and hyphen(-).  Other than these character you cannot use any characters. It is like a username in the social media. It should be unique if someone already taken a name that you need then you can not get that name. For eg I tried to create alias with my name but it shows that already taken.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/e17fb8c4-f42a-4cb7-912e-e5e035881138)
Account alias already takenSo I cannot get the arunpragash so i need to choose another name so I tried with another name.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/5b4d1508-6c0a-45fd-8273-b69a6412aa95)
Create with unique nameAfter given your unique then click create alias button, it will create an alias for your account. And show alert that alias created successfully. And also you can right side account alias is created. Then the sign-in URL also generated for IAM user to sign-in.
![image](https://github.com/arunpragash-periyasamy/Blog-Writting/assets/79126203/1fe1a54f-bedb-440d-9ebd-a4de589391a5)
Alias created successfully.

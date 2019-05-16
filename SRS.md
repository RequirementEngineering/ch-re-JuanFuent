APP FOR A Restaurant Management System (SRS)
=
Introduction
-
PURPOSE
-
The purpose of this SRS document is to coer the overall description of the Restaurant Managemet System, specifically the product perspectvie, function, characteristics, some contrains. It will also describe how the system will pergom and under which it must operate.

SCOPE
-
Generally the menus of a restaurant are based on paper and therefore impose restrictions on the prices available and a responsibility to update them. The first step in this SRS document is specify is replacement of paper based menus using an electronic format, the second relates to an electronic strategy for the office handling or cashiering of a customers orders. this management system, we will provide an app that can be used by the customers to order food. All

-All the users who like use the system, need create a account.

-Customers can also make payment through debit or credit card using POS which will be integrated with the management software.

-Customers can see current discount facility of the restaurant.

-Customer is able to view the menu, place orders, and organize the final bill through an smartphone.

-The food staff, whit their touch display interfacces to hte system, is able to view orders sent to the kitchen by customers.

-During preparation, the customers can see the status of each item, and can send notificacions when items are completed.

All the information about daily expenses and profit will be saved in the system, also the required information about employees will be saved in the system which can be only accessed by the system admin.

Definition, Aronyms and Abbreviations
-
| Term         | Description                                                                                       |
| ----- | ---- |
| System Admin | Is a person who is resposible for managing the whole system and who has full access to the system |
| System User  | A person who is using or operating the system but with a limited privilege.                       |
| Database     | Colecction of all the information monitored by thi system                                         |
| POS          | A point of sale system is wither a stan alone machine or a network of input and output devices used by restaurant|
| Order | Comprises one or more items |
| Item | Single serving of food |
| Customer | Restaurant patron that orders/ pays for meal |
| Chef | Staff member whose primary job is to take order |
| Account | Comprises all the meals from a user |
| Payment | Comprises the total cost of zero or more meals and zero or more tips|
| Bankcard | Customer debit/credit card |
| Menu | Surface computer representation of the available items and other options|

Overview
-
Product Perspective
-
Is the help the restaurant are more effectively and efficiently by computerizing meal ordering, billing and inventory control. The another point is generate data, after analyze the data for help the manager to make appropiate business decisions for the restaurant, for example, knowing the number of customers for a particular time interval, the manager can decide wheter more cheff are required.

Product functions
-
- Login/Logout
- Customer check menu and select the dishes he/she wants
- Place Order
- Cancel/edit order
- Chef Accept Order
- Chef mark orders complete
- Customer Select payment method
- The admin can make operation on staff Members, menu itemss and inventory.
- Customer can edit their Information
- Delivery Man Information
- Customer provide feedback


User Characteristics
-
| Actor's     | Description                                                                                       |
| ----- | ---- |
| Customer     | Can access the system through wifi connection and order food.                                     |
| Employees    | Chef.- Can the see the order and after preparing the food he will tell the system that the food is ready.                                Delivery Man.- He is in charge of taking the food to the client.                                  |
| Admin        | Can edit the price, count total earning and expenditure.                                          |

Constraints
-
- The Customer always need have connection to internet.
- Have a credit / debit card.
- Customer address must be correct

Assumptions and dependencies
-
One assumption about the software is that it will always be used on tablets or smarphones that have enough resources to run application. if the tablet does not have enough hardware resources available for the application, there may be scenarios where the application does not work as intended or not even at all

User Interface
-
Customer interface
- The customer interface will contain some screen. All the screen will have a consistent layout.

Login/Logout
- Here the user enters the data of his account to be able to enter the application

Check Menu
- In this screen, system shows a list of cards of dishes. Each dish will have an imagen, its price per serving

Edit/Cancel Order
- Aftre confitming the order, in this screen customer will be show "Edit order" and "Cancel Order" buttons.

FeedBack
-In this session the user can leave a comment, about the quality of the dish that he acquired

Hardware Interface
-
There must be a logical address of the system in IPv6 format. As well as an active database, in which all the dishes that are in the menu of the restaurant will be stored. Moreover, the central screen in kitchen which be displaying the status of order queues.

Software Interface
-
- For Databe services system shall use to MySQL
- System will run on android version above or equal to Mashmallow 6.0
- System use there must be a logical address of the system in IPv6 format

Communications Interface
-
Communication function required the internet protocol version 6 and it will follow HTTPS. It will use FTP for whole system with local server. And email communication to device of the system

Functional Requirements
-
- General use case
![alt text](https://raw.githubusercontent.com/RequirementEngineering/ch-re-JuanFuent/master/SRS.PNG)


- Use Case 1: Registrer and add informacion.

 Activity       | Description                                                                                                          |
| ----- | ----  |
| Primari Actor | User                                                                                                                 |
| Pre Condition | Internet Connection available and download the app                                                                   |
|               | 1.-The user enters their username and password, with which they registered.                                           
| Main Scenario | 2.-The system verifies the information it enters and is in charge of reapplying that it is correct.                 
|               | 3.-The user enters the data of his address, so that the delivery person knows where to take the future orders that |                   |   are made in that account.                                                                                             
|               |  4.-The information is saved in the system.                                                                          |

![alt text](https://github.com/RequirementEngineering/ch-re-JuanFuent/blob/master/UC1.PNG)

- Use Case 2: Check Menu and Place Order

 Activity       | Description                                                                                                          |
| ----- | ----  |
| Primari Actor | User                                                                                                                 |
| Pre Condition | Internet Connection available                                                                   |
|               | 1.-See the menu and select your meal. 
| Main Scenario | 2.-Select the payment method.                 
|               | 3.-Confirm Order                                                                                                    |

![alt text](https://github.com/RequirementEngineering/ch-re-JuanFuent/blob/master/UC2.PNG)

- Use Case 3: Prepare the dish

 Activity       | Description                                                                                                          |
| ----- | ----  |
| Primari Actor | Chef                                                                                                                 |
| Pre Condition | Having received an order                                                                   |
|               | 1.-Review the order 
| Main Scenario | 2.-Check if there are enough ingredients                
|               | 3.-Confirm that the order is complete                                                                                                    |

![alt text](https://github.com/RequirementEngineering/ch-re-JuanFuent/blob/master/UC3.PNG)


- Use Case 4: Bring the food to the destination

 Activity       | Description                                                                                          |
| ----- | ----  |
| Primari Actor | Delivery man                                                                                         |
| Pre Condition | Confirm that the order is complete                                                                   |
|               | 1.-Take the order                                                                                    |
| Main Scenario | 2.-Review the customer's location                                                                    |
|               | 3.-Notify that you are on your way                                                                   |                                 | 

![alt text](https://github.com/RequirementEngineering/ch-re-JuanFuent/blob/master/UC4.PNG)

- Use Case 5: Registrer and add informacion.

 Activity       | Description                                                                                                          |
| ----- | ----  |
| Primari Actor | Admin                                                                                                                |
| Pre Condition | None                                                                    |
|               | 1.-The admin has full access to the system                                          
| Main Scenario | 2.-Edit the price of dishes or make a discount                 
|               | 3.-Delete dishes or add new dishes |                   |                                                                                               
|               |  4.-Check the profits that were during the day.                                                                          |

![alt text](https://github.com/RequirementEngineering/ch-re-JuanFuent/blob/master/UC5.PNG)

Nonfunctional Requirements
-

### Performance Requirements
The system must be interactive, and the delays involved must be less. So, in every action response of the system, there are no immediate delays. In case of scrolling through the menu there should be a delay  beore the next page of menu items is displayed otherwise our people's dinning experience is affected. The order should be placed in pending orders and be visible to the head chef .

### Safety Requirements
The software is completely environmentally friendly and does not cause any safety violations. The menu will have a flexible font that can be zoomed so as to not over constrain the eyes.

### Security Requirements
The software is completely environmentally friendly and does not cause any safety violations. The menu will have a flexible font that can be zoomed so as to not over constrain the eyes.

Elicitation Process
-
The next elicitation process was carried out at a small local business called "MamaBurge's" which sells hamburgers, cakes, tacos and other snacks. Because the business is small, it was not possible to obtain much information, because in it only two people called Noé and Rogelio work, who are brothers. The information that was obtained was the following:

Juan(interviewer) .- Good afternoon, would you allow me to ask you some questions about the activities about your work and how do you do them?

Noé.-If it's okay.

Juan.-After the client makes an order by phone, what are the following processes to perform?

Noé.-First of all it is checked if there are other orders before the one that has just been made, in case the customer is notified more or less how long it could take to leave your order, also during the call is also verified that you really have the ingredients that are needed to prepare the order so that afterwards he makes the decision of whether to make a change or cancel the order.

Juan.-And how do they do it when they end up with an ingredient?

Noé.-It depends on each situation, for example there are times that we realize that is what is selling more during the day, then I can send my brother to buy things that could be finished, here in Soria. The other thing is that we can not get all the ingredients out of hand, so we decided to cancel any dish that has the missing ingredient, and we have to wait until working terms to get them and be prepared for the next day.

Juan.-And the home delivery they have, how is it?

Noé.-Ah, the truth is that we only deliver in places that are close to here, since sometimes they ask us to take the food to places a little far and then the other order may be near here, so it does not suit I'm very much going around a lot.

Juan.- Ah, well, thank you very much for helping me.

Noé.-You're welcome.

Because the orders are made per call and maybe they forgot to mention me some things, or that I also do not ask for other processes. I decided to add some things for example instead of them going to buy their ingredients they were assigned a supplier, and also some parts about the process of preparing the food.

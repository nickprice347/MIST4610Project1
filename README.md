# Team Members: 
1. Haley Ford @HaleyFord
2. Albert Sun @Glockgeta
3. Avanish Thota @avanish-thota27
4. Nicholas Price @nickprice347
5. Manafie Kabir @manafiekabir
6. Sydney Seid @sydneyseid 

## Team Name: 
61608 Group 5 
## Problem Description: 
The current scenario involves creating a relational database for a tennis club to ensure all data is properly allocated, and the business runs smoothly and efficiently. The majority of the model is centered around the entity “Members”. Members are at the forefront of the business since they determine which transactions take place, what divisions and leagues to join, what courts to reserve in conjunction with the coaches, which coaching programs to be a part of, and more. In addition to members, the club also employs a variety of general staff employees who can fulfill maintenance requests on various courts. The goal of the model is to accurately use and generate data, show the relationships between the various entities, and allow for queries to promptly be asked and solved to easily allow the analysis of data.
## Data Model: 
Explanation of our data model: 

<img width="521" alt="Screenshot 2024-03-26 at 6 04 39 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/18e904ff-8d97-43e2-bd1c-01ea7e8e6d43">

*Numbers Match Up With Our Client’s Points*
Our model is structured around a tennis club and its various entities are representative of key daily functions. The members entity is a key aspect of our model, and therefore is present in multiple different relationships. 

1. & 2.


Starting with entities one and two from our client, we created a many to many relationship between members and courts. Members can reserve many courts and courts can have multiple members present on them. The many to many relationship resulted in an associative entity, court reservations.
 
3.


Next, members can belong to many coaching programs and coaching programs have multiple members present in them. These two entities form an associative entity, sessions. Coaching programs and members may also at times have no sessions. 
Additionally, the coaching programs are led by coaches. Coaches have a one to many relationship with coaching programs, as one coach can teach many coaching programs, but a coaching program can only be led by one coach at a time. 
Additionally, the coaches entity has a one to many relationship with the court reservation entity as a coach can make multiple court reservations, but a reservation can only belong to one coach.  

4. 


Members can belong to many tennis leagues, and a tennis league is made up of many members. These two entities have a many to many relationship, which results to an associative entity divisions. 

5.


The Pro Shop Inventory entity can belong to many transactions, and the transactions can consist of multiple pro shop items. These two entities resulted in an associative entity, transaction details. 
Additionally, members can make multiple transactions from the proshop, but a singular transaction can only belong to one member. 

6. & 7.


Our general staff entity can perform maintenance on multiple courts, and each court can have multiple faculty working on its upkeep. Thus an associative entity maintenance request is created to symbolize this many to many relationship. 

## Data Dictionary: 
## Queries: Query 1 Description:

Query 1 lists the ID of the members who have not made any court reservations at the time. 

<img width="521" alt="Screenshot 2024-03-26 at 5 54 55 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/47f7dece-b48f-4a3f-bdaa-ad06b24c4806">

Query 1 allows managers to see which members have not reserved a court. This can be beneficial so that managers can inquire about if there is a reason why the member is being inactive, or if they need assistance with the reservation process. This can also be helpful for managers to determine which members they need to be marketing their services to more to increase revenues.


Query 2 Description: 

Query 2 lists the item type, the item brand, and the sum of the quantity ordered to determine the most popular item. The results are ordered by quantity ordered in descending order. 

<img width="521" alt="Screenshot 2024-03-26 at 5 56 16 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/cf362a18-f35a-4e3f-92e1-df888fe59db7">


Managers are keen on identifying which item is the most popular. Understanding which item is in high demand will allow managers to make informed decisions related to inventory management and ensure enough items are in stock for customer demand. 


Query 3 Description: 

Query 3 lists how many coaches are assigned to each age group, and the court locations where they conduct coaching sessions

<img width="521" alt="Screenshot 2024-03-26 at 5 58 39 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/d83e1b71-7565-4732-935a-b22fcfc428b7">


Proper resource allocation is critical for a business’s longevity. If there’s a higher demand for coaching sessions from a specific age group, assigning more coaches to said age group would result in improved member experience. Knowing court locations and where coaching sessions are being conducted may minimize conflicts with other club activities, thus having strategic planning over such variables will be useful for analysts to anticipate future demand and make keen decisions. 


Query 4 Description:

Query 4 lists the total transaction value for members whose individual total transaction value exceeds the average total transaction value across all members. 

<img width="521" alt="Screenshot 2024-03-26 at 5 58 56 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/a6e9d6bb-b962-4eac-b2ab-8f58672e115e">


Contemporary marketing strategies to maximize consumer loyalty and profit earnings place heavy emphasis on marketing toward the most loyal, highest-spending individuals. Such marketing tactics may include personalized promotions, discounts, or incentives that could sway loyal members to spend even more. Cultivating such strong relationships with said members, may attract new members who aspire to receive similar treatment.  








Query 5 Description: 

Query 5 lists the staff members who have more than 1 maintenance request with a “Pending” status. It lists the staff member’s ID, the location of the court, and the total number of “Pending” requests that the staff member has. 

<img width="521" alt="Screenshot 2024-03-26 at 5 59 17 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/b426d1a6-2cf6-4acc-9c1e-fd7f88373de8">


Query 5 allows the manager to see which staff members have “Pending” or uncompleted tasks. This data will show the manager if there are staff members who are not completing their work which is essential for performance reviews, and promotion decisions. This also makes sure that the manager is up to date on what still needs to be completed to ensure the right staff members are spoken to so that jobs are completed effectively and efficiently.


Query 6 Description: 

Query 6 lists the items in the pro shop’s inventory that are the brand Nike. The results are ordered in ascending order of the item price.

<img width="521" alt="Screenshot 2024-03-26 at 5 59 34 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/ecbc6969-3466-421d-9e65-4b357fdd8a9b">


Query 6 shows which items are the brand Nike. This is helpful in that the pro shop staff will be able to track the popularity of the brand and see if the brand should continue to be ordered and in what quantity. Nike is a popular brand and it is important to keep a lot in stock for members.


Query 7 Description: 
Query 7 lists the membership ID, member’s first name, and member’s last name of those who have a balance greater than the average balance of all members and became a member of the club in the year 2018. 


<img width="521" alt="Screenshot 2024-03-26 at 5 59 59 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/db473647-cdb7-440f-b987-5c21f9a0318b">

Query 7 allows management to see the financial behavior of members who joined in 2018 and compare the behavior with members who joined the club in other years. The information is useful in 


Query 8 Description:
Query 8 lists the type of item and the total sales generated by that item in the ProShopInventory.
Query 8 allows us to see which items are producing the most revenue, and therefore determine profits from that. Managers may use a query like this to determine if items or segments are worth keeping based on their profitability.

<img width="521" alt="Screenshot 2024-03-26 at 6 02 12 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/a0df748c-75f5-4ed0-95dc-301251b303fc">





Query 9 Description: 

Query 9 counts the number of members per league, including leagues with no members, the league’s ID, and the name of the league, grouped by the league.

<img width="521" alt="Screenshot 2024-03-26 at 6 03 34 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/14cda89e-c0b8-46dd-b93c-d3cc82457cff">


Query 9 could be useful for management to see what leagues are popular and can make considerations for price changes in accordance to demand. Another use case could be determining allocation of marketing funds based on leagues that would generate the most profit.



Query 10 Description:

Query 10 counts the number of members in each experience level category and groups them accordingly, this is useful for our manager.

<img width="521" alt="Screenshot 2024-03-26 at 6 04 00 PM" src="https://github.com/HaleyFord/MIST4610Project1/assets/163012596/52193a81-15a1-4f54-962f-d530a6eab987">



Query 10 could be useful for management to see what staffing needs are by looking at the experience level of members, allowing them to hire coaches that fit the needs of the members. Another use case could be figuring out what kinds of tournaments to host based on the experience level and number of players in each.



## Database Information:  
Name of our database: ns_Sp24_61608_Group5

Each query listed above is marked in the database using stored procedures. The procedures can be called using the following format: CALL TP_Qx(); (where ‘x’ is replaced by the query number)

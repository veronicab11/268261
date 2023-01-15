Fast Fashion Recommandation Systems
Veronica Boni, Gabriel Stanziola, Omar Lezar

Describe the project briefly

The aim of our project was to implement our recommendation systems for a prestigious fast fashion firm. The goal of the implementation is to increase revenues by suggesting more suitable articles for each of our clients.


 We were given three csv files: recsys_articles.csv in which we had all the information regarding each article sold in the store, a recsys_customers.csv file in which we had some information regarding the age of each customer and if the customer was either involved in fashion or part of the club or not and the last file called recsys_transactions.csv in which we had the report of all the purchases made by each customer

Brainstorming process

We were given three csv files: recsys_articles.csv in which we had all the information regarding each article sold in the store, a recsys_customers.csv file in which we had some information regarding the age of each customer and if the customer was either involved in fashion or part of the club or not and the last file called recsys_transactions.csv in which we had the report of all the purchases made by each customer

At first we wanted to take a look at the data that we had in order to structure the model in the best way possible. We choose a content filtering for the first recommendation system in which we wanted to find the similarities between the articles sold in the store. 
For the second recommendation we created a collaborative filter user-item which analyses the behavior of a customer and then compares it with those of the other customers, but we didn't take into consideration the age nor the interest of the custumer in this case since we thought the information would not have given the best recommendations. And then we merged this two filters and we created an hybrid, which we think between all these systems is the one that takes into consideration more features and therefore could give us a better result. 
<img width="547" alt="content model example" src="https://user-images.githubusercontent.com/101734080/212569602-b16522ad-3ae5-4134-86e1-4277b4941bb4.png">

<img width="556" alt="collaborative model example" src="https://user-images.githubusercontent.com/101734080/212569604-66bf73f7-daa8-48fd-a822-d6385f47657b.png">


Experimental Design

We tried different methods, we tried the K Nearest Neighbors, not only for the collaborative filtering, but also for the content, however we saw that by analyzing the features by using the .get_dummy() function we could have a simpler algorithm, but we chose carefully what kind of features we wanted by using the most suitable ones, in our opinion. For the collaborative filtering we tried also many algorithms, we tried by using the sparse matrix but the sparsity of it was equal to 0.11% which is way lower than the least it should be (0.5%). 

Results 

In the code we displayed many reccomendations and we checked than the model was working and that the reccomendations that our model gave had a logic and made sense in the first place.

here below there is the final reccomendation (using the hybrid model) for our customer with ID 4 


<img width="393" alt="hybrid model example" src="https://user-images.githubusercontent.com/101734080/212569590-0ea7f261-5665-4849-8815-26002c5de422.png">



Conclusion 

Our interest was from the beginning to create an hybrid model since we think especially for the aim of the project, which is to sell articles such as clothes and accessories it is the best one, since it takes both the content filter and the collaborative and joins them into a more efficient model. 



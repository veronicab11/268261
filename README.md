Fast Fashion Recommandation Systems
Veronica Boni, Gabriel Stanziola, Omar Lezar

[Section 1]: Describe the project briefly

The aim of our project was to implement our recommendation systems for a prestigious fast fashion firm. The goal of the implementation is to increase revenues by suggesting more suitable articles for each of our clients.


 We were given three csv files: recsys_articles.csv in which we had all the information regarding each article sold in the store, a recsys_customers.csv file in which we had some information regarding the age of each customer and if the customer was either involved in fashion or part of the club or not and the last file called recsys_transactions.csv in which we had the report of all the purchases made by each customer

[Section 2]: Brainstorming process

We were given three csv files: recsys_articles.csv in which we had all the information regarding each article sold in the store, a recsys_customers.csv file in which we had some information regarding the age of each customer and if the customer was either involved in fashion or part of the club or not and the last file called recsys_transactions.csv in which we had the report of all the purchases made by each customer

At first we wanted to take a look at the data that we had in order to structure the model in the best way possible. We choose a content filtering for the first recommendation system in which we wanted to find the similarities between the articles sold in the store. 
For the second recommendation we created a collaborative filter user-item which analyses the behavior of a customer and then compares it with those of the other customers, but we didn't take into consideration the age nor the interest of the custumer in this case since we thought the information would not have given the best recommendations. And then we merged this two filters and we created an hybrid, which we think between all these systems is the one that takes into consideration more features and therefore could give us a better result. 

[Section 3]: Experimental Design

We tried different methods, we tried the K Nearest Neighbors, not only for the collaborative filtering, but also for the content, however we saw that by analyzing the features by using the .get_dummy() function we could have a simpler algorithm, but we chose carefully what kind of features we wanted by using the most suitable ones, in our opinion. For the collaborative filtering we tried also many algorithms, we tried by using the sparse matrix but the sparsity of it was equal to 0.11% which is way lower than the least it should be (0.5%). 

[Section 4]: Results 

In the code we displayed many reccomendations and we checked than the model was working and that the reccomendations that our model gave had a logic and made sense in the first place.

here below there is the final reccomendation (using the hybrid model) for our customer with ID 4 

Recommendations for: Liliana:
3182    Kelly top
6143        Scout
3940        Osman
Name: prod_name, dtype: object
Recommendations for: S. Skinny HW Ankle Star Consc:
3687    S. Skinny HW Ankle Star Consc
4251                Shaping Skinny HW
138                 S.Skinny L.W Epic
Name: prod_name, dtype: object
Recommendations for: Woody hoodie:
2607    Frugan 2p longsleeve
2973          Vanessa 2-pack
1894                 Lee rib
Name: prod_name, dtype: object
Recommendations for: Miley LL Satin PJ  (W):
281        Alex Jogger (J)
282        Alex Jogger (J)
1503    Lindsay N-slip (W)
Name: prod_name, dtype: object
Recommendations for: Vintage Slim HW ankle consc.:
2081    Vintage Slim HW ankle consc.
5345    Embrace Slim HW ankle Consc.
6394         Loose Straight Campaign
Name: prod_name, dtype: object
Recommendations for: Highwaist 30 den 1p Tights:
6357    Fake legging NEW FIT
77       Small dot 1p Tights
85          Fake 1p Leggings
Name: prod_name, dtype: object
Recommendations for: Perrie Slim Mom Denim TRS:
308         Julia RW Skinny Denim TRS
617    Jade Trash HW Skinny Denim TRS
167         Perrie Slim Mom Denim TRS
Name: prod_name, dtype: object
Recommendations for: Pink HW barrel:
1409        DeLuca pull on TVP RW
3606               Pink HW barrel
1412    DeLuca pull on TVP RW TVP
Name: prod_name, dtype: object
Recommendations for: Jackie brief 2pk HR LS:
268                   Bra Extender
3298    Cate sless wless push body
4182     Kendall long leg biker FS
Name: prod_name, dtype: object
Recommendations for: LW (K) Rose cons rib polo:
3267          Frida push up seamless
4166      OP NEW wireless padded Rio
5595    LW (J) Mahalia Consc S-shirt
Name: prod_name, dtype: object
Recommendations for: LW (K) Rose conc rib trs:
6400       LW (K) Rose conc rib trs
5582       May Seamless Legging (J)
5589    LW (J) MAHALIA Consc Jogger
Name: prod_name, dtype: object
Recommendations for: LW (J) consc PRICE jogger:
5579     LW (J) CANDLE consc Hoodie
5591    LW (J) MAHALIA Consc Jogger
4358                  Botkyrka tank
Name: prod_name, dtype: object
Recommendations for: LW (J) Conc PRICE SWEATSHIRT:
6442     LW (J) Conc PRICE SWEATSHIRT
2381                          Hjulsta
5737    LW (J) VERONIKA Consc S-Shirt
Name: prod_name, dtype: object
Recommendations for: Liliana:
3182    Kelly top
6143        Scout
3940        Osman
Name: prod_name, dtype: object
Recommendations for: Biker shorts rib:
6357    Fake legging NEW FIT
77       Small dot 1p Tights
85          Fake 1p Leggings
Name: prod_name, dtype: object
Recommendations for: Elle Sweater Dress:
4246    Eleonor button dress
3823      Zabrina midi dress
2717             Dolly dress
Name: prod_name, dtype: object



[Section 5]: Conclusion 

Our interest was from the beginning to create an hybrid model since we think especially for the aim of the project, which is to sell articles such as clothes and accessories it is the best one, since it takes both the content filter and the collaborative and joins them into a more efficient model. 



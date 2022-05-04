<h1> Assignment 3 </h1>
<h2> Molly Cook </h2> 

<p>For my first iteration on assignment 3, I edited a few things outlined below:</p>

<h3> Count Vectorizer </h3> 
<p>I edited the count vectorizer to remove stop words, ascii accents, and characters using a regex. These are some elements I pulled from assignment 1.</p>

![image](https://user-images.githubusercontent.com/86888346/166617429-e8dc7929-554b-4320-8f8a-eab555f8e643.png)

<h3> Fit Kmeans / plt </h3> 
<p>I changed the range for the cluster number from (1, 11) to (1, 50) and applied the sample code from option 1 to plot the elbow chart.</p>

![image](https://user-images.githubusercontent.com/86888346/166617454-27265c3d-997b-4843-8804-1a4a289a4684.png)

<h3>Result</h3>
<p>Looking over the results, I did notice the model was quite successful in some ways (Ice cream, meats, and dry goods like flour were successfully clustered together) However, there were some odd clusters like a majority of fruits & veggies clustered with salmon and salsa... The model takes a very long time to run, but I think moving forward I'm going to have to resolve this odd issue.</p>
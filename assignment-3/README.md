<h1> Assignment 3 </h1>
<h2> Molly Cook </h2> 

<p>For my final iteration on assignment 3, I made the below adjustments</p>

<h3>Vectorizer </h3> 
<p>I removed the count vectorizer and returned the TfidVectorizer with an n-gram range of 1,3. The count vectorizer seemed to be making really large clusters instead of dividing them more evenly and accurately. </p>
<img width="1075" alt="Screen Shot 2022-05-10 at 8 04 37 PM" src="https://user-images.githubusercontent.com/86888346/167744211-c65015ad-5f07-433b-af03-1fd559931046.png">


<h3> Fit Kmeans / plt </h3> 
<p>I changed the range for the cluster number from (1, 11) to (1, 50) and applied the sample code from option 1 to plot the elbow chart.</p>

![image](https://user-images.githubusercontent.com/86888346/166617454-27265c3d-997b-4843-8804-1a4a289a4684.png)

<h3>Result</h3>
<p>Looking over the results, I did notice the model was quite successful in some ways (Ice cream, meats, and dry goods like flour were successfully clustered together) However, there were some odd clusters like a majority of fruits & veggies clustered with salmon and salsa... The model takes a very long time to run, but I think moving forward I'm going to have to resolve this odd issue.</p>

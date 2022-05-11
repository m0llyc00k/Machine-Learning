<h1> Assignment 3 </h1>
<h2> Molly Cook </h2> 

<p>For my final iteration on assignment 3, I made the below adjustments</p>

<h3>Vectorizer </h3> 
<p>I removed the count vectorizer and returned the TfidVectorizer with an n-gram range of 1,3. The count vectorizer seemed to be making really large clusters instead of dividing them more evenly and accurately. </p>
<img width="1075" alt="Screen Shot 2022-05-10 at 8 04 37 PM" src="https://user-images.githubusercontent.com/86888346/167744211-c65015ad-5f07-433b-af03-1fd559931046.png">


<h3> Fit Kmeans / plt </h3> 
<p>I created a range of cluster numbers and looped through them so that the model would run faster. I found that number that were closer together and a large range worked well.</p>

<img width="1089" alt="Screen Shot 2022-05-10 at 8 06 38 PM" src="https://user-images.githubusercontent.com/86888346/167744393-1976f6bf-8fb0-4423-bf75-a39ff34dc0b6.png">

<h3>Result</h3>
<p>Looking over the final results, the model did pretty well! The biggest issue I had initially was that salmon and fish products were winding up in unrelated clusters. I was finally able to get fish products out of salsa, ice cream, veggies, etc. (I think some of the adjectives like 'fresh' used to describe the fish were pretty similar to adjectives used to describe fruits and vegetables, which inevitable made salmon wind up with romaine.) </p>
<p>Here is a fish cluster:</p>
<img width="1102" alt="Screen Shot 2022-05-10 at 8 09 04 PM" src="https://user-images.githubusercontent.com/86888346/167744748-6968b483-fa6a-40b5-8487-4e8f09b3ebde.png">
<p>Here is a (separate!) salsa cluster:</p>
<img width="1106" alt="Screen Shot 2022-05-10 at 8 08 34 PM" src="https://user-images.githubusercontent.com/86888346/167744849-33f7f029-5611-44a4-a88b-c3b8db451998.png">
<p>The last trend that I noticed was that many clusters were determined by brand names rather than the contents themselves, but most brands seemed to make similar products so I don't see it as an issue. I also think from a useful perspective that it would be helpful to know the brands that have contaminated foods, given that they are the source. See example below:</p>

<img width="1090" alt="Screen Shot 2022-05-10 at 8 10 19 PM" src="https://user-images.githubusercontent.com/86888346/167745115-5898f8b3-f22f-4e26-bf15-a39c2441e55c.png">

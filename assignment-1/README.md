<h1>Assignment 1 - Movie Review Sentiment Analysis - Molly Cook</h1>
<p>My first approach to this assignment was to add features and see if I could find a pattern there. I added a myriad of different features, as seen below, but decided to only implement 2 features. I removed the 2 existing features and used 'caps_count' and 'quotes_count'. The caps feature finds more that 2 capital letters in a row and the quotes count feature splits the spring by a quotation to find the count. To be honest, I didn't find a ton of success with many of the features and perhaps with a little more conscious tinkering I could have used better feautres. </p>

![image](https://user-images.githubusercontent.com/86888346/156940755-419bc2e2-ab39-4dad-8a9b-bcdbbf16744d.png)

<p>The next thing I did was I changed the hashing vectorizer to a count vectorizer so that I could use an n-gram and find word groupings rather than just single words. I am extracting 2-grams of words in addition to the 1-grams of individual words.This seemed to improve all the modules a bit, with the few models that were close to perfect (SVM, logistic regression, Naive Bayes, Perceptron, and Ridge Regression Classifier) now having 100% precision and accuracy.  </p>

![image](https://user-images.githubusercontent.com/86888346/156941285-75cba720-a166-45eb-a79f-510f48d76db6.png)
![image](https://user-images.githubusercontent.com/86888346/156941686-5a88442e-1c17-4e86-8061-5d16bb2552aa.png)



<p>The OLS model gave me some issues and typically would always come out with 48-50% precision and accuracy. I was able to improve this a bit with about 52% accuracy and 54% precision. The amount of false positives and true positives was greatly reduced congruently. </p>

<p>The last thing I did was use stop words, which seemed to lower the quantity of true positives and fasle positives of the OLS model, but not necessarily improve accuracy or precision. I made some attempts in using LemmaTokenizer but wasn't fully convinced that I was using it properly, so I got rid of it</p>

<h2>Before:</h2>

![image](https://user-images.githubusercontent.com/86888346/156941674-6b61475d-a21b-4acf-96a2-8898808e2aa9.png)


<h2>After:</h2>

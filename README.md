<h1> Acquisition Prediction using Social textual data and company profiles </h1>

<p>Acquisition prediction deals with choosing proper target companies for the bidder company, and is an important and challenging task. </p>

<p>Acquisition prediction is the critical step that makes assessments on each company about its chance of being acquired, which will facilitate both parties to develop the best strategies.</p>

<h2> Data Collection </h2>

<p><strong> Web crawlers </strong> are used to scrap data from techblogs, and investors forum. The collect data in a automated way and store it a local files </p>

<p> Web crawling package used - <a href="http://scrapy.org/"> scrapy </a></p> 

<p><strong> Data Manipulation </strong>is done transform the unstructured data to structured form, performed using <a href="http://pandas.pydata.org/">Pandas</a></p>

<h2> Textual data processing </h2>

<p>Text document data must be converted to a vector represtation, for it to be used by a classifier. </p>

<a href="https://radimrehurek.com/gensim/models/doc2vec.html">Doc2Vec</a> is used to convert the documents to vectors. Doc2Vec works by building paragraph vector (<a href="https://cs.stanford.edu/~quocle/paragraph_vector.pdf">reference</a>) which works well for variable length textuals inputs ranging from sentences to paragraph </p>
<p>Doc2Vec algorithm is made accessible by an amazing one-stop python package for text mining <a href="https://radimrehurek.com/gensim/">gensim</a></p>

<h2> Prediction </h2>

<p>Neural networks are used to handle the classification task, due to the high-dimensionality of the dataset (simple Logistic regression is also performed for comparison) </p>
<p>The Neural network is built using a python package, which makes lightning fast mathematical computaion by leveraging the GPU, <a href="http://deeplearning.net/software/theano/"> Theano </a> </p>

<h2> Result </h2>

<p>The results are close to reality, the model accurates captures the acquisition trends going on in the food delivery and real estate industries, but is far from perfect.
One of the limitations of the model is, it cannot differentiate the context between a company that is getting acquired and the company that acquires it. </p>

<h3>Improvements to be done </h3>
<ul>
<li>Get quality company profiles from database providers like CrunchBase, Owler </li>
<li>Try a bespoke random forest classifier with feature engineering </li>

 

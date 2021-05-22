Recommender systems have become widespread in various Internet services: contextual advertising, films and music of interest to the user, selection of goods and services in online stores. Algorithms for constructing recommendations take into account the user's profile, the history of his requests, purchases, and information about users who are similar to him. These algorithms are developing rapidly and have proven their effectiveness, their implementation increases service traffic and sales. A new area of application for recommender systems is healthcare. Over the decades, huge amounts of medical data have been accumulated, such as case histories, mortality and morbidity rates, treatment protocols, and even health data continuously taken from a person by special sensors. Intelligent systems are being developed for diagnosing diseases, choosing a method of treatment, and tracking the daily health of a person. The article provides a general introduction to recommender systems, a review of the literature on the use of recommender systems in health care, and also discusses the problem of building recommender systems to optimize hospital purchases.


The central aspect in building a recommender system is the choice of the algorithm. The use of one or another algorithm is conditioned by the initial data, their dimension and the context of the recommendations. This part will describe the main algorithmic approaches to the construction of recommender systems.
The collaborative filtering method is based on individual user ratings. The method tries to predict the most relevant item for the user using a rating matrix. Typically, the rating matrix is sparse. There are various ways to fill in the blanks in the matrix that can be used as guidelines. So the main algorithms  that helping make our objective to real are numpy reciprocal for calculating euclidean distance, fidfVectorizer for vectoring strings

Management in biomedical systems
The simplest are the Memory-based Collaborative Filtering correlation models. Their features are storing the entire rating matrix and measuring the similarity between objects and users by correlating the rows and columns of the matrix. To fill in the gaps in the data, you use nonparametric regression for users or for features. Correlation methods are intuitive and easy to implement. The main disadvantages of correlation methods are the problem of cold start and the need to store a huge sparse rating matrix. Latent models are free from these disadvantages.
In our system we have used 'Item-Based','Item/Price-Based','Item/Price/Brand-Based' inMaxScaler as preprocessing.  
To increase the productivity of the methods, latent models of collaborative filtering are used. The rating matrix is used to evaluate the user profile and the profile of objects, which have a significantly lower dimension than the initial data. Latent models can be based on co-clustering, probabilistic approach, and matrix decompositions. Singular value decomposition of matrices is most often used.

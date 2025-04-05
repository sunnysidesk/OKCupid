# Match Made in ML - A Profile Matching Algorithm

This machine learning project was produced by a team of three as part of the graduate Machine Learning course at UC Davis. Named 'Match made in ML', it explores the use of AI in online dating by leveraging Facebook AI Similarity Search (FAISS) with cosine similarity to match dating profiles from the publicly available OKCupid dataset. We implemented three methods: a baseline Cosine Similarity model, a FAISS-based model, and an optimized Weighted FAISS model tuned via grid search and cross-validation. Our grid search identified the best weight combination (Essay=2.0, Features=0.5, Numerics=0.5) with improved performance metrics, achieving a MAP of 0.7699 and an MRR of 0.9838. These results demonstrate that our optimized Weighted FAISS model provides high ranking quality and efficiency—key factors in making meaningful connections in online dating.

Our approach used FAISS with cosine similarity enhanced by a weighted feature combination optimized through grid search and cross-validation. Our experiments indicate that by prioritizing essay embeddings, our Weighted FAISS model outperforms baseline methods in key ranking metrics (MAP and MRR) while maintaining reasonable diversity. Through this project, we realised the importance of achieving balance between ranking quality, diversity and efficiency, as well as the fact that choosing the best model also depended on the project priority. Realistically, when a user is shown potential matches, the order matters significantly, meaning if highly compatible matches appear lower in the list, users might stop scrolling before reaching them, were this algorithm implemented in a dating application. This led to the conclusion that weighted FAISS is the best model to leverage, also having feature-engineered user profile features to weigh personality-enhancing features higher. This project highlights the potential of leveraging advanced similarity search techniques in the competitive space of online dating with a focus on most relevant matches ranking higher, paving the way for more intelligent and personalized matchmaking systems.

Read the full project report [here](report/Project_Report)  
View the preprocessing approach [here](preprocessing/EDA_&_preprocessing.ipynb)  
View the modelling approach [here](modelling/okcupid_Matching.ipynb)  

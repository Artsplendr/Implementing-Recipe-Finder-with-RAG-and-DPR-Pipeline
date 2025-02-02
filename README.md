# Implementing Recipe Finder

#### The goal of this repository is to implement Recipe Finder Assistant, by using two different approaches:

#### The first notebook
implements personalized Recipe Finder, that retrieves and adapts recipes based on user queries using FAISS for similarity search and GPT-4 for generating refined recipes.

#### The second notebook
implements personalized Recipe Finder with a Retrieval-Augmented Generation (RAG) + Dense Passage Retrieval (DPR) pipeline. It leverages DPR encoders to generate embeddings for a dataset of recipes, which are stored in a FAISS index for efficient retrieval. When a user submits a query, the system retrieves the most relevant recipes using FAISS and a DPR-based similarity search. The top-ranked recipes serve as context for a generative model (facebook/bart-large), which refines or adapts the recipe based on the user’s preferences.

#### References
The dataset of recipes, used in this project, is available at this [link](https://raw.githubusercontent.com/tabatkins/recipe-db/master/db-recipes.json).

#### If you found this repository helpful, drop it a &#11088; :)!

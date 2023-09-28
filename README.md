# Beer-Recommender-System
In order to explore potential differences among popular beer brands based on consumer perceptions, I collected approximately 6000 reviews from a beer review forum. I conducted the following analysis to create a recommendation system that generates a list of beer brands aligning with consumer preferences.

* Data Preprocessing: I began by cleaning the scraped reviews. Brands with fewer than 50 reviews were filtered out, and stopwords were removed for further analysis.

* Exploratory Data Analysis: To identify the most frequently discussed attributes related to beer, I calculated word frequencies. Similar attributes were grouped together by replacing them in the reviews. Additionally, I performed LIFT analysis to uncover associations between beer brands and attributes, assessing any notable differences among brands.

* Building the Recommendation System: I employed two methods to construct the recommendation system. The first method combines VADER sentiment analysis with Bag of Words cosine similarity. The second method relies solely on cosine similarity, utilizing Spacy word embeddings.

Each method has its advantages and limitations. Bag of Words cosine similarity is effective when dealing with rare words and seeking an exact match. Conversely, when dealing with words that convey broader meanings, word embeddings offer a more comprehensive word space, resulting in improved matches.

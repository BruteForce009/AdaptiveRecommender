# Adaptive Recommender
A recommendation system that can suggest personalized news articles or blog posts to users based on their reading history and interests. Utilizes the News Category dataset containing around 210k news headlines from HuffPost, which has been cleaned and pre-processed. It is based on content-based filtering, which recommends articles
based on their similarity to a given article. This system will be able to learn and adapt to the user's preferences over time and provide relevant and engaging content.
<br/><br/>

### Content-based filtering
Content-based filtering uses item features to recommend other items similar to what the user likes, based on their previous actions or explicit feedback. First a similarity metric is constructed. Then, the system scores each candidate item according to this similarity.
For a simple example, let <b>X</b> and <b>Y</b> be the two binary vectors. Since <b><X, Y> = Σ<sub>i</sub>X<sub>i</sub>Y<sub>i</sub></b>, a feature appearing in both <b>X</b> and <b>Y</b> contributes a 1 to the sum. It is the number of features that are active in both vectors simultaneously. A high dot product then indicates more common features, thus a higher similarity.
![blog9_img1](https://user-images.githubusercontent.com/57285244/234851528-653313af-c90d-4a2d-b4d6-8b18bf9ee38c.png)

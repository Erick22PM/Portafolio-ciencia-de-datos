# Professional Portfolio Documents — Erick Pérez Mendoza

This repository contains a curated collection of project reports, technical documents, and final deliverables focused on Data Science, Machine Learning, Data Engineering, Natural Language Processing, Computer Vision, and AI-powered analytical systems.

Each project document summarizes the problem statement, dataset description, methodology, feature engineering process, models used, results, limitations, and conclusions.

## Projects

### 1. Predictive Analysis of Sleep Quality

This project focuses on analyzing sleep quality through demographic, health, lifestyle, physical activity, screen usage, and medical variables. The objective was to study the factors associated with good or poor sleep quality through data preprocessing, exploratory data analysis, feature engineering, multicollinearity analysis, and analytical dataset construction.

The dataset includes 20,000 records and 26 numerical, categorical, and boolean variables related to sleep habits, physical and mental health, activity patterns, substance consumption, screen exposure, and ocular health.

**Main techniques applied:**

- Data cleaning and preprocessing.
- Exploratory Data Analysis.
- Feature engineering.
- Variable discretization.
- Multicollinearity analysis.
- Weight of Evidence and Information Value.
- Analytical dataset construction.
- Dashboard development for data visualization.

**Document:** [`01_Predictive_Analysis_Sleep_Quality.pdf`](./01_Predictive_Analysis_Sleep_Quality.pdf)

---

### 2. Reggaetón Mexa: Hits of the Future

This project analyzes the success of Mexican reggaeton songs on digital streaming platforms such as Spotify and Deezer. The main objective was to identify musical, lyrical, temporal, and structural patterns associated with song popularity and to build predictive models capable of estimating a song’s potential performance.

The project integrates data from Spotify API, Genius API, Deezer API, and audio analysis with Librosa. The dataset includes more than 2,000 songs and hundreds of engineered variables related to popularity, lyrics, explicit content, ranking, tempo, rhythm, release dates, and audio characteristics.

**Main techniques applied:**

- Data extraction from public APIs.
- Lyrics cleaning and text processing.
- Audio feature extraction.
- Exploratory Data Analysis.
- Feature engineering.
- Predictive modeling.
- Supervised regression.
- Model evaluation with R², MAE, and RMSE.
- Analytical dataset construction.

**Results:**

Several regression models were tested. Traditional linear models showed limited performance, while an MLPRegressor achieved a moderate predictive capacity with an R² close to 0.42. The project also identified data quality challenges caused by inconsistencies, missing values, and noise from public API sources.

**Document:** [`02_Reggaeton_Mexa_Hits_of_the_Future.pdf`](./02_Reggaeton_Mexa_Hits_of_the_Future.pdf)

---

### 3. Movie Posters: Visual Style Classification and Similarity Search

This computer vision project focuses on identifying visual and artistic patterns in movie posters. The goal was to classify and group movie posters according to shared visual characteristics and to find posters that are visually similar to each other.

The dataset was built using The Movie DB API and includes information such as movie title, poster image, ID, and release date. It contains more than 14,000 movies from 1950 to the present. Each poster was converted into a 512-dimensional visual embedding using OpenAI’s CLIP model.

The project applied dimensionality reduction and clustering techniques to explore the visual structure of the dataset. PCA was used to reduce the embeddings from 512 to 50 dimensions, followed by t-SNE for 2D visualization. DBSCAN was then applied to identify visual groups or artistic currents. A k-distance curve was used to select the DBSCAN inflection point, with an epsilon value around 0.64.

**Main techniques applied:**

- Data extraction from The Movie DB API.
- Image processing.
- Visual embeddings with CLIP.
- Vector representation of movie posters.
- Dimensionality reduction with PCA.
- 2D visualization with t-SNE.
- Unsupervised clustering with DBSCAN.
- K-distance curve analysis.
- Visual style identification.
- Similarity search using cosine similarity.

**Results:**

The analysis identified approximately 30 visual groups or artistic currents. Some clusters corresponded to recognizable poster styles such as anime, horror, franchise-based visual identities, and unique posters classified as noise due to their distinctive visual style. The project also implemented a recommendation approach based on cosine similarity to retrieve posters visually similar to a reference poster.

**Document:** [`03_Movie_Posters_Visual_Styles.pdf`](./03_Movie_Posters_Visual_Styles.pdf)

---

### 4. Hybrid Sticker Recommendation and Classification System

This deep learning and computer vision project focuses on improving sticker discovery and recommendation in messaging applications. The system uses the `nyuuzyou/stickers` dataset, which contains hundreds of thousands of stickers associated with emoji labels.

The project was structured in three main phases: supervised sticker classification using a convolutional neural network, visual embedding extraction with CLIP, and a hybrid recommendation system based on visual similarity, emotional context, and text analysis.

**Main techniques applied:**

- Convolutional Neural Networks.
- Multiclass image classification.
- Image preprocessing.
- Visual embeddings with CLIP ViT-B/32.
- Cosine similarity.
- Dimensionality reduction with PCA and t-SNE.
- Unsupervised clustering with DBSCAN.
- Hybrid recommendation system design.
- Dataset imbalance analysis.
- Evaluation of technical limitations and ethical considerations.

**Results:**

The supervised CNN model showed limited performance due to the high complexity of the multiclass problem, with approximately 1,276 emoji classes. However, CLIP embeddings proved more effective for visual similarity-based recommendations. The project concluded that embedding similarity is a more viable approach than traditional classification for this type of visual recommendation system.

**Document:** [`04_Hybrid_Sticker_Recommendation_System.pdf`](./04_Hybrid_Sticker_Recommendation_System.pdf)

---

### 5. StoryIA: AI Assistant for Script Writing and Storytelling Analysis

StoryIA is a multimodal AI project designed to help TikTok content creators improve their scripts, thumbnails, hashtags, and narrative structure. The platform analyzes textual, visual, and quantitative elements to estimate the potential success of a short-form video and generate actionable recommendations.

The system combines Natural Language Processing, Computer Vision, semantic embeddings, supervised learning, unsupervised clustering, and generative AI. It was integrated into an interactive Streamlit platform where users can upload a script and thumbnail, receive a full analysis, get narrative recommendations through a chatbot, and generate audio using synthetic voice.

**Main techniques applied:**

- TikTok data scraping.
- Transcript and description processing.
- Language normalization and translation.
- Narrative feature extraction.
- Text embeddings.
- Visual thumbnail analysis with CLIP.
- Unsupervised clustering with HDBSCAN.
- Viral performance classification.
- Narrative score regression.
- Streamlit application development.
- Chatbot integration for narrative feedback.
- Multimodal AI system design.

**Results:**

The project built a weighted narrative score based on likes, comments, and shares. It also identified visual and narrative clusters across different creators and developed supervised models to classify videos into low-performance, normal-performance, and viral categories. The final platform serves as an AI-powered assistant for creators who want to optimize storytelling content using data-driven insights.

**Document:** [`05_StoryIA_AI_Script_Assistant.pdf`](./05_StoryIA_AI_Script_Assistant.pdf)

## Technical Areas Covered

- Data Science.
- Machine Learning.
- Deep Learning.
- Data Engineering.
- Exploratory Data Analysis.
- Natural Language Processing.
- Computer Vision.
- Recommendation Systems.
- Text and image embeddings.
- Supervised and unsupervised learning.
- Feature engineering.
- Predictive modeling.
- Dashboards and interactive applications.
- AI-powered creative tools.

## Repository Structure

```text
professional-portfolio-docs/
├── README.md
├── 01_Predictive_Analysis_Sleep_Quality.pdf
├── 02_Reggaeton_Mexa_Hits_of_the_Future.pdf
├── 03_Movie_Posters_Visual_Styles.pdf
├── 04_Hybrid_Sticker_Recommendation_System.pdf
└── 05_StoryIA_AI_Script_Assistant.pdf

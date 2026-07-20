👕 AI-Powered T-Shirt Recommendation using CLIP & LLaVA
📖 About the Project

This project was developed as part of my AI internship to solve a Multimodal Product Choice Personalization problem. The goal was to recommend T-shirts based on a user's previous visual preferences rather than relying only on product descriptions or keywords.

The recommendation system learns from a user's historical choices, identifies visual patterns using Vision-Language Models, and recommends similar products from a new collection. Along with recommendations, the system also generates natural language explanations for why a particular T-shirt is suggested.

During the internship, I continuously improved the implementation by experimenting with different approaches, studying research papers, and comparing multiple recommendation techniques before arriving at the final workflow.

🎯 Problem Statement

The objective of this project is to build an AI-powered recommendation system that can:

Learn a user's visual preferences from previously selected T-shirts.
Recommend the most relevant products from a new dataset.
Explain the reason behind each recommendation using a Vision-Language Model.
Explore different machine learning approaches to identify the most suitable recommendation pipeline.
🚀 Project Development Journey

Instead of directly implementing the final solution, the project was developed in multiple stages. Every day, new ideas and improvements were added based on observations, experiments, and discussions.

Approach 1: CLIP + LLaVA

The first implementation focused only on CLIP and LLaVA.

CLIP was used to extract visual embeddings from T-shirt images.
Similarity between historical preferences and new products was calculated using CLIP embeddings.
LLaVA was then used to generate explanations describing why the recommended T-shirt matches the user's preferences.

This approach helped understand how Vision-Language Models can perform image-based recommendation without training a separate classifier.

Approach 2: CLIP + LLaVA + Logistic Regression

After the initial implementation, the recommendation pipeline was extended by adding Logistic Regression.

In this approach:

CLIP extracted image embeddings.
Logistic Regression learned the user's preferred and non-preferred patterns.
Products were ranked according to their predicted preference scores.
LLaVA generated human-readable explanations for the final recommendations.

This experiment introduced supervised preference learning into the recommendation system.

Approach 3: CLIP + LLaVA + K-Nearest Neighbors (KNN)

To compare another recommendation strategy, KNN was also implemented.

In this version:

CLIP generated visual embeddings.
KNN identified products that were visually closest to the user's preferred items.
The nearest matching products were recommended.
LLaVA explained the reasoning behind each recommendation.

This allowed comparison between similarity-based recommendation and classifier-based recommendation.

📚 Research Papers Studied

Before implementing the models, I explored research papers related to Vision-Language Models to better understand their working principles.

The papers mainly focused on:

CLIP (Contrastive Language–Image Pretraining)
LLaVA (Large Language and Vision Assistant)

Reading these papers helped me understand concepts such as image-text representation learning, multimodal understanding, zero-shot learning, visual reasoning, and explainable AI, which guided the implementation throughout the project.

🤖 Understanding LLaVA

LLaVA is a Vision-Language Model that combines image understanding with natural language generation. Unlike traditional image classification models, it can understand visual content and provide detailed textual responses.

In this project, LLaVA was used to explain why a recommended T-shirt matches the user's historical preferences, making the recommendation system more interpretable and user-friendly.

🌟 Applications of LLaVA

During the literature review, I also explored some popular real-world applications of LLaVA.

1. Visual Chatbot

LLaVA can interact with users by answering questions related to an image and carrying out image-based conversations.

2. Visual Question Answering (VQA)

LLaVA can analyze an image and answer questions such as identifying colors, objects, clothing styles, or other visual details present in the image.

💡 Key Learning

Throughout this project, I gained practical experience with Vision-Language Models, multimodal recommendation systems, preference learning, CLIP embeddings, Logistic Regression, KNN-based recommendation, prompt engineering, and explainable AI. I also learned how to read and understand research papers and gradually improve a project through continuous experimentation and implementation.

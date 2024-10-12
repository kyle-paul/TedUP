# TedUp
[![> Video Demo](https://img.shields.io/badge/Video%20Demo-blue)](https://www.youtube.com/watch?v=EkW7s3Nhtyc)

## Feedback from 2nd Round before national round
- UI is relatively dark $\rightarrow$ New clean minimal and more friendly UI 
- Virtual Therapist is not suitable $\rightarrow$ TedUp (TedupBot, TedupBlog, TedupPod)
- Focus in the target audience (competitive advantage over Woebot and Wysa) $\rightarrow$ Released Vietnamese version for the chatbot, progess recorder, blogs, and podcasts
- Leak of user information when the system uses info to analyze for the team to take action $\rightarrow$ Connect database between app and web for user can login and accept the term and condition 
- Categories for blog $\rightarrow$ 5 main categories and tags for each blog
- Community building $\rightarrow$ reactions, comments, bookmarks
- What's new?
    - Hybrid Recommender System = Neighborhood Collaborative Filtering + Content-based Filtering (with the help of Tags)
    - Cold Start problem $\rightarrow$ solved 
    - New playlists of podcasts
    - Synced Database between App function and Web function (Bot can query the content from blogs to give advice to user)


## Abstract & introduction

Adolescents are facing various challenges to their mental health due to their exposure to online risks and pressures, such as cyberbullying, misinformation, social comparison, and unrealistic expectations. They also have to deal with the stress and anxiety from their academic and personal lives, which can affect their self- esteem and well-being. These factors can lead to negative emotions and behaviors, such as depression, isolation, self-harm, and substance abuse. Teenagers are reluctant to ask for help because of the stigma around mental health disorders, and there are also additional limitations including waiting lists and geographic restrictions. There is a significant gap in the treatment that should be available conveniently and cost-effectively, and the services available at hand. The ratio of therapists, psychiatrists, psychiatric social workers and mental health nurses to patients is 1: 10,000, even in developed countries (Kislay, 2020). The disparity in the system means that most people with menta health problems will never get the support the need. In response, we developed a technology-based application that provides online support and guidance to adolescents with mental health
problems.

## Approach

The application uses natural language processing and artificial intelligence to interact with users in a conversational manner, and offers a toolbox of features to help them cope with stress, anxiety, depression, and other challenges. The application also integrates mental health assessment tools to monitor the users’ progress and provide

feedback. We assume that technology-based applications can be a viable and scalable alternative to face-to-face mental health services for adolescents. Our solution consists of four main components:

- A general emotion classifier that can categorize the user’s story (diary) into positive, negative, or neutral emotions, based on a deep neural network with bidirectional LSTM (BiLSTM) architecture. We evaluated our solution using a self-scraping dataset of online diaries from various websites. We compared different architectures and models for each component and selected the best ones based on their accuracy and performance.
- A complex emotion classifier that can further classify the user’s story into 12 fine-grained emotion categories, such as anger, sadness, remorse, fear, depression, lonely, joy, love, optimism, gratitude, and pride. This component uses a transfer learning approach with BERT pretrained model to achieve better performance. The results from this step are then used to quantify the user’s mental health quality based on a our mathematical formula.
- A chatbot that can respond to the user’s story with empathetic and supportive messages, and suggest some practical solutions to help them cope with their negative emotions and improve their well-being.
- We have a time series analysis model that can predict the user’s future emotional trends based on their past diary entries. This component can help the user monitor their progress and identify potential risks or opportunities for intervention. (This feature need time to be improved)
- Finally, there is a recommender system using neighbourhood collaborative filtering to suggest the best=fit blogs that can solve problems for users in a personalized way.

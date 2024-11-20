---
title: "Deep Learning-based Query-Response System for Farmers"
description: "IIT Indore"
startDate: "July 2022"
endDate: "Jan 2023"
heroImage: "/people-talking-planter.webp"
---

The project, titled "Kisan Query Response System (KisanQRS)," addresses the crucial need for timely and accurate information delivery to farmers in the agricultural sector. The traditional approach of relying on call centre agents for query resolution often leads to inconsistent quality and delayed responses. In response, KisanQRS offers a robust query-response framework based on Deep Learning techniques, aiming to provide prompt and pertinent responses to farmers' queries.

KisanQRS employs a multi-step approach to process and respond to farmers' queries efficiently. Firstly, it integrates semantic and lexical similarities of queries to identify and group similar queries using a rapid threshold-based clustering method. Before clustering, data cleaning techniques are applied, such as the removal of special characters and extra white spaces, enhancing the accuracy of clustering. Moreover, the removal of crop names from queries facilitates clustering regardless of the specific crop mentioned.

After clustering, a query mapping module is trained using an LSTM-based Deep Learning model to accurately map queries to relevant clusters. This LSTM model is chosen for its ability to handle the sequential structure and long-term dependencies inherent in textual data. Subsequently, an answer retrieval method is employed, which clusters candidate answers for each crop, ranks these answer clusters based on the number of answers, and selects the leader of each cluster to provide the top-K answers.

The project utilizes a dataset comprising a subset of 34 million call logs from the Kisan Call Centre (KCC), operated by the Government of India. Performance evaluation of the query mapping module and answer retrieval method is conducted on data from five major states of India, consisting of 3,00,000 and 10,000 samples, respectively. The results demonstrate the superior performance of KisanQRS, achieving a top F1-score of 96.58% for query mapping and a competitive NDCG score of 96.20% for answer retrieval.

The contributions of the project include the introduction of KisanQRS, a novel query-response system tailored for the agricultural domain. It offers a fast and efficient query clustering approach based on semantic and token-wise similarities, coupled with an LSTM-based query mapping module for accurate cluster labeling. Additionally, the project proposes a novel answer retrieval method, demonstrating high effectiveness in retrieving relevant answers.

Practical implications of KisanQRS include providing farmers with a reliable, data-driven response system for their daily agricultural queries, thereby enhancing decision-making and awareness of best practices. The platform could also be integrated into voice-assisted chatbots to accommodate digitally under-skilled farmers. Moreover, call centre workers can leverage this system to access information swiftly and accurately, improving query resolution efficiency.





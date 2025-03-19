---
title: "Multimodal Sarcasm Detection"
description: "University of Groningen"
startDate: "May 2023"
endDate: "July 2024"
heroImage: "/multimodal.webp"
---

<div class="bg-gray-100 p-2 rounded-md inline-block">
  <a href="https://ieeexplore.ieee.org/abstract/document/10887864" class="text-black-500 underline hover:text-blue-700" target="_blank">
    Publication
  </a>
</div>

In this project, a novel multimodal approach is proposed to enhance the accuracy of sarcasm detection by addressing key challenges posed by emotional incongruities and modality-specific relationships. The core innovation lies in the integration of Graph Attention Networks (GATs) to capture intra-modal dependencies and a Cross-modal Contrastive Attention Mechanism to identify emotional incongruities between modalities (text, audio, video). Sarcasm often hinges on the contrast between expressed and implied emotions, which may not always be explicitly conveyed within a single modality. Thus, the framework models these incongruities through pair-wise comparisons of emotional features across different modalities to accurately detect sarcasm.

To address the problem of data scarcity, the proposed method employs advanced data augmentation techniques: it uses a lip synchronization strategy (Wav2Lip) to adjust the speaker's lip movements to match the augmented audio, which is generated using fine-tuned Fast Speech 2. The audio is derived from augmented text samples, which are generated through few-shot prompting with GPT-4o. 

Features are extracted using pre-trained and fine-tuned (for emotion recognition) models: BERT for text, Wav2Vec2 for audio, and Vision Transformers (ViT) for video, to extract the raw and emotion feautures, respectively. Additionally, the framework utilizes supervised contrastive learning to create discriminative embeddings, pushing the model to better differentiate between sarcastic and non-sarcastic instances.

The method constructs graphs for each modality (text, audio, video) with nodes representing d-dimensional feature vectors. Highly similar nodes are connected, emphasizing strong intra-modal relationships. Then, these graphs are processed through Graph Attention Networks (GAT) to learn dependencies within each modality, producing modality-specific embeddings that are fused through collaborative gating.

To capture emotional incongruities between modalities, the contrastive attention mechanism normalizes and aligns emotion features from each modality into a common embedding space. Then, it generates opponent attention weights to highlight discrepancies, which are used to create contrastive matrices that capture modality-specific emotional differences.

Finally, the embeddings from the previous steps are combined and refined using supervised contrastive learning. This encourages the model to differentiate between sarcastic and non-sarcastic instances, with a final classifier trained to predict the emotion based on the learned features.

The proposed framework demonstrates a significant performance improvement over existing methods, achieving a macro F1 score of 74.96% on the MUStARD++ dataset, outperforming prior state-of-the-art by 1.6%.
---
title: "Semantic Comprehension of Multimodal Content"
description: "IIT Indore"
startDate: "Feb 2023"
endDate: "Oct 2023"
heroImage: "/mm-orient.webp"
---

<div class="bg-gray-100 p-2 rounded-md inline-block">
    <a href="https://github.com/devraj-raghuvanshi/MM-ORIENT" class="text-black-500 underline hover:text-blue-700" target="_blank">
    [GitHub]
  </a>
</div>

This project addresses the challenge of acquiring efficient multimodal representations for various tasks while mitigating the influence of noise inherent in monomodal features. Traditional multimodal learning methods often employ complex fusion techniques to merge features from different modalities, potentially overlooking discriminative information within monomodal features and propagating noise in the resulting multimodal representations.

To overcome these challenges, we propose a novel framework that acquires multimodal representations in a cross-modal manner without requiring explicit interaction between different modality representations at the latent stage. The approach utilizes cross-modal relation graphs to reconstruct monomodal features, wherein nodes represent features of one modality and edges are established based on features of another modality. This method effectively reduces noise propagation in multimodal features while comprehending high-order relationships between modalities.

Additionally, a Hierarchical Interactive Monomodal Attention (HIMA) mechanism is introduced to enhance multitasking capabilities. HIMA operates in two stages, generating region-based and word-level attention vectors on individual modalities before creating a unified representation for the multimodal content. This attention mechanism helps extract discriminative information from individual modalities before late-fusing them to generate a joint representation.

Moreover, the framework leverages generative AI-based large language models (LLMs) for text augmentation, enhancing the performance of the framework. By incorporating task-specific text features in the final representation, our model effectively comprehends multimodal content for multiple tasks, including sentiment analysis, sarcasm detection, and hate speech detection.





The proliferation of abusive language on digital platforms poses a significant threat to user
safety, mental well-being, and the integrity of online discourse. While automated
moderation systems have made strides in detecting toxic content, most existing models are
monolingual and struggle with code-switching, transliteration, and linguistic diversity.
This project addresses the urgent need for a robust, multilingual abusive language detection
system capable of handling noisy, mixed-script inputs across English, Telugu, and
Malayalam.
To overcome the limitations of traditional approaches, we propose a phoneme-aware fusion
architecture that integrates semantic and phonetic representations. The system leverages
XLM-Roberta for multilingual text encoding, a Transformer-based phoneme encoder for
phonetic feature extraction, and a cross-attention fusion module to align and combine both
modalities. An adapter layer refines the text embeddings, while auxiliary tasks such as
language identification and embedding reconstruction enhance generalization. The model
is trained using a composite loss function comprising focal binary cross-entropy, cross-
entropy, and mean squared error, with adversarial robustness introduced via Fast Gradient
Method (FGM).
Experimental results demonstrate the effectiveness of the proposed system, achieving
90.4% accuracy, 84.16% precision, 100% recall, and an F1 score of 91.40 on the test set.
The ROC curve yields an AUC of 0.98, indicating excellent discriminative capability.
Confusion matrix analysis confirms perfect sensitivity, with no abusive samples missed.
These findings highlight the model’s suitability for real-world deployment in content
moderation pipelines, especially on platforms serving linguistically diverse communities.
By combining phonetic awareness, cross-modal fusion, and adversarial training, the system
offers a scalable and inclusive solution for detecting abuse across languages, scripts, and
cultural contexts.

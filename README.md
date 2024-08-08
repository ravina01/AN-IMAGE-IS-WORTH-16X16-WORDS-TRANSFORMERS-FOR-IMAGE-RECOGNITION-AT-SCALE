
# AN IMAGE IS WORTH 16X16 WORDS: TRANSFORMERS FOR IMAGE RECOGNITION AT SCALE

### Let's Summarize the paper -

- itroduces the ViT, a model for image recognition that applies the transformer architecture, to computer vision tasks.

1. ViT - It proposes a method to use transformers for image recognition by splitting an image into patches(16 x 16), treating these patches as token (words) similar to those in NLP, and feeding then into a transformer model.

2. Model Architecture - Each image is divided into a sequence of fixed size non-overlapping patches, linearly embedded, and then fed into a standard transformer encoder.  A class token is added to the sequence of embeddings, which eventually holds the representation used for classification.

3. Training and Performance: ViT models are pre-trained on large datasets (like JFT-300M) and fine-tuned on smaller datasets (like ImageNet). The paper demonstrates that with sufficient pre-training, ViT models can outperform convolutional neural networks (CNNs) on various image recognition benchmarks.

4. Advantages: The use of transformers allows the model to capture long-range dependencies and relationships between patches. ViT models also scale well with the amount of available training data, and their performance improves significantly with larger datasets.

5. Results: The ViT achieves state-of-the-art results on several image classification benchmarks, surpassing traditional CNN architectures when pre-trained on large datasets.

6. Challenges: Training transformers for image recognition requires large datasets and significant computational resources. Without large-scale pre-training, ViT models do not perform as well as CNNs

7. batchsize used is 4096 its huge. 

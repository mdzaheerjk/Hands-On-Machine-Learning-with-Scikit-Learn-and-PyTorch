# HOML PyTorch #1 versus HOML Keras & TensorFlow #3

I wrote three TensorFlow (TF) editions of this book, published by O'Reilly in 2017, 2019, and 2022. If you have already read the latest TensorFlow edition of this book, here are the main changes you will find in this book (for changes between editions 1 and 2, see https://homl.info/changes2, and for changes between editions 2 and 3, see https://homl.info/changes3):

* All the code in the book was updated to recent library versions.
* All the code in Part 2 was migrated from TensorFlow and Keras to PyTorch. There were significant changes in all of these chapters.
* TensorFlow-specific content was removed, including former Chapter 12 (Custom Models and Training with TensorFlow) and Chapter 13 (Loading and Preprocessing Data with TensorFlow), and former Appendices C (Special Data Structures) and D (TensorFlow Graphs).
* The new Chapter 10 now introduces PyTorch, as well as TorchVision, TorchMetrics, and hyperparameter tuning using Optuna.
* I also added three big chapters on transformers (this is by far what required the most work, along with the SSM appendix):
    * Chapter 15 covers transformers for natural language processing. We build a Transformer from scratch, and use it to create a translation system from English to Spanish. Then we learn about encoder-only models like BERT, great for text classification tasks, multiple choice question answering, and more. Then we learn about decoder-only models like GPT, which are excellent at text generation, zero-shot learning, and much more. We then proceed to create a Transformer-based chatbot using pretrained models from the Hugging Face Hub. We learn how to fine-tune a pretrained model using SFT, RLHF, and DPO. Finally, we learn about RAG, vector databases, and how to connect the chatbot to tools, including using MCP.
    * Chapter 16 presents vision transformers (including ViT, DEiT, PVT, Swin, DINO, and more) and multimodal transformers (including VideoBERT, ViLBERT, CLIP, DALL·E, Perceiver, Flamingo, BLIP, and more).
    * Chapter 17, available online at https://homl.info/, discusses several advanced techniques to speed up and scale up transformers. This includes ways to speed up decoding, such as Key/Value caching and speculative decoding. We also look at how to accelerate attention, including sparse attention techniques (such as the Sparse Transformer, LongFormer, BigBird, and the Routing Transformer) and approximate attention techniques (such as the Reformer, Linformer, Performer), and projection-sharing techniques such as multi-query attention, grouped-query attention, and multi-head latent attention, and optimized implementations such as FlashAttention. We then scale up using mixture of experts (MoE), and speed up training using parameter-efficient fine-tuning (PEFT) such as low-rank adaptation (LoRA), activation checkpointing, sequence packing and bucketing, gradient accumulation, and various parallelism techniques.
* Chapter 18 goes into more depth on diffusion models, and also shows how to use pretrained diffusion models.
* Chapter 19 on reinforcement learning now covers Actor-Critic algorithms, including PPO, and it shows how to train your own agent to beat an Atari game, using the Stable-Baselines3 library.
* There are also three new appendices:
    * Appendix B (Mixed Precision and Quantization) explains how to shrink models so they can run faster and fit on smaller devices.
    * Appendix D (Relative Positional Encoding) discusses advanced positional encoding techniques for transformers.
    * Appendix E presents state-space models (SSMs).
* I also added Appendix F on older popular artificial neural network architectures, [available online](https://homl.info).
* To make room for the newer content, the chapter on support vector machines (SVMs) was [moved online](https://homl.info) and renamed to Appendix C; the last two appendices are also online at the same URL, and the deployment chapter was partially merged into Chapter 10.

The three editions of the TensorFlow/Keras version of this book are nicknamed homl1, homl2, and homl3. This book, which is the first edition of the PyTorch version, is nicknamed homlp. Try saying that three times in a row.

Note that most of the changes compared to the latest TensorFlow edition are in the second part of the book. If you have read homl3, then don't expect big changes in the first part of the book, other than up-to-date libraries: the fundamental concepts of machine learning haven't changed since 2022.

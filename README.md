# paligemma-finetning

Paligemma Finetuning for Medical dataset (Brain Scans)

# Dataset Used:
The dataset consists of brain scan and corresponding ground truth. 
Train: 161k
Test: 500

Link: gokulsabari/brain-xray (Uploaded in HuggingFace Dataset)

# Model Used

Paligemma (google/paligemma-3b-pt-224)

![image](https://github.com/user-attachments/assets/f9100a93-9815-42e9-9632-075adbae7a37)

Encoder Used: SigLIP-So400m
Decoder used: Gemma-2B

There are three important parts in a Vision Language Model
1) Image Encoder
2) Projection Layer
3) Text Decoder

# Image Encoder
In a Vision-Language Model (VLM), the image encoder is like a translator for pictures. It takes an image and processes it to understand the important details. The encoder turns this visual information into a form that the model can use, typically as a series of embeddings. These embeddings capture the essence of the image so that the model can relate it to words or text. Essentially, the image encoder helps the model "see" and understand what's in a picture so it can be used in tasks like image captioning or visual question answering.

# Projection Layer
The projection layer in a Vision Language Model (VLM) plays a crucial role in aligning the visual and textual information. 
The projection layer's main purpose is to map the visual and textual features into a shared embedding space. This allows the model to reason about the relationships between images and text.

# Text Decoder
In a Vision-Language Model (VLM), the text decoder takes the processed visual information (embeddings) from the Projection Layer and generates human-readable text from it. It essentially "translates" the visual details into a sentence, phrase, or word, allowing the model to produce captions, answer questions, or provide descriptions based on the image. The text decoder turns the model's understanding of an image into language that we can easily understand. 

# MultiModdal
## What is Multimmodal Learning?
> Multimodal learning is teaching or learning from a combination of various modes of data. Modes are channels of information, or anything that communicates meaning in some way, such as **text, images, sounds, gestures**, etc. Multimodal learning engages the mind in multiple learning styles at the same time, and can suit different learners and applications.
## Dataset 
[WebVision](https://data.vision.ee.ethz.ch/cvl/webvision/dataset2017.html) dataset.

<img width="691" alt="Screenshot 2023-11-23 113345" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/ca694708-b275-4573-b164-bfa0195aad3d">

The outline of the work is as follows:
1. Sharing of Experience: Municipal issue feedback classification in the Singapore government
2. Text Classification: Train a text classification model using [BERT](https://arxiv.org/abs/1810.04805)
3. Text and Image Classification (v1): Train a dual-encoder text and image classification model using BERT and [ResNet-50](https://arxiv.org/abs/1512.03385)
4. Text and Image Classification (v2): Train a joint-encoder text and image classification model using ALign BEfore Fuse ([ALBEF](https://github.com/salesforce/ALBEF))
## Model Architectures
A text-encoder model which uses only the text to predict the label.
![image](https://github.com/Mrkomiljon/MultiModdal/assets/92161283/85247f24-8326-4373-99f1-ad2782cf14ea)
## BERT-ResNet
A dual encoder which comprises a separate text encoder (BERT) and an image encoder (ResNet-50).
![image](https://github.com/Mrkomiljon/MultiModdal/assets/92161283/9d49ba6f-e0e9-4aa2-b5d0-532801b74b6d)
## ALBEF
A joint text-image encoder which aligns the BERT text encoder's embeddings with the image encoder's (Vision Transformers).
![image](https://github.com/Mrkomiljon/MultiModdal/assets/92161283/3a6cba2d-8a0f-4749-83ec-0e6a36335bed)
## Results
<img width="512" alt="Screenshot 2023-11-23 112823" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/849e947f-aef9-4261-8400-013c0a742f5a">
<img width="635" alt="Screenshot 2023-11-23 112749" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/ca6070ce-6fe7-4d0a-86dd-081c764150ad">
<img width="638" alt="Screenshot 2023-11-23 112534" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/c31f7e6b-7937-4a3c-9657-d77e1d544999">
<img width="639" alt="Screenshot 2023-11-23 112031" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/31437ede-1225-4fb8-b152-db033bb0f27e">
<img width="688" alt="Screenshot 2023-11-23 111944" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/14cd29c7-0c52-4cd7-b538-95bcc4563606">
<img width="1013" alt="Screenshot 2023-11-23 111742" src="https://github.com/Mrkomiljon/MultiModdal/assets/92161283/e32c6aa1-1d87-4f55-9fbe-db78c965f737">


# Facial-Recognition-And-Verification

This notebook is a programming exercise of the Deep Learning Specialization by Deeplearning.ai. In this notebook, we will build a face recognition system. Many of the ideas presented here are from [FaceNet](https://arxiv.org/pdf/1503.03832.pdf). 

Face recognition problems commonly fall into two categories:

- **Face Verification**  - &quot;is this the claimed person?&quot;. For example, at some airports, we can pass through customs by letting a system scan wer passport and then verifying that we (the person carrying the passport) are the correct person. A mobile phone that unlocks using wer face is also using face verification. This is a 1:1 matching problem.
- **Face Recognition**  - &quot;who is this person?&quot;. For example, employees entering the office without needing to otherwise identify themselves. This is a 1:K matching problem.

FaceNet learns a neural network that encodes a face image into a vector of 128 numbers. By comparing two such vectors, we can then determine if two pictures are of the same person.

**In this notebook, we will:**

- Implement the triplet loss function
- Use a pretrained model to map face images into 128-dimensional encodings
- Use these encodings to perform face verification and face recognition

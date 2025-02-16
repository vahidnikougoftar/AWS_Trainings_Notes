# Foundational models
- With FMs, instead of gathering labeled data for each model and training multiple models as in traditional ML, you can adapt a single FM to perform multiple tasks. These tasks include text generation, text summarization, information extraction, image generation, chatbot interactions, and question answering. FMs can also serve as the starting point for developing more specialized models.
-
## Foundation Model Lifecycle 
1. Data Collection : Massive Unlabeled data (e.g. Images,Video, text off internet)
2. Pre-training : self-supervised learning (i.e. generating context and associations based on Self-supervised learning makes use of the structure within the data to autogenerate labels)
3. Optimization : a Foundational Model (FM) can be optiized for specific domains, using Prompt engineering, RAG, and Fine Tuning.
4. Evaluation : important for biz needs, regardless of a off-the shelf or Fine Tuned model. Can have different metrics and it's business dependant.
5. Deployment : APIs or embedded software
6. Monitoring and improvements : model drift (less accurate results over time with new data)

# Types of Foundational Models:
1. LLMs
2. Diffusion Models (forward Diffusion => Reverse Diffusion)
3. Multimodal Models
4. GANs (Generative Adversarial Networks)
6. Variational Autoencoders (encode / decode steps: the model encodes the input data into a Latent Space: lower level representation of input data; then decodes a Guassian statistical representation of the model to generate new data)

## <b>Optimizing</b> the FM : 
1. Prompt engineering : fastest and lowest cost
2. Fine-Tuning: a supervised learning step (remember FMs are initially self-supervised pre-training) with narrower dataset to update parameters of the NN.
   2.1. Instruction fine-tuning uses examples of how the model should respond to a specific instruction. Prompt tuning is a type of instruction fine-tuning.
   2.2. Reinforcement learning from human feedback (RLHF) provides human feedback data, resulting in a model that is better aligned with human preferences.
3. RAG (Retrieval Augmented Generation)
This technique is similar to fine-tuning. However, rather than having to fine-tune an FM with a small set of labeled examples, RAG retrieves a small set of relevant documents and uses that to provide context to answer the user prompt. RAG will not change the weights of the foundation model, whereas fine-tuning will change model weights.
   

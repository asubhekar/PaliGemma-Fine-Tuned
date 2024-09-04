# PaliGemma-Fine-Tuned-CordV2
PaliGemma is a versatile and lightweight vision-language model (VLM) inspired by PaLI-3 and based on open components such as the SigLIP vision model and the Gemma language model. It takes both image and text as input and generates text as output, supporting multiple languages. It is designed for class-leading fine-tune performance on a wide range of vision-language tasks such as image and short video caption, visual question answering, text reading, object detection and object segmentation.

### Model Architecture 
PaliGemma is the composition of a Transformer decoder and a Vision Transformer image encoder, with a total of 3 billion params. The model was fine tuned on CordV2 dataset.

### Inputs and outputs
- Input: Image and text string, such as a prompt to caption the image, or a question.
- Output: Generated text in response to the input, such as a caption of the image, an answer to a question, a list of object bounding box coordinates, or segmentation codewords.

### Model Acceleration
- Model was trained using PyTorch Accelerate

### Optimization 
- Utilized BitsandBytes to quantize the model to 4-bit from float-32.
- Used Q-LORA.

### Future Work 
- Training the model using HuggingFace Acclerate framework. 


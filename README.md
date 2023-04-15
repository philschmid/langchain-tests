# LangChain tips to work with HuggingFace Transformers


1. Use Tokenizers to split data into tokens to fit the model max length
2. use `chain.prompt_length(docs)` to make sure the prompt is not too long for your model 
3. Define `model_kwargs` to pass to the model forward method, e.g. `do_sample=True, max_length=100, top_k=50, top_p=0.95, temperature=0.9`
4. 
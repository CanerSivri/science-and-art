Case 1 (500,0.95,0.7):


<img width="306" height="172" alt="1" src="https://github.com/user-attachments/assets/19e44c30-1e9d-4cba-be21-8988745f9b93" />


Outputs:


<img width="1918" height="1037" alt="1 1" src="https://github.com/user-attachments/assets/fe859cea-d4fc-44bd-ac86-bf459b61008c" />


Case 2 (700,1,1):


<img width="309" height="170" alt="2" src="https://github.com/user-attachments/assets/059bdd9a-43d9-4523-92e7-591dd2188e66" />


Outputs:


<img width="1912" height="1041" alt="2 1" src="https://github.com/user-attachments/assets/3a0bc3cf-9f82-4a57-8fb1-3935affa5e6f" />


Case 3 (300,0.5,0.5):


<img width="290" height="174" alt="3" src="https://github.com/user-attachments/assets/55028512-12c8-4564-9b9f-9d42d5515326" />


Outputs:


<img width="1912" height="1037" alt="3 1" src="https://github.com/user-attachments/assets/d334b51e-30da-40d3-84f0-28c46a5dacf8" />



-> max_length: This parameter controls the maximum number of tokens (words or sub-word units) the model will generate for its response.
Increasing max_length: Allows for longer, more detailed, and potentially more comprehensive responses. However, it can also lead to the model repeating itself or losing coherence over very long generations.
Decreasing max_length: Results in shorter, more concise responses. Useful when you need quick answers or want to avoid verbosity.

-> temperature: This parameter directly controls the randomness of the generated text. It works by scaling the probability distribution of the next token.
Increasing temperature (e.g., from 0.5 to 1.0 or higher): Makes the model's output more random, creative, and diverse. The model is more likely to choose lower-probability tokens, leading to unexpected or surprising responses. High temperatures can sometimes lead to less coherent or nonsensical text.
Decreasing temperature (e.g., from 0.5 to 0.1 or lower): Makes the model's output more deterministic and focused. The model becomes more confident in choosing high-probability tokens, resulting in more conservative, predictable, and often more coherent responses. A very low temperature (e.g., 0.1) can make the model repetitive.

-> top_k: This parameter limits the sampling pool to the top k most probable next tokens.
Increasing top_k (e.g., from 50 to 100): Expands the set of tokens from which the model can sample. This generally leads to more diverse and less predictable responses, as the model considers a wider range of options.
Decreasing top_k (e.g., from 50 to 10): Narrows the set of tokens from which the model can sample. This makes the responses more focused and predictable, as the model is restricted to only the very highest-probability words. Setting top_k=1 is equivalent to greedy decoding (selecting only the single most probable token).

-> top_p (also known as Nucleus Sampling): This parameter limits the sampling pool to the smallest set of tokens whose cumulative probability exceeds p.
Increasing top_p (e.g., from 0.5 to 0.95): Allows the model to consider a larger and more diverse set of tokens whose cumulative probability is high. This can lead to more creative and varied outputs, as the model can pick from a wider, yet still high-probability, range of options.
Decreasing top_p (e.g., from 0.5 to 0.1): Constricts the set of tokens from which the model can sample, focusing on only the very highest-probability tokens. This makes the responses more conservative, predictable, and less prone to generating unusual or irrelevant text.

# Email Classification
## Custom Architecture
## Architecture 

- ### Input
    Body and subject of mail.
    
- ### Embedding Layer
    Pretrained GloVe (6B, 300D) embeddings. Frozen during training.

- ### Encoders
    Bidirectional LSTM encoders for both subject and body.

- ### Attention Layers
    Applied to both subject and body encoder outputs to capture important parts of input

- ### Shared Dense Layer/Block 
    Linear => ReLU => Dropout(0.2) \
    Concatentation of rich representations of subject and body 
    


# CS336LanguageModelingFromScratch

📺 **YouTube Link**: [Stanford CS336 Language Modeling from Scratch | Spring 2025](https://www.youtube.com/watch?v=SQ3fZ1sAqXI&list=PLoROMvodv4rOY23Y0BoGoBGgQ1zmU_MT_)

With experience in Python, RNNs, NLP, and Transformers, I’m following this Stanford open course to deepen my understanding of language models and identify areas for further improvement.

📘 I will upload all the assignments here to document my learning journey and connect with peers for discussion and collaboration.


## 📚 Overview of the Class

- Data Processing  
- Tokenization  
- Model Architecture  
- Training  
- Scaling Laws  
- Alignment  

---

## 🧱 First Class: Tokenization

### 🔄 String to Tokens (Indices)

**Methods of Tokenization:**
- **Character-level**:  
  - Small tokens  
  - Longer sequences  
- **Word-level**:  
  - Larger tokens  
  - Shorter sequences  
- **BPE (Byte Pair Encoding)**:  
  - A subword-level method that balances vocabulary size and sequence length

##  Second Class: Pytorch and Resource Accounting
Tensor: basic block of storing everything, such as parameter, gradienets, activations, optimizer states

### Memory(GB) accounting

### Compute (FLOPS) accounting
Bu default, tensors are stored in CPU memory

- **Tensors on gpu**:  
- **Tensor operation**:  
  - storage: stride  
  - slice:
  - elementwise: 
  - matmul:  batch, sequence.
- **Tensor einops**: 
  - concept: a library for manipulating tensors where dimensions are named.
  - Jaxtyping: keep track of tensor dimensions
  - einsum: it is generalized matrix multiplication with good bookkeeping.
  - reduce:
  - rearrange:
- **Tensor operations flops / cost**: 
  - concept: A floating-poin operation(FLOP) is a basic operation like addition(x + y) or multiplication(xy).
  - Two confusing acronyms
    - FLOPs: floating-point operations
    - FLOP/s or FLOPS: floating-point operations per second, which is used to measure the speed hardware.
  - Model FlOPs utilization (MFU)
    - Definition: (actual FLOP/s) / (promised FLOP/s) [ignore communication/overhead]
    - mfu = actual_flop_per_sec / promised_flop_per_sec
    - Usually, MFU of >= 0.5 is quite good (and will be higher if matmuls dominate)
    FLOP/s depends on hardware(H100 >> A100) and the datatype(bfloat16 >> float32)
- **Gradients basics**:
  - Basic ML knowledge to understand:
    - The heart of training a neural network:
      - forward pass (forward propagation): feed input data through the neural network to produce an output. 
      - backward pass (backpropagation): 
        - After forward pass and the calculation of the loss, the backward pass begins. The process moves in the reverse direction, from the output layer back to the input layer.
        - Goal: calculate the gradient of the loss function with respect to each of the network's parameters (weights and biases).
        - Backward gradient: 
        
  - 







    

 

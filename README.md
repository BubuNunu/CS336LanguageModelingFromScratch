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

##  Second Class: Pytorch and jjjResource Accounting
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
  - 
    

 

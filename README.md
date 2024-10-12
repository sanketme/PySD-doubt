### **PySD model run not matching with vensim model run**

### **Description:**

We create a stock-flow model in Vensim, where:

1. **Both input and output parameters** initially take deterministic values.  
2. **One input parameter** is then replaced with a randomly generated value following a normal distribution (RND).  

Both versions of the model (with deterministic and RND inputs) are run in Vensim, and the results are saved as CSV files.

Next, we save the Vensim models and **run them again using PySD**. As part of the experiment, we pass the RND-generated input parameter from the Vensim model into the PySD run using the **`params=` argument**. 

### **Issue:**
We expect the PySD model to produce the same output as the corresponding Vensim model, but **the results are different**. 

### **Objective:**
We want to understand **why** the outputs from the PySD and Vensim models do not match, and how we can modify the PySD run to generate the same output as the Vensim calculations.


### **What does it lead to?**
The actual model (which has not been shared), produces quite a different results in the PySD run which is of main concern for my solution

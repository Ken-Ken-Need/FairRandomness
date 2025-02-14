# FairRandomness

## Project Description
This is a research focused project, aiming at developing a system to evaluate the fairness of random generated by delayed hash methods. In particular, we aim at measuring the cost of manipulating a real-life random event, such as stock price or sport game outcome.

To clarify more, the **fair randomness** we talked about should have the following properties:

1. All parties don't have to trust each other, in the sense that there's a public scheme that everyone could produce the same output and convinced that it is fair randomness.
2. To achieve the property above, the input of such scheme will be a real-world event, such as stock prices or sport game outcome, with entropy high enough to produce a random enough outcome.

   For example, if we take the first digit of AAPL stock price as input, it will not serve as a good random source as it has a low entropy, while the third digit after the decimal point of the stock price, though having a high entropy, is easy manipulated by an adversary. 

   <img width="697" alt="stock prices of AAPL in the last year" src="https://github.com/user-attachments/assets/260ab014-673b-41e1-9092-e75c026fa354" />


There are several interesting research angles to explore when considering a randomness scheme that binds its output to a real-life event (like a stock price) combined with cryptographic tools. Here are some key aspects:

1. **Entropy Analysis and Measurement:**  
   - **Source Quality:** Investigate how much entropy is present in real-life events such as stock prices. Are the last-n digits of a stock price sufficiently random?  
   - **Statistical Testing:** Develop or apply statistical tests to validate the distribution and unpredictability of the digits extracted from such events.

2. **Economic and Game-Theoretic Modeling:**  
   - **Incentive Structures:** Model the economic incentives for potential attackers. Quantify the cost required to manipulate the stock price versus the potential gain from influencing the randomness outcome.  
   - **Manipulation Resistance:** Analyze under what conditions (cost/gain ratios) the scheme is secure, and how changes in market dynamics might affect this balance.

3. **Cryptographic Hash Functions and Random Oracle Modeling:**  
   - **Hash Function Security:** Research how the properties of hash functions (collision resistance, preimage resistance, etc.) ensure that combining the real-life event with a hash function preserves fairness.  
   - **Random Oracle Assumptions:** Study the implications of treating the hash function as a random oracle in this context, and explore any limitations or alternatives.

4. **Fairness and Transparency in Randomness Generation:**  
   - **Verifiability:** Design methods to allow independent verification that the randomness was generated correctly, using publicly available data (e.g., stock prices) and transparent hash computations.  
   - **Protocol Design:** Create protocols that ensure no single party can manipulate or influence the outcome, possibly by incorporating commitments or time-lock puzzles.

5. **Robustness Against Adversarial Manipulation:**  
   - **Attack Vectors:** Identify potential attack vectors (such as market manipulation or data feed tampering) and propose defenses.  
   - **Risk Assessment:** Evaluate how robust the randomness is in various scenarios, including situations with partially compromised data sources.

6. **Comparative Analysis with Other Randomness Sources:**  
   - **Benchmarking:** Compare the fairness and security of using a real-life event like a stock price versus other randomness sources (e.g., hardware random number generators, environmental noise).  
   - **Hybrid Approaches:** Investigate the benefits and drawbacks of combining multiple entropy sources to improve overall randomness quality.

Each of these areas not only delves into the technical details of cryptographic security but also addresses economic and practical concerns, making the research both interdisciplinary and highly relevant to real-world applications.
## Planning
1. **Literature review**
2. **Learn more about information theory**
3. **Evaluation of the information entropy of the random events as mentioned above**
## Objectives


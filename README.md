Here's a `README.md` template for your CYK algorithm implementation:

---

# CYK Algorithm Implementation

This repository contains an implementation of the **Cocke-Younger-Kasami (CYK) algorithm** in [specify the programming language you've used]. The CYK algorithm is used to determine whether a given string can be generated by a context-free grammar (CFG) in **Chomsky Normal Form (CNF)**.

## Features
- Parses strings using a context-free grammar in CNF.
- Supports user-defined CFG input in the correct format.
- Efficiently checks if a string belongs to the language generated by the CFG.
  
## Algorithm Overview
The CYK algorithm is a bottom-up parsing algorithm that works with context-free grammars in Chomsky Normal Form. The input consists of a string `w` and a CFG `G`. The algorithm constructs a table of possible non-terminal symbols that can generate each substring of `w`. In the end, it checks if the start symbol of the grammar can generate the entire string.

### Key Steps:
1. **Input**: A string `w` and a CFG `G` in Chomsky Normal Form.
2. **Initialization**: Construct a 2D table where each entry contains possible non-terminal symbols that generate the corresponding substring of `w`.
3. **Table Filling**: For each substring, recursively fill the table by checking which grammar rules apply.
4. **Final Check**: If the start symbol of the CFG is in the top-right entry of the table, the string `w` can be generated by the grammar.

## Files
- `cyk.py` (or relevant file name): Contains the implementation of the CYK algorithm.
- `grammar.txt`: Contains a sample CFG in CNF format.
- `README.md`: This documentation file.

## Getting Started

### Prerequisites
- [Programming language used, e.g., Python 3.x]
- Basic understanding of context-free grammars and Chomsky Normal Form.

### Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/Jilpadalia/CYK-algorithm-TOC.git
   ```
2. Navigate to the project directory:
   ```bash
   cd CYK-algorithm-TOC
   ```
3. Run the algorithm:
   ```bash
   streamlit run sample.py
   ```
4. Provide the string to be checked and the CFG in CNF format.

### Example

To check if the string `"baaba"` can be generated by a CFG in CNF, run the algorithm and input the string when prompted.

## Output
The program will output whether the string belongs to the language of the grammar or not.

### Sample Output:
```
The string 'baaba' belongs to the language of the given grammar.
```

## Contributing
Feel free to fork this repository, submit issues, or make pull requests if you have improvements or find bugs!



---

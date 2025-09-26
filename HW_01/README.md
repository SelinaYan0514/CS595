# CS 595 Homework 1: Merkle Trees and Cryptographic Hashing

**Due date:** Tuesday, September 16 at 11:59pm on [Gradescope](https://www.gradescope.com) (entry code: 2244N4).  

*You must follow the Academic Code of Conduct and Collaboration Policy stated in the course syllabus at all times while working on this assignment.*

---

## Assignment Overview
This assignment consists of three parts:

1. **Merkle Tree Verification**  
   Verify that a given Merkle Tree root has been computed correctly.  

2. **Transaction Inclusion**  
   Verify that the transaction is included in the block by computing the Merkle Tree path to the root.  

3. **Modified Hash Function**  
   Modify the hash function to use SHA-256 truncated to the first 12 bits and demonstrate how to forge transaction inclusion.  

---

## Getting Started
To begin, first load the autograder tests in one of the following ways:

- **Using Google Colab**: Execute the code block provided and upload the zipped `tests` folder.  
- **Running Jupyter Notebook locally**: Unzip `tests.zip` and ensure the `tests` folder is in the same directory as this notebook. Then continue to part 1.  

# CST407SRSDOD
Data Oriented Design

Project Name(s):  

    - DOD

Purposes:  

    - Understand Data Oriented Design.  
    - Learn to use C++ concurrency library.  
    - Practice using the C++ random number generator and clocks.  

Specification:  

This SRS contains 2 parts.  

For both parts of the SRS, you will need to do the following:  
- Create an contiguous array of bytes (std::byte or unsigned char) in 2 dimensions.  Tip: Use a vector<byte> and divide into chunks if your memory stack is too small.  
- Fill the array with uniformly distributed random values in the range \[0, 256).  
- Calculate the number of values greater than T where T is \[0, 256).  

Count the number of values greater than the threshold T.  

Measure the time it takes to complete counting and graph the result as the dependent variable.  

Before coding, write your hypothesis results in your REPORT.md file predicting the basic shape of the resulting graphs. There are no points having your hypothesis confirmed, but a well thought out hypothesis will earn you points. When completed, review your hypothesis and why your hypothesis was confirmed or refuted. 

Create graphs as follows to test both your hypothesis:  

1) Row/Column Major  

Independent variable:  
- Where N == \[1, 5000), create square array\[N]\[N]

Compare:  
- Row vs Column order traversal.  

Constants:  
- Single threaded.  
- Maximum value threshold == 127.  

---

2) Thread Local Storage

Independent variable:  
- Number of tasks.  

Compare:  
- Thread global increment of total array vs local increment.  
- Maximum value threshold == 0, 63, 127, 191 and 254.  

Constants:  
- Row order traversal  
- Where N == 5000, create square array\[N]\[N] (Tip: Use a vector<byte> and divide into chunks.)  

###

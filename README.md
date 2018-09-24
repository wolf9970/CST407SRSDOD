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
- Create an contiguous array of bytes (std::byte or unsigned char) in 2 dimensions.  Tip: Use a vector<std::byte> and divide into chunks if your memory stack is too small.  
- Fill the array with uniformly distributed random values in the range \[0, 256).  
- Calculate the number of values greater than T where T is \[0, 256).  

Count the number of values greater than the threshold T.  

Measure the time it takes to complete counting and graph time as the dependent variable.  

Before coding, write an hypothesis for your results in your REPORT.md file predicting the basic shape of the resulting graph. There are no points having your hypothesis confirmed, but a well thought out hypothesis will earn you points. When completed, review your hypothesis and compare to the actual results expected.  

Tips:  
- array\[N]\[N] does NOT mean a 'C' array in this specification.  
- Use a vector<byte> and divide into chunks, but any contiguous data structure will work.  
    
Create graphs as follows to test both your hypothesis:  

Part 1:  Row/Column Major  

Independent variable:  
- Where N == \[1, 5000), create memory contiguous square array\[N]\[N] (I do NOT mean a 'C' array)  

Compare:  
- Row vs Column order traversal.  

Invariants:  
- Single threaded.  

---

Part 2:  Thread Local Storage

Independent variables:  
- Number of tasks.  
- Number of threads.  

Compare:  
- Thread global (not local) increment of total array vs task based.  
- Maximum value threshold == 0, 63, 127, 191 and 254.  

Invariants:  
- Row order traversal  
- N == 5000, create square array\[N]\[N]

###

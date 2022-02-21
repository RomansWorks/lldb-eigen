# lldb-eigen

This is a modified version of the original LLDB extension for pretty-printing Eigen matrices. 

Original can be found here: https://gitlab.com/libeigen/eigen/-/blob/master/debug/lldb/eigenlldb.py

The modification handles some edge cases where the variables on the frame are declared such that the Matrix template parameters are nested under other templates, due to CRTP. 



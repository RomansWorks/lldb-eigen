# lldb-eigen

This is a modified version of the original LLDB extension for pretty-printing Eigen matrices. 

Original can be found here: https://gitlab.com/libeigen/eigen/-/blob/master/debug/lldb/eigenlldb.py

The modification handles some edge cases where the variables on the frame are declared such that the Matrix template parameters are nested under other templates, due to CRTP. 

# Using

(note: copied from the file header)

1. Add the following line (change it according to the path to this file)
    to the file ~/.lldbinit (create one if it doesn't exist):
        `command script import /path/to/eigenlldb.py`
2. Inspect the variables in LLDB command line
        `frame variable`



# Unhandled File Error in Shell Script

This repository demonstrates a common error in shell scripting: the lack of error handling when working with files. The `bug.sh` script attempts to process a file, but it fails silently if the file doesn't exist or is unreadable. The `bugSolution.sh` script demonstrates how to improve the script by adding robust error handling.

## Bug

The `bug.sh` script lacks error handling, leading to unexpected behavior if the target file is missing or inaccessible.  This can be especially problematic in production environments.

## Solution

The `bugSolution.sh` script addresses this issue by:

1. Checking if the file exists using `-f`.
2. Checking if the file is readable using `-r`.
3. Displaying informative error messages if the file is not found or is not readable.
4. Using exit codes to indicate success or failure.

This improved error handling increases the robustness and reliability of the script.
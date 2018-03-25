# Tests Folder

This folder is for tests. 

## Test Structure

There are two kinds of tests we will be writing.

1.  Code unit tests. These tests verify minimal sections of code. They will be written with a native testing library. Probably using one or more of:
    - For general testing:
        - `catch2`
        - `gtest`
        - Boost.Test
    - Test fixture mocking:
        - `mockitopp`
    - Benchmarking:
        - `googlebench`
2. Functional tests. These tests verify the function of the code as a whole. They will be written in a scripting language.
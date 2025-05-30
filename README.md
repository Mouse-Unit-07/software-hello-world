# Hello World Repo
- Simple Hello World repo w/ source code and a main.c for a hello_world interface w/ a single function that prints "Hello World\r\n"
- Serves as an example of a source code repository and required structure/CMakeLists.txt files to be compatible w/ the generic development environment developed for the team.

## Structure
  - **CMakeLists.txt**
    - top level CMakeLists.txt file

  - **main.c**
    - main to run standalone on MCU if needed; optional otherwise

  - **hello_world/** [your interface]
    - **print_hello_world.c**
    - **print_hello_world.h**
    - **CMakeLists.txt**
      - interface level CMakeLists.txt file
      - **tests/**
        - **CMakeLists.txt**
          - interface tests level CMakeLists.txt file 
        - **test_print_hello_world.cpp**
          - interface tests
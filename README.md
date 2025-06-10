# BrickGame Snake
- The program must be developed in C++ language of C++17 standard.
- The program must consist of two parts: a library that implements the logic of the snake game and a desktop interface.
- A finite-state machine must be used to formalize the logic of the game.
 The library must conform to the specification given in the first part of BrickGame (you can find it in materials/library-specification.md)
- The program library code must be located in the `src/brick_game/snake` folder.
- The program interface code must be located in the `src/gui/desktop` folder
- The library that implements the game logic must be covered by unit tests. - Pay special attention to checking the FMS states and transitions. Use GTest library for tests. The coverage of the library with tests must be at least 80 percent.
- The program must be built using a Makefile with the standard set of targets for GNU-programs: all, install, uninstall, clean, dvi, dist, tests. Installation directory can be arbitrary
- The implementation must be with a GUI, based on one of the GUI libraries with an API for C++17:
  - Qt
- The program must be implemented using the MVC pattern. Also: 
  - there must be no business logic code in the view code;
  - there must be no interface code in the model, presenter and view model
  - controllers must be thin.
- Copy the library folder with the game logic from the BrickGame v1.0 project.
- The desktop interface must support the game from the BrickGame v1.0 project.
- Copy the folder with the console interface of the game from the BrickGame v1.0 project.
The console interface needs to support the Snake.
- The following mechanics must be in the Snake game:
  - The snake must move across the field on its own, one block ahead when the game timer expires.
  - When a snake meets an "apple", its length increases by one.
  - When the length of the snake reaches 200 units, the game ends with the player winning.
  - When a snake bumps into a field boundary or itself, the game ends with the player losing.
  - The user can change the direction of movement of the snake using the arrows, and the snake can only turn left and right relative to the current direction of movement.
  - The user can speed up the movement of the snake by pressing the action key.
- The initial length of the snake is four "pixels".
- The playing field is 10 "pixels" wide and 20 "pixels" high.
- Prepare a diagram showing all states and transitions between them for the implemented FMS for project submission.

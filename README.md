# Dockerfile CMD Instruction Error
This example demonstrates a common error in Dockerfiles: combining the `pip install` and application execution within a single `CMD` instruction. If the `pip install` step fails, the subsequent execution of the application will not occur, and no error will be reported.

**bug.Dockerfile** contains the erroneous Dockerfile.

**bugSolution.Dockerfile** shows the corrected Dockerfile.

The solution separates the installation and execution steps, providing clearer error reporting and more robust behavior.
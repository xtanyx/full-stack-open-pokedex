Language: C

Linting:
There are many tools available for linting from ones that act as static code analysers, to ones that can format your code to a specific coding style. Static code analyzers help debug and find vulnerabilities in code that isn't currently being run (static). Some examples of tools that help perform static code analysis: 
- GCC with -fanalyzer flag 
- clang-format: a set of tools that make sure your code follows a specific coding style
- PMD: checks for code duplication

Testing:
- API sanity checker: It analyses declarations of in C header files to generate input data and and come up with simple test cases. Suitable for simple use cases.
- Unity Test: unit testing for soruce code that targets microcontrollers
- Check: a unit testing framework that runs in a separate address space from your code and helps catch assertion and segmentation errors. The test reports can be generated in multiple formats.

Building:
- CMake: a build system that supports multiple build trees for different purposes. Includes a cross-platform testing system.
- Make: helps build programs by specifying how to compute files from other files
- Ninja: a build system who focus in on speed

There are many alternative Continuous Integration Services to Jenkins and Github actions:
- AWS Codebuild: enables compiling, testing and packaging after just specifying source code location and choosing build settings.
- Bamboo: a CI/CD server
- Kraken CI: a self-hosted system focused on testing

Assuming the project is one on the smaller case and doesn't deal with any out of the box usage cases, Github actions is probably the better option to use for CI/CD since it requires minimal initial setup, and the team would need something they can start using it immediately.
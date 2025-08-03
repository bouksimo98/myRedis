[![progress-banner](https://backend.codecrafters.io/progress/redis/89b2f94c-794e-41cd-95dd-20ab2823ee9a)](https://app.codecrafters.io/users/codecrafters-bot?r=2qF)

This is a starting point for C++ solutions to the
["Build Your Own Redis" Challenge](https://codecrafters.io/challenges/redis).

In this challenge, you'll build a toy Redis clone that's capable of handling
basic commands like `PING`, `SET` and `GET`. Along the way we'll learn about
event loops, the Redis protocol and more.

**Note**: If you're viewing this repo on GitHub, head over to
[codecrafters.io](https://codecrafters.io) to try the challenge.

# Prerequisites

The entry point for your Redis implementation is in `src/Server.cpp`. Study and
uncomment the relevant code, and push your changes to pass the first stage:

```sh
git commit -am "pass 1st stage" # any msg
git push origin master
```

That's all!

Ensure the following are installed:

1. CMake ≥ 3.16
1. A C++ compiler (GCC, Clang, or MSVC)
1. make or ninja

# Installing vcpkg (if not already installed)

```sh
# Clone vcpkg
git clone https://github.com/microsoft/vcpkg.git ~/vcpkg

# Bootstrap vcpkg
cd ~/vcpkg
./bootstrap-vcpkg.sh
```

# Building the Project

1. Run `./your_program.sh` to run your Redis server, which is implemented in
   `src/Server.cpp`.
1. Commit your changes and run `git push origin master` to submit your solution
   to CodeCrafters. Test output will be streamed to your terminal.

# Interacting with Your Redis Server

To test with a Redis client (e.g., nc or telnet):

```sh
nc localhost 6379
```

Then type:

```
PING
```

Expected output:

```
+PONG
```

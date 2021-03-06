# Building

Since Ponce v0.3 we have moved the building compilation process to use `CMake`. Doing this we unify the way that configuration and building happens for Linux, Windows and OSX. 

We now support providing feedback on the pseudocode about symbolic or taint instructions. For this feature to work you need to add `hexrays.hpp` to your IDA SDK include folder. `hexrays.hpp` can be found on `plugins/hexrays_sdk/` on your IDA installation path. 

If you have not purchased the hex-rays decompiler you can still build Ponce by using `-DBUILD_HEXRAYS_SUPPORT=OFF`. 

We use Github actions as our CI environment. Check the [action files](https://github.com/illera88/Ponce/tree/master/.github/workflows) if you want to understand how the building process happens.
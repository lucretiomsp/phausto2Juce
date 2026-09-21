# phausto2Juce
Resources to learn how to export Phausto DSps to JUCE plugins

##How to build the plugin with cmake.
cmake -B build -DCMAKE_BUILD_TYPE=Release -DJUCE_PATH=/path/to/JUCE
cmake --build build --config Release -j

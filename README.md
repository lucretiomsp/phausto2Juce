# phausto2Juce
Resources to learn how to export Phausto DSps to JUCE plugins

## Create a stereo Zita Reverb and export it
```smalltalk
dsp := (Wire new => ZitaRevStereo new ) stereo asDsp.
dsp init.
dsp export2JuceWithName: 'ZitaVerb' type: PhEffectType new.
```

##How to build the plugin with cmake.
```bash
cmake -B build -DCMAKE_BUILD_TYPE=Release -DJUCE_PATH=/path/to/JUCE
cmake --build build --config Release -j
```

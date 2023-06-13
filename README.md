A collection of tools for live VJing sound reactive visuals. To use, copy everything inside 'ext-tox' into a folder in your project called 'ext-tox'.

AudioAnalysis.toe is an example. Drag any file you want into the Audio File In CHOP, the song I used wouldn't fit inside this repo.

# Components

ChannelStrip is a simple preprocessing tool with a few stages:

- A gain stage
- Optional sum to Mono
- An EQ powered by the Melda MEqualizer VST
- A noise gate

It outputs the processed audio and the triggers from the gate. This is really useful, for example, to trigger an ADSR envolope on drum hits.

Crossover is a 4 band crossover filter. It outputs the audio from each band. For processing full tracks, drum overheads, room mics, or other sound sources with a lot of frequency content in them. It can be really powerful to hook up ChannelStrips after Crossovers.

# Monitoring

Each component allows for sending audio from different points in the processing chain out to an audio device like headphones. There's no way yet to have mutually exclusive monitoring, but I'm working on it.

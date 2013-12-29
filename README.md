# Playrec Example Scripts

This repo contains a number of scripts that give examples of how to use Playrec, and provide some basic functionality that may be useful in other scenarios. Scripts include:

## test_playrec

Checks if playrec is available and then runs 3 output tests on a selected output device. The first test shows simple blocking output, the second uses simple non-blocking output and the third shows how continuous output can be achieved without needing to precalculate all samples.

## select_play_device

Displays a textual list of all available output devices in the command window, and waits for user input to select. Only a valid device number can be selected.

## select_rec_device

Displays a textual list of all available record devices in the command window, and waits for user input. Only a valid device number can be selected.

## play_wav

Plays a mono or stereo wav file using Playrec. The samples are loaded from the file in sections, demonstrating how to create a continuous output without glitches.

## play_ambi_wav

Plays a WAVEX Ambisonic Wav file using Playrec. The samples are loaded from the file and converted to the required output in sections, demonstrating how to create a continuous output without glitches. This utilises wavexread.m, a version of wavread modified by Sylvain Choisel to read wave-format-extensible files.

## spectrum_analyser

Uses Playrec to show a realtime spectrum and waveform, and some of the possibilities that Playrec can be used for.

## bformat_dec

Decodes a B-Format signal into speaker feeds, as used by play_ambi_wav.

## bformat_enc

Encodes a mono signal into a B-Format signal at a specified azimuth and elevation.

## bformat_rot_tilt_tumble

Rotates, tilts and tumbles a B-Format signal.

## loop_back

Demonstrates simultaneous input and output by looping an input channel onto one or more outputs. By optimising parameters the latency can be reduced, depending on the target platform.


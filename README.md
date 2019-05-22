# Sawtooth Waveform

This is demo of a sawtooth waveform and the math to create it.

## Preparation

All the code in this repo wsa made with the [Anaconda Distribution](https://www.anaconda.com/distribution/) of Python, which makes installation of all the libraries needed to run it easier. If you want to bypass that distribution and install all the dependencies yourself, that can work. But those instructions are not covered here.

In addition to Anaconda, this require the `sounddevice` module to be loaded. You can do this with

```
pip install sounddevice
```

Also you can run `jupyter notebook` in the directory of this repo to access the notebook in this repo.

## Usage

To play a pure sawtooth wave and write its output to a file, run the following command:

```
python pure_sawtooth_to_file_and_speakers.py
```

To play a sawtooth wave by additive synthesis:

```
python additive_sawtooth_to_file_and_speakers.py
```

To explore the math and visual explorations of sawtooth waves use the Jupyter notebook, see the notebook sawtooth_in_pictures.ipynb.

Note that while you can view it in directly in GitHub, the rendering of the equations is better if you look at in jupyter directly.

## Topics not covered

The most important topc not covered is that of the Nyquist rate when handling sawtooth waves. *You need to limit the number of harmonics you put in the wave* or you will cause alias if you overrun the Nyquist sampling rate. These demos use a sampling rate of 44100 hz for simplicity. But 96000 hz is often used to capture the higher harmonics of sawtooth waves.

### Now go out an have fun with sawtooth waves!

## Legal Things

MIT License

Copyright (c) 2019 Alicia Key

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

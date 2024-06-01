# Audio Transport

Windows Version of: https://github.com/sportdeath/audio_transport

## Usage

### Static Use

You will need [```fftw3```](http://fftw.org/), [```ffmpeg```](https://ffmpeg.org/) and [```audiorw```](https://github.com/deleonerick1808/audiorw_windows).


Once the dependencies are installed, install ```audio_transport``` with ```cmake```:

    git clone https://github.com/deleonerick1808/audio_transport_windows
    mkdir audio_transport\build
    cd audio_transport\build
    cmake .. -D BUILD_EXAMPLES=ON
    cmake --build . --config Release
    cmake --install .

Note that for the files FindAUDIORW.cmake and FindFFTW.cmake you need to update the directories of where to find the libraries. To install it might be required to run command prompt as administrator. Also, before building, you might need to manually link the libraries of FFMPEG to Visual Studio because there might be errors that will make the build fail.

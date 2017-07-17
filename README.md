Audiobox - Docker   [![Build Status](https://travis-ci.org/v1shwa/audiobox-docker.svg?branch=master)](https://travis-ci.org/v1shwa/audiobox-docker) [![Docker Automated buil](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/v1shwa/audiobox/)
---

A jupyter notebook based Docker image for speech/audio synthesis with all essential tools included.

### Usage
  - Pull Image
   
        docker pull v1shwa/audiobox   
  - Launch a jupyter notebook in detached mode
  
        docker run -p 8888:8888 -d v1shwa/audiobox
  - Mount current directory as data volume
        
        docker run -p 8888:8888 -v $(pwd):/appdata -d v1shwa/audiobox
  - Set a custom password for jupyter notebook. (default: `password`)
        
        docker run -p 8888:8888 -v $(pwd):/appdata -e NB_PASSWORD="mynewpass"  -d v1shwa/audiobox
    
    You can now access the jupyter notebook at [localhost:8888](http://localhost:8888/)

### What's Included?
 - ffmpeg
 - Python 3.6
 - pip
 - numpy
 - scipy
 - scikit-learn
 - pandas
 - matplotlib
 - jupyter
 - pydub
 - pyaudio
 - nussl
 - librosa
 - peakutils
 - mir_eval
 - auditok
 - pyAcoustics

### Feedback/Contributing
Feature requests, PRs for new tools & other suggestions are always welcome.

### License
[The MIT License](./LICENSE)

# anlaysis of audio/video stream

a typical test enviroment as below
![deploy](./draw.io/004-analyzer-deploy.png)

## 1. Audio codec validity

The system (Camera) under test does codec with the specific audio source and outputs the result to test system (Tester), then the test system compares the audio source and result.


### Scenarios/User story

#### a) Simple test

As a streaming media system tester, I want to test the audio validity for some kind of audio codec ( G711, AAC ...), So that I can validate the audio quality.

#### b) Latency of the media system

As a streaming media system tester, I want to test the time between audio generate to the rendering at last, So that I can calc the latency of audio system.


### 2. Video codec validity

The system (Camera) under test does codec with the specific video source and outputs the result to test system (Tester), then the test system compares the video source and result.

### Scenarios/User story

#### a) Simple test

As a streaming media system tester, I want to test the camera video validity for some kind of video codec ( H.264, VP9 ...), So that I can validate the video quality.

#### b) Latency of the media system

As a streaming media system tester, I want to test the time between video generate to the rendering at last, So that I can calc the latency of video system.



## 3. Audio and video sync check

In the streaming media system, the audio/video's codec and tranport are separated usually , the audio and video lantency are different. If the diffence is larg, as a consequence what you heared would not you see.

#### b) Audio and video sync the media system
As a streaming media system tester, I want to test the time between video and audio asynchronization, so that I can tell if the system is work for user.
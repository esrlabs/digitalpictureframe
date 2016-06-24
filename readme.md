# Digital Picture Frames with Presence Recognition
a ESRLabs 2016 labdays project

## Vision
Build multiple digital picture frames displaying our team. Experiment with Bluetooth LE: detect who's phone is nearby and highlight the corresponding teammate on the frame.

## Architecture

#### Smartphone
Presence recognition is realized by a smartphone app for android detecting BLE beacons signal emitted by each frame.

#### Broker
A mqtt broker receives the presence information from each smartphone and informs the corresponding frame about

#### Digital Picture Frames
Each frame is equipped with a BLE beacon emitting an unique signal. Each frame listens to the broker and displays pictures of detected teammates using javascript.

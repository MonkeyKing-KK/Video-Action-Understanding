# Video-Action-Understanding
## Definitions
Action Recognition(AR): is the process of classifying a complete input(either an entire video or a specified segment) by the action occurring in the input. <br>
Action Prediction(AP): is the process of classifying an incomplete input by the action yet be to observed. Including action anticipation(AA) and early action prediction(EAP). <br>
Temporal Action Proposal(TAP): is the process of partitioning an input video into segments(consecutive series of frames) of action and inaction by indicating start and end markers of each action instance. Temporal Action Localization/Detection(TAL/D) is the process of creating temporal action proposals and classifying each action. <br>
Spatiotemporal Action Proposal(SAP): is the process of partitioning an input video by boteh space(bounding boxes) and time(per-frame OR start and end markers of a segment) between regions of action and inaction. Spatiotemporal Action Localization/Detection(SAL/D) is the process of creating spatiotemporal action proposals and classifying each frames's bounding boxes(or action tubes when a linking strategy is applied) <br>
## Models
### CNN Models
Reducing computational costs: C3D, P3D, R(2+1)D, ARTNet, MFNet, GST, CSN <br>
Recognizing long-range temporal dependencies: LTC-CNN, NL, Timeception, STDA <br>
Other: TSM, TrajectoryNet <br>
### RNN Models

### State-of-the-Art Model Architecture
Action Recognition Models: <br>
Single-stream architectures: extract one 2D or 3D input feature from a video and output of the CNN is the prediction. <br>
Two-stream ofr multi-streams architectures: one stream for RGB learning and one stream for motion feature learning <br>
Temporal segmentation architectures: address long-term dependencies of actions. TSN, T-C3D, TRN, ECO, SlowFast <br>
Two-stage learning: the first stage uses temporal segmentation methods to extract segment embedded feature vectors, the second stage trains on those features. 3D-fusion, CNN+LSTM

**Overview**

We introduce a deep learning approach to track multi-
ple, non-overlapping repeated action sequences in dance
videos. It addresses challenges in understanding repeated
actions and their variations due to factors like speed, dura-
tion, and environmental conditions. We build on the archi-
tecture of Google’s RepNet, a transformer-based model ca-
pable of class-agnostic action repetition counting, by adding
a multilayer perceptron model called Sequence Segmenter
Model (SSM) to identify boundary video frames between
different action sequences. We then train this new model on
an synthetic dataset that we create by concatenating videos
from UCF101, a large scale action recognition dataset. We
then propose an evaluation dataset consisting of 100 dance
videos to assess the performance of this model. To under-
stand the effectiveness of our SSM addition, we also a pro-
pose an approach to assess the performance of a pretrained
RepNet model available from the original paper and a Rep-
Net model that we re-train on our synthetic UCF101 dataset
on the same evaluation dataset. We consider metrics such
as precision, recall, F1 score, mean absolute errors, allow-
ing us to investigate whether our modification of the RepNet
architecture enhances action recognition in the dance video
domain.

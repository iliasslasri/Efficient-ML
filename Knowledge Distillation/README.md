# Knowledge Distillation

Slides : [Knowledge Distillation]

Problem: Tiny models are hard to train.

Solution: Train a bigger model and then distill the knowledge to a smaller model. We have a teacher network and a student network. The teacher network is a bigger model and the student network is a smaller model. The teacher network is trained on the dataset and then the student network is trained on the same dataset but with the teacher network's output as the target. The student network tries to mimic the teacher network's output.
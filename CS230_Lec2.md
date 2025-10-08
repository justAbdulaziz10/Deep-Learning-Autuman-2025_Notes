CS230 – Lecture 2: Supervised, Self-Supervised, & Weakly Supervised Learning
**Date:** 2025-10-08  
**Instructor:** Kian Katanforoosh

Model = Architecture + Parameters
• Architecture: The blueprint or design of the neural network.
• Parameters: The numerical values (weights, biases) the model learns during training.
• Feature Engineering: Manual - humans specify features.
• Feature Learning: Automatic - the network figures out features during training.
• Encoding: Any representation in vector form.
• Embedding: An encoding where closeness = similarity.
• One-Hot Vector: Exactly one thing is true.
• Multi-Hot Vector: Multiple things can be true at the same time.
• Use a known proxy project to evaluate how much data you need.
• Be scrappy. For example, if you'd like to find a good resolution of images to use for your data, but don't have time for a large scale experiment, approximate human-level performance by testing your friends as classifiers.
• Your data collection strategy is critical to the success of your project. (If applicable) Don't hesitate to get out of the building.
• You can gain insights on your labelling strategy by using a human experiment.
• Refer to expert advice to earn time and be guided towards a good direction.
• In face verification, we have used an encoder network to learn a lower dimensional representation (called "encoding") for a set of data by training the network to focus on non-noisy signals.
• Triplet loss is a loss function where an (anchor) input is compared to a positive input and a negative input. The distance from the anchor input to the positive input is minimized, whereas the distance from the anchor input to the negative input is maximized.
• You learned the difference between face verification, face identification and face clustering.

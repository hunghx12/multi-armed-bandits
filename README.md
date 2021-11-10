# Multi-armed bandits: LinUCB and MLinUCB

This is the implementation of LinUCB and MLinUCB.
Great appreciation to the teaching team of Statistical ML, the University of Melbourne for such an exciting assignment!

## Data format

Each row comprises 103 space-delimited columns of integers:
* Column 1: The arm played by a uniformly-random policy out of 10 arms;
* Column 2: The reward received from the arm played (0-1);
* Column 3: An indicator for missing rewards (for MLinUCB). 1: reward is available or 0: reward is missing.
* Columns 4–103: The 100-dim flattened context: 10 features per arm, first the features for arm 1, then arm 2, etc. up to arm 10.

Due to the University's copyright restrictions, the dataset will not be disclosed.

## Methods:

* play(self, context): Plays an arm based on the provided context.
* update(self, arm, context, reward): Updates the internal state of the MAB with given rewards.

## References

LinUCB: https://arxiv.org/pdf/1003.0146.pdf
MLinUCB: https://arxiv.org/pdf/2007.06368.pdf
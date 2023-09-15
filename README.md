# larva-tagger-benchmark

This project aims to benchmark previously published animal pose estimation tools on video 
recordings of Drosophila larvae. The goal is to identify a tool that is best suited for the application on 
large-scale video recordings of larvae. We require a tool that is capable of tracking multiple larvae and extracting 
5-11 spine points per larva per frame.

This repository contains notebooks that might be useful to perform the benchmark on your own data.

We included four trackers in this benchmark:
- MWT (Multi-Worm Tracker, [Paper](https://doi.org/10.1038%2Fnmeth.1625))
- Tierpsy ([Paper](https://doi.org/10.1038%2Fs41592-018-0112-1))
- WF-NTP (Wide field-of-view Nematode Tracking Platform, [Paper](https://doi.org/10.1038/s41596-020-0321-9))
- DeepLabCut multi-animal ([Paper](https://www.nature.com/articles/s41592-022-01443-0))

To ensure a fair comparison, we developed an automized hyperparameter-optimization for the parameter-based 
trackers (MWT, Tierpsy, and WF-NTP). The code for the optimization can be found 
in the [larva-tagger-tune repository](https://github.com/Lilly-May/larva-tagger-tune).
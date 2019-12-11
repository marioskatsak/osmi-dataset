ROSMI Dataset
=========================

_Authors: Miltiadis Marios Katsakioris, Ioannis Konstas and Helen Hastie_

Download Link
-------------

**[Download the full release of the ROSMI dataset here (ZIP)](https://github.com/tuip)**

Description
-----------

The ROSMI dataset is a new multimodal corpus of visual and natural language instruction pairs, in the domain of emergency response, whereby the subjects are given a scene in the form of a map and are tasked to write an instruction to command a conversational assistant to direct a number of robots and autonomous systems to either inspect an area or extinguish a fire. These types of emergency scenarios usually have a central hub for operators to observe and command humans and RAS to perform specific functions aided by 'Command and Control' style interfaces, where the robotic assets are visually observable as an overlay on top of the map.
These map-based interfaces are thus dynamic in nature, adding an extra layer of complexity that we attempt to capture herein. Although our focus is on emergency response resolution with robots, the data and collection method are applicable to collaborative tasks that involve moving objects with respect to a 2D map, such as in gaming and human instruction-giving. 
Our contributions are summarised as follows: 
1) a novel dataset comprising of map-based instructions for human-robot interaction;
2) the accompanying structured metadata that can be used to train instruction understanding models.


Please refer to [our LREC2020 paper](https) for 
a detailed description of the dataset.

Images are only necessary if vision algorithms are to be employed. Otherwise, the location and ID of all blocks are in the JSONs (<1Mb vs 167Mb for images)

Contents
--------

### Files ###

* trainset.csv – the training set
* devset.csv – the development set
* testset.csv – the challenge test set (meaning representations only)
* testset_w_refs.csv – evaluation test set with reference natural language 
    utterances

### CSV Data Fields ###

- **mr** – textual meaning representation (MR)
- **ref** – corresponding natural language utterance (human reference)

Note that several human references correspond to a single MR, i.e., multiple 
lines contain the same MR.

Citing
------

If you use this dataset in your work, please cite the following paper:

```
@inproceedings{


}
```

License
-------

Distributed under the [Creative Commons 4.0 Attribution-ShareAlike license
(CC4.0-BY-SA)](https://creativecommons.org/licenses/by-sa/4.0/).


Acknowledgements
----------------

This research received funding by Seebyte, Datalab and MASTS-S. This work was also supported by the EPSRC funded ORCA Hub (EP/R026173/1, 2017-2021).

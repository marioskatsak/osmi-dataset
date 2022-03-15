ROSMI Dataset
=========================

_Authors: Miltiadis Marios Katsakioris, Ioannis Konstas and Helen Hastie_

Download Link
-------------

**[Download the full release of the ROSMI dataset here (ZIP)](https://drive.google.com/open?id=12dmeL1SIgpt-8RKeR4Rl_RhJ9yJAo73v)**

Description
-----------

The ROSMI dataset is a new multimodal corpus of visual and natural language instruction pairs, in the domain of emergency response, whereby the subjects are given a scene in the form of a map and are tasked to write an instruction to command a conversational assistant to direct a number of robots and autonomous systems to either inspect an area or extinguish a fire. These types of emergency scenarios usually have a central hub for operators to observe and command humans and RAS to perform specific functions aided by 'Command and Control' style interfaces, where the robotic assets are visually observable as an overlay on top of the map.
These map-based interfaces are thus dynamic in nature, adding an extra layer of complexity that we attempt to capture herein. Although our focus is on emergency response resolution with robots, the data and collection method are applicable to collaborative tasks that involve moving objects with respect to a 2D map, such as in gaming and human instruction-giving. 
Our contributions are summarised as follows: 
1) a novel dataset comprising of map-based instructions for human-robot interaction;
2) the accompanying structured metadata that can be used to train instruction understanding models.


Please refer to [our ICMI2020 paper](https) for 
a detailed description of the dataset.

Images are only necessary if vision algorithms are to be employed. Otherwise, the location and ID of all blocks are in the JSONs (<1Mb vs 167Mb for images)

Contents
--------

### Files ###

* ROSMI.json – all 783 scenarios
* scenario[0-6].json – 7 json files containing the static meta-data of each unique map.
* images – folder containing all map images

### ROSMI.JSON Data Fields ###

  * "imgid" - ID of the corresponding image of the map,
  * "split" - train/val/test identification,
  * "image_filename" -  name of the corresponding image file,
  * "scenario_items" - name of the corresponding map file,
  * "landmarks"  - list of all mentioned landmarks and their corresponding annotations and meta-data,
  * "dynamo_obj" - list of all dynamic objects that make each scenario unique from each other,
  * "gold_coordinates" - Gold Standard Coordinate to be predicted,
  * "sentid" - id of sentence/scenario,
  * "sentence" - sentence of the corresponding scenario
  * "gold_pixels" - Gold Standard Pixels to be predicted
  
  

Citing
------

If you use this dataset in your work, please cite the following paper:

```
@inbook{10.1145/3382507.3418861,
author = {Katsakioris, Miltiadis Marios and Konstas, Ioannis and Mignotte, Pierre Yves and Hastie, Helen},
title = {ROSMI: A Multimodal Corpus for Map-Based Instruction-Giving},
year = {2020},
isbn = {9781450375818},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3382507.3418861},
abstract = {We present the publicly-available Robot Open Street Map Instructions (ROSMI) corpus: a rich multimodal dataset of map and natural language instruction pairs that was collected via crowdsourcing. The goal of this corpus is to aid in the advancement of state-of-the-art visual-dialogue tasks, including reference resolution and robot-instruction understanding. The domain described here concerns robots and autonomous systems being used for inspection and emergency response. The ROSMI corpus is unique in that it captures interaction grounded in map-based visual stimuli that is both human-readable but also contains rich metadata that is needed to plan and deploy robots and autonomous systems, thus facilitating human-robot teaming.},
booktitle = {Proceedings of the 2020 International Conference on Multimodal Interaction},
pages = {680–684},
numpages = {5}
}
```

License
-------

Distributed under the [Creative Commons 4.0 Attribution-ShareAlike license
(CC4.0-BY-SA)](https://creativecommons.org/licenses/by-sa/4.0/).


Acknowledgements
----------------

This research received funding by Seebyte, Datalab and MASTS-S. This work was also supported by the EPSRC funded ORCA Hub (EP/R026173/1, 2017-2021).

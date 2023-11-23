# SCCI

## The data repository for the “Electrospinography (ESG) for non-invasively recording spinal sensorimotor networks in humans” project.

### Non-Invasive Brain-Machine Interface Systems Lab, IUCRC BRAIN, University of Houston.


## Paper Reference:

Steele AG, Faraji AH, Contreras-Vidal JL. (2023) Electrospinography for non-invasively recording spinal sensorimotor networks in humans.


Journal of Neural Engineering, in press. DOI: (pending)


## Overview:
- The project proposes a novel non-invasive method for directly measuring spinal sensorimotor networks.
- Focus is on evaluating the feasibility of Electrospinography (ESG) for assessing spinal sensorimotor networks during single-joint movements.
- Synchronous recording of electroencephalography (EEG), electromyography (EMG), and ESG during lower-limb tasks in neurologically intact subjects (NIS).



## Data Structure:


The dataset follows the structure outlined below, using subject NIS005 as an example:

NIS005

├── Subject Code

├── EEG

├── Lumbar

├── Lumbar Noise

├── EMG

└── srate   

### Subject Code:
In this data structure, 10 healthy subjects (NIS) perform specific movements, including right and left plantarflexion (RPF, LPF), and right and left knee flexion (RKF, LKF). Each participant is assigned a code from 1 to 10 (e.g., NIS005).

An illustration of the experiment with a participant performing knee flexion:

![Media1 (2)](https://github.com/uhbmilab/SCCI/assets/151566358/7107957e-c8a7-45a5-8428-dcaac982b5b1)


### EEG:

EEG

├── Rest 

├── LPF [28 x X]

├── RPF [28 x X]

├── LKF [28 x X]

└── RKF [28 x X]

EEG data collected with 28 channels following the modified 10-20 international standard arrangement.

### Lumbar:

Lumbar

├── Rest 

├── LPF [15 x X]

├── RPF [15 x X]

├── LKF [15 x X]

└── RKF [15 x X]

Fifteen electrodes are positioned on the thoracic and lumbar sections of the spine (refer to the picture) for specified movements (RPF, LPF, RKF, and LKF).

![Pic4](https://github.com/uhbmilab/SCCI/assets/151566358/07f03267-a87b-4cae-b779-fda7578e1d16)

The Lumbar section is a matrix of 15 by X for movement tasks performed in five blocks of five repetitions, totaling 25 receptions per movement (e.g., 15x16000 for RPF).

### Lumbar Noise:

LumbNoise

├── Rest 

├── LPF [4 x X]

├── RPF [4 x X]

├── LKF [4 x X]

└── RKF [4 x X]

Four sensors as the reference for noise represented in a matrix of the size 4 by X (e.g., 4x16000 for RPF).

![Pic2222](https://github.com/uhbmilab/SCCI/assets/151566358/3515f780-7019-4a1a-bb93-c53661221a4d)


### EMG:

EMG

├── Rest 

├── LPF [32 x X]

├── RPF [32 x X]

├── LKF [32 x X]

├── RKF [32 x X]

└── Names [8 x 2]

EMG sensor placement includes the left and right rectus femoris (RF), the semitendinosus portion of the medial hamstrings (MH), the tibialis anterior (TA), the gastrocnemius (MG), and the lateral aspect of soleus (SOL) muscles.

![Pic5](https://github.com/uhbmilab/SCCI/assets/151566358/4b81ce5a-5cd9-46d3-a711-b487d90d5aae)


### Srate:
The recorded data had a sample rate of 1000 Hz.

## Funding:
This work was supported by The Institute for Rehabilitation and Research (TIRR) Mission Connect grant (Award #021-112). The funders were not involved in the design of the study, the collection, analysis, and interpretation of the experimental data, the writing of this article, or the decision to submit this article for publication.

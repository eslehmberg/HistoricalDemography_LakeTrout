## Microsatellite Library Preparation for Lake Trout (*Salvelinus namaycush*)

#### Original protocol here: Marcy-Quay, B., Wilson, C. C., Osborne, C. A., & Marsden, J. E. (2023). Optimization of an amplicon sequencing-based microsatellite panel and protocol for stock identification and kinship inference of lake trout (Salvelinus namaycush). Ecology and Evolution, 13, e10020. https://doi.org/10.1002/ece3.10020
#### Protocol modifications: Caleigh Smith (Ontario Ministry of Natural Resources) and Emma Lehmberg (Lakehead University & IISD ELA)

## Before beginning 

1. Complete a HotSHot extraction (see inluded protocol). 
2. Qubit a random set of samples from each plate (6-10). If the concentration is extremely high, these may need to be diluted (amount TBD). For Qubit protocol, see product instructions
3. *Clean your workspace before and after you work, always*. This is more important than anything. Use a 20% bleach solution to wipe down all surfaces and tools. Let everything dry before use.

## 1. PCR 1 

Fill out the excel sheet that calculates amounts needed (this should not vary as long as you're doing a full plate). It helps to track which samples are complete.

### Recipe: 10uL volume
- 5uL Qiagen Multiplex PCR Plus Master Mix
- 3.5uL DNA
- 1uL RNAase-free water
- 0.5uL 2uM primers (pooled in equal amounts)

### Thermocycler settings

|Step         | Temperature (C) | Time (sec)     |
|:-----------:|:---------------:|:--------------:|
| Initial Denaturation |   95   | 300 (5 minutes)|
|                 | __35 cycles__ |                      |
| Denaturation         | 95     | 30             |
| Annealing            | 60     | 90             |
| Extension            | 72     | 90             |
|                 | __Final Extension__ |                |
| Extension            | 68     | 600 (10 minutes)|

TOTAL RUN TIME: 2 hours, 17 minutes

Run the same random samples on the Qubit after PCR1 is complete. You only need to do this for the first few plates. Once you're sure it's working, this step can be bypassed. 

It's sometimes worth also running some of those samples on a gel if you have time, at least for the first few plates.

## 2. PCR 2 

###(*see below for Truseq modifications*)

### Recipe: 10uL volume per well
- 2 μL NEB OneTaq HotStart Buffer
- 1.5uL PCR1 product
- 5.85uL RNAase-free water
- 0.2 μL 10 mM dNTPs
- 0.2 μL of 10 μM i5 index adapter
- 0.2 of 10 μM i7 index adapter
- 0.05 μL of NEB OneTaq HotStart Polymerase

### Thermocycler settings

|Step         | Temperature (C) | Time (sec)     |
|:-----------:|:---------------:|:--------------:|
| Initial Denaturation |   94   | 60 (2 minutes) |
|                | __10 cycles__ |                     |
| Denaturation         | 94     | 30             |
| Annealing            | 62     | 60             |
| Extension            | 68     | 60             |
|                | __Final Extension__ |               |
| Extension           | 68     | 500 (5 minutes) |

TOTAL RUN TIME: 33 minutes

## 3. Pooling and cleaning

a. Pool all samples in single plates, so that you have the same number of tubes as you have plates.

b. Aliquot 200uL from each pooled sample and use Beckman-Coulter Ampure XP magnetic beads to clean any fragments (0.625x bead:sample ratio for large fragments).

c. Do a second clean for small fragments using 0.85x ratio of bead:sample using the same sample you just cleaned.

d. Use the qubit to quantify each pooled sample.

## Notes for using Truseq adaptors 
*The indexing protocol is different for the Truseq indexes though. The i05 indexes are in plate format and should be 5uM each. I make a i07 ‘cocktail’ with 106uL of 10uM i07 primer and 530uL of Mastermix. In a new plate for indexing I combine 6uL of the i07 cocktail, 2uL of the respective i05 indexes and 2uL of amplified product. The cycling conditions I’ve been using are as follows:

 

95° - 15 min

10 cycles of

95° - 10 sec

65° - 30 sec

72° - 30 sec

Followed by 72° - 5 minutes and a 4° hold

 

I followed the bead size selection in the Ben MQ paper, though it is different from what I do in other protocols.*  
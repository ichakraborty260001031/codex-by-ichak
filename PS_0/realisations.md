## What I learnt after trying all the different hyperparameters

So I tried about 30 combinations of different parameters, and finally reached to a 0.67 validation accuracy.

### Key Insights:

* **Learning Rate Dynamics:** Too high of a learning rate cant reduce loss after a certain range. lr from 0.008-0.011 is the sweet spot.
* **Network Depth:** A denser network (4 blocks) allow better fitting but need higher epoch and adequate patience to converge.
* **Dropout Balance:** High dropouts underfit and low ones overfit, the best for my experiment was 0.25.
* **Data Augmentation:** Augmentation provides a huge boost to validation accuracy , the random flipping, shifting and rotation, allows for better generalisation.

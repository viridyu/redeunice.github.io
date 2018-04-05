
[back to homepage](https://viridyu.github.io/)

## 20180327

> 1. When I use full_cycle, the l1 loss is hard to converage to the value for the half_cycle (5 vs 1). Whereas the gan loss could converage quickly. So the gan loss and l1 loss are not balanced. What if I set the hyper-paramater for l1 loss larger? Can it make the two kinds of losses converage at the same time? Another experiment is needed to prove this thought. **This seems to be wrong**
> 2. Why in half_cycle, the G loss is smaller than D loss? **It's because of the display, not the network itself.**

## 20180329

> 1. In the WGAN, the sigmoid should not be applied in discriminator.
> 2. In wgan-gp, the Batch-norm in D should be deleted.
> 3. **try dilated convolutional layer in my model.**

## 20180405

> 1. cannot guarantee the contexture similarity between the synthesized and the real images
> 2. use the variation similarity loss?
> 3. the contexture similarity can be constrained by watershed filter loss.

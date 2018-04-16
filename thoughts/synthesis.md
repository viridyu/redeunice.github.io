
[back to homepage](https://viridyu.github.io/)

## 20180327

> 1. When I use full_cycle, the l1 loss is hard to converage to the value for the half_cycle (5 vs 1). Whereas the gan loss could converage quickly. So the gan loss and l1 loss are not balanced. What if I set the hyper-paramater for l1 loss larger? Can it make the two kinds of losses converage at the same time? Another experiment is needed to prove this thought. **This seems to be wrong**
> 2. Why in half_cycle, the G loss is smaller than D loss? **It's because of the display, not the network itself.**

## 20180329

> 1. In the WGAN, the sigmoid should not be applied in discriminator.
> 2. In wgan-gp, the Batch-norm in D should be deleted.
> 3. **try dilated convolutional layer in my model.**  gan loss starts to expand at very begining!!!!

## 20180405

> 1. cannot guarantee the contexture similarity between the synthesized and the real images
> 2. use the variation similarity loss?
> 3. the contexture similarity can be constrained by watershed filter loss.
> 4. sobel operator?


## 20180411 partition1
> 1. half: epoch 160; lambda 300
> 2. sobelLoss: epoch 130; lambda 100,30
> 3. variationLoss: epoch 70; lambda 100,?30
> 4. poolingLoss: epoch 150; lambda 100,100
> 5. wgan_gp: epoch 140; lambda 10
> 6. l2: epoch ?; lambda 300
> 7. dilated: bad
> 8. half: bad; lambda 100
> 9. maxpoolingLoss: bad
> 10. sobelLoss_rise: epoch 140; lambda 100,100; rise epoch0~50; step 2


## 20180416 partition2
> 1. half: epoch 110; lambda 300
> 2. sobelLoss_rise: bad; lambda 300,100; rise epoch0~50; step 2
> 2. sobelLoss_rise_lambda30: epoch 110; lambda 300,30; rise epoch0~60; step0.5

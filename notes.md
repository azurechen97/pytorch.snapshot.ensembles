## Goal

- [ ] Improve the method's performance (e.g. achieve lower error if the underlying task is classification)
- [ ] Improve the method's running time
- [ ] Simplify the method (e.g. show that some key components of the method can be removed without significantly affecting its performance)
- [ ] Generalize the method (i.e. show that your modification allows the method to work on a setting where the original one does not work)

You should submit a 4-page long report, including what your goal was, a detailed description of your extension of the original method, empirical results and discussion including a comparison with the original method, and a conclusion section that summarizes your findings (which might be negative findings -- i.e. it is possible that you don't achieve your goal even after significant effort, in which case you should report what you tried anyway: you will not be penalized if, ultimately, your extension doesn't 'work').

## Ideas
- [ ] Other than cyclic cosine annealing
    - large learning rate multiple times (because only one step is not enough for escaping the local minimum)
    - then discretely drop to small learning rate
- [ ] why update learning rate at each iteration?
- [x] why last m?
- [ ] why average? how about max and voting?
- [ ] use large first then cosine
- [ ] save the model after each epoch

## Result

### baseline
Test set: Average loss: 2.4204, Accuracy: 7394/10000 (74%)

### se
Test set: Average loss: 1.9214, Accuracy: 7530/10000 (75%) (initial_lr = 0.2, M=6)
(initial_lr = 0.2, M=10)
### se epoch
Test set: Average loss: 1.8335, Accuracy: 7655/10000 (77%) (initial_lr = 0.2, M=6)
(initial_lr = 0.2, M=10)

### min loss
Test set: Average loss: 1.9310, Accuracy: 7530/10000 (75%) (initial_lr = 0.2, M=6)
(initial_lr = 0.2, M=10)

### min val loss
(initial_lr = 0.2, M=6)
(initial_lr = 0.2, M=10)

### vote
Test set: Average loss: 1.9250, Accuracy: 7537/10000 (75%) (initial_lr = 0.2, M=6)
(initial_lr = 0.2, M=10)
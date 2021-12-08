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

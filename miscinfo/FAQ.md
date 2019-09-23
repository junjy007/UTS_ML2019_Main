# A2

* Word Count
Follow the sepcification, as page number in subject outline may not be a good
measurement of the volume as the document contains graphics, tables and other
formatting matters. The volume is suggestive and not requirement anyway, as
long as your description is clear, and your argument logically supports what
you did, it is fine.

* Design Data Structures/Plan Data Models and Tests
"Plan Data Models" is mainly for practical data modelling task. "Data
Structure" is mainly a concern for algorithm implementation. But the there is
no black/white distinction here. As when modelling some data, you still need
to consider data/model parameter management; while implementing algorithm
requires you to consider the data model. Maybe it is just the amount of focus
you allocate to each aspect differs for the two tasks.

For test, data modelling task needs a plan to demo your solution is
effective. Algorithm implementation task needs a plan to show your
implementation is correct.

* Video Highlights
Were I to do it, I would talk for ~1min on each of the following points
1. Why you do this and the challenge
2. Your solution to the challenges
3. What you have learned.

* Ethical Discussion
From the specification:
The report includes discussions about the social/ethical aspect of the
proposed technique/project. You can adopt one or more ethical models, such as
the utilitarian approach or the Kantian duty-based approach. You should
anticipate the potential misuses of your technique.


## Specific to Practical Data Modelling

* One algorithm or many?

The number of models is not essential. Use multiple algorithms is ONE of the
means that you can use to support your design / choice of the model.

* Can I use XXX data?

As long as you can convince people it is worthy doing in both aspects:
1. for some *feasible* good: useful / helpful / or just interesting
2. there are some challenges worhty your 4-week effort

## Specific to Algorithm Implementation

* Can I implement KNN?

If you mean the following, 

```
import numpy as np
from collections import Counter
def KNN(query_x, training_x, training_y, k=1):
  distances = np.linalg.norm(training_x - query_x), axis=1)
  sort_index = np.argsort(distances)
  b = Counter(training_y[sort_index[:k]])
  return b.most_common(1)
```

No, this is too simple. But you can try to imporve the spatial/time
efficiency or the way of voting etc. to make it a worthy project.

* Performance of my implementation?

It is not required to be competative with industry level implementations. You
need only to show that your implementation works.
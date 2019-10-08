# A2

* Word Count

Follow the sepcification, as the page number in subject outline may not be a good measurement of the volume as the document contains graphics, tables and other formatting matters. The volume is suggestive and not requirement anyway, as long as your description is clear, and your argument logically supports what
you did, it is fine.

* Design Data Structures/Plan Data Models and Tests

"Plan Data Models" is mainly for practical data modelling task. "Data Structure" is mainly a concern for algorithm implementation. But there is no black/white distinction here. As when modelling some data, you still need to consider data/model parameter management; while implementing algorithm requires you to consider the data model. Maybe it is just the amount of focus you allocate to each aspect differs for the two tasks.

For the test, data modelling task needs a plan to demo your solution is effective. Algorithm implementation task needs a plan to show your implementation is correct.

* Source Code in Report

Yes, codes are allowed and even recommended, as they are the most accurate way of demoing your work. On the other hand, if some code block is large and not directly relevant, e.g. visualisation helper functions, you can put it away in a separate area and fold it before exporting PDF. Moreover, if a code block depends on its context and not easily moved, you can hide the code (and optionally keep its output) using colab editor "EDIT:SHOW/HIDE CODE". 

* Video Highlights

Were I to do it, I would talk for ~1min on each of the following points
1. Why you do this and the challenge
2. Your solution to the challenges
3. What you have learned.

* Ethical Discussion

From the specification: The report includes discussions about the social/ethical aspect of the proposed technique/project. You can adopt one or more ethical models, such as the utilitarian approach or the Kantian duty-based approach. You should anticipate the potential misuses of your technique.

* Submission

Similar to A1, you need to submit a PDF file to TurnitIn on UTSOnline, which includes a link to your notebook in your github repo. 

If there are more than one people in a team, only one submission is needed, but you need to mention at the beginning of your report all team members' Full Name
and Student ID. 

For 31005 students, please upload the video pitch to YouTube and include the link in your report.

ALL LINKS MUST BE PROVIDED IN PLAIN TEXT. You can embed the link for convenience but plain text URL must be present in the report lest the embedded link be stripped by some security software.


## Specific to Practical Data Modelling

* One algorithm or many?

The number of models is not essential. Use multiple algorithms is ONE of the means that you can use to support your design/choice of the model.

* Can I use XXX data?

As long as you can convince people it is worth doing in both aspects:
1. for some *feasible* good: useful / helpful / or just interesting
2. there are some challenges worthy your 4-week effort

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

No, this is too simple. But you can try to improve the spatial/time efficiency or the way of voting etc. to make it a worthy project.

* Performance of my implementation?

It is not required to be competitive with industry-level implementations. You need only to show that your implementation works.

# A3

* Word Count

No hard requirement. For both 32513 and 31005, try to make a report as concise as possible while covering points in the specification. As a guideline, a typical answer (31005) may contain 1000 words, and a typical proposal (32513) may contain 1200 words. Both word counts are text body only.


Do NOT inflate the report with enlarged figures or unorganised program outputs.

* Video Pitch (32513)

See above (video pitch for 31005 A2). Of course, the pitch should be relevant to your proposal, e.g. replacing "what learned from te project" with "deployment/commercialisation considerations".

You can talk slides or present the pitch by yourself in front a camera, or both.

* PDF Submission: Is it compulsory to export the PDF file from Jupiter Notebook?

No. A3 does not require implementation. Thus if your report doesn't contain code but instead containing a lot of graphics that you would like to edit and use in other word processing software, stay with what you are familiar with.

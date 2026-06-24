# TakeMeter Planning

## Community

I chose FIFA World Cup discussions from public online communities. People share opinions, predictions, reactions, and analysis before, during, and after matches, which makes it a good topic for this project.

## Labels

### Analysis

Comments that explain something using facts, reasoning, tactics, or statistics.

Examples:

* Argentina controlled possession for most of the match.
* France created more scoring chances because of their attacking pressure.

### Prediction

Comments that predict a future result or outcome.

Examples:

* Brazil will make the semifinals.
* Spain is going to win the group.

### Reaction

Comments that mainly express feelings or emotions.

Examples:

* What an amazing goal!
* I can't believe they lost that game.

### Other
Comments that do not fit Analysis, Prediction, or Reaction. These are usually questions, requests for information, or logistical discussion.

Examples:
* Where can I buy a Bosnia jersey?
* Which light rail station should I use?

## Hard Edge Cases

Some comments include both analysis and prediction. If the main point is predicting what will happen, I will label it Prediction. Otherwise, I will label it Analysis. Some comments may not fit any of the three main categories. These comments will be labeled Other.

## Data Collection Plan

I will collect at least 200 public FIFA World Cup comments and posts. If I do not have enough examples for one label, I will collect more examples for that category.

## Evaluation Metrics

I will use accuracy, precision, recall, F1 score, and a confusion matrix to see how well the model performs.

## Definition of Success

I would consider the project successful if the fine-tuned model performs better than the baseline model and can correctly classify most comments.

## AI Tool Plan

### Label Stress Testing

I will use AI to create example comments that are difficult to classify so I can test my labels.

### Annotation Assistance

I may use AI to suggest labels, but I will review every label myself before using it.

### Failure Analysis

I will use AI to help identify patterns in incorrect predictions and then review those patterns myself.


# Findings

## Connect 4 Dataset
### Neural Networks (aka MLP: Multi Layer Perceptron)
The specified layer sizes defines how many perceptrons should be in a hidden layer: (50, 60, 70) means that the first hidden layer has 50 perceptrons, the second has 60 and the third has 70 perceptrons.

Layer size (50):

             precision    recall  f1-score   support

          0       0.41      0.07      0.13      1289
          1       0.73      0.66      0.69      3341
          2       0.81      0.94      0.87      8882

    avg / total   0.75      0.79      0.76     13512

    [[  96  350  843]
    [  78 2209 1054]
    [  59  487 8336]]


Layer size (50, 50):

             precision    recall  f1-score   support

          0       0.41      0.18      0.25      1230
          1       0.65      0.82      0.72      3173
          2       0.89      0.88      0.89      9109

    avg / total   0.79      0.80      0.79     13512

    [[ 217  527  486]
    [ 109 2610  454]
    [ 197  904 8008]]


Layer size (50, 50, 50):

             precision    recall  f1-score   support

          0       0.44      0.19      0.26      1319
          1       0.74      0.72      0.73      3298
          2       0.85      0.93      0.89      8895

    avg / total   0.79      0.81      0.79     13512

    [[ 247  390  682]
    [ 176 2388  734]
    [ 135  447 8313]]


Layer size (50, 100, 50):


             precision    recall  f1-score   support

          0       0.40      0.26      0.32      1290
          1       0.73      0.73      0.73      3273
          2       0.87      0.91      0.89      8949

    avg / total   0.79      0.81      0.80     13512

    [[ 344  444  514]
    [ 221 2625  504]
    [ 257  604 7999]]


Layer size (50, 50, 50, 50, 50):

             precision    recall  f1-score   support

          0       0.39      0.23      0.29      1291
          1       0.71      0.75      0.73      3339
          2       0.87      0.91      0.89      8882

    avg / total   0.79      0.80      0.79     13512

    [[ 294  451  546]
    [ 213 2508  618]
    [ 247  586 8049]]


Layer size (50, 100, 100, 100, 50):

             precision    recall  f1-score   support

          0       0.35      0.27      0.30      1266
          1       0.73      0.71      0.72      3359
          2       0.87      0.90      0.88      8887

    avg / total   0.78      0.80      0.79     13512

    [[ 339  352  575]
    [ 307 2393  659]
    [ 315  542 8030]]


Layer size (50, 100, 150, 100, 50):

             precision    recall  f1-score   support

          0       0.33      0.33      0.33      1285
          1       0.72      0.71      0.72      3357
          2       0.88      0.88      0.88      8870

    avg / total   0.79      0.79      0.79     13512

    [[ 424  353  508]
    [ 369 2387  601]
    [ 476  562 7832]]


### kNN (k Nearest Neighbours)

n = 5:

             precision    recall  f1-score   support

          0       0.31      0.20      0.24      1279
          1       0.62      0.57      0.59      3339
          2       0.81      0.88      0.84      8894

    avg / total   0.72      0.74      0.73     13512

    [[ 254  382  643]
    [ 262 1900 1177]
    [ 294  769 7831]]

n = 10:

             precision    recall  f1-score   support

          0       0.44      0.10      0.17      1228
          1       0.71      0.60      0.65      3348
          2       0.81      0.94      0.87      8936

    avg / total   0.75      0.78      0.75     13512

    [[ 128  352  748]
    [  83 1993 1272]
    [  81  478 8377]]

n = 50:

             precision    recall  f1-score   support

          0       0.50      0.00      0.01      1311
          1       0.76      0.29      0.41      3373
          2       0.71      0.98      0.82      8828

    avg / total   0.70      0.71      0.64     13512

    [[   4  148 1159]
    [   3  962 2408]
    [   1  158 8669]]

n = 250:

    UndefinedMetricWarning: Precision and F-score are ill-defined and being set to 0.0 in labels with no predicted samples.

             precision    recall  f1-score   support

          0       0.00      0.00      0.00      1243
          1       0.76      0.08      0.15      3297
          2       0.68      0.99      0.81      8972

    avg / total   0.64      0.68      0.57     13512

### Random Forests

n = 10

             precision    recall  f1-score   support

          0       0.40      0.19      0.26      1299
          1       0.72      0.68      0.70      3296
          2       0.84      0.92      0.88      8917

    avg / total   0.77      0.79      0.77     13512

    [[ 244  356  699]
    [ 154 2237  905]
    [ 205  523 8189]]


n = 20

             precision    recall  f1-score   support

          0       0.42      0.14      0.21      1281
          1       0.75      0.69      0.72      3253
          2       0.84      0.94      0.89      8978

    avg / total   0.78      0.81      0.78     13512

    [[ 179  336  766]
    [ 129 2249  875]
    [ 119  400 8459]]


n = 50

             precision    recall  f1-score   support

          0       0.49      0.13      0.20      1319
          1       0.78      0.70      0.74      3319
          2       0.83      0.96      0.89      8874

    avg / total   0.79      0.81      0.79     13512

    [[ 168  348  803]
    [ 112 2307  900]
    [  64  285 8525]]


n = 250

             precision    recall  f1-score   support

          0       0.55      0.12      0.20      1254
          1       0.80      0.68      0.74      3390
          2       0.83      0.96      0.89      8868

    avg / total   0.79      0.82      0.79     13512

    [[ 152  316  786]
    [  65 2308 1017]
    [  59  256 8553]]


n = 500

             precision    recall  f1-score   support

          0       0.54      0.12      0.20      1251
          1       0.81      0.69      0.74      3399
          2       0.83      0.97      0.89      8862

    avg / total   0.80      0.82      0.79     13512

    [[ 149  300  802]
    [  88 2344  967]
    [  40  258 8564]]

### Naive Bayes

priors = None:

             precision    recall  f1-score   support

          0       0.13      0.09      0.11      1342
          1       0.37      0.23      0.28      3275
          2       0.70      0.82      0.75      8895

    avg / total   0.56      0.61      0.58     13512

    [[ 125  296  921]
    [ 257  756 2262]
    [ 566 1010 7319]]


priors = [0.6583, 0.2462, 0.0955] (exact values from dataset page https://archive.ics.uci.edu/ml/machine-learning-databases/connect-4/connect-4.names):

             precision    recall  f1-score   support

          0       0.14      0.17      0.16      1333
          1       0.30      0.62      0.41      3282
          2       0.76      0.45      0.56      8897

    avg / total   0.59      0.46      0.48     13512

    [[ 230  754  349]
    [ 345 2045  892]
    [1018 3917 3962]]


priors = [0.65, 0.25, 0.1]:

             precision    recall  f1-score   support

          0       0.15      0.18      0.16      1300
          1       0.31      0.64      0.41      3341
          2       0.77      0.42      0.55      8871

    avg / total   0.59      0.45      0.48     13512

    [[ 236  740  324]
    [ 383 2147  811]
    [ 977 4143 3751]]
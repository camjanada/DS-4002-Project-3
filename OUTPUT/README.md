# Outputs

## Model Results

| File | What it shows |
| --- | --- |
| [Confusion matrix](confusion_matrix.png) | True and predicted centuries for the 40 paintings in the original painting-level test set. The diagonal contains the 24 correct predictions. |
| [Test accuracy comparison](test_accuracy_comparison.csv) | Test-set size, model accuracy, majority-century baseline accuracy, and improvement in percentage points for both splits. |
| [Feature-selection cross-validation results](feature_selection_cv_results.csv) | Mean five-fold validation accuracy for 32, 64, 128, 256, and 512 ResNet-18 features, with and without artist grouping. |

The model achieved **60.0%** test accuracy on the painting-level split and **51.2%** on the artist-grouped split. These results used all 512 features and exceeded their respective baselines by **27.5** and **20.9 percentage points**. Cross-validation used the 157 training paintings. Mean validation accuracy peaked at **56.7% with 64 features** when grouped by artist and **58.5% with 128 features** without artist grouping.

## Exploratory Figures

| File | What it shows |
| --- | --- |
| [Date precision by century](date_precision_by_century.png) | The percentage of paintings in each century with an exact year, an approximate date, or a missing display date. |
| [Paintings by medium](paintings_by_medium.png) | The number of paintings in each medium recorded by the Met. |

See the [data README](../DATA/README.md) for context on the exploratory figures.

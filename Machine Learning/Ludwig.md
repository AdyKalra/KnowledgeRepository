# [Ludwig](https://uber.github.io/ludwig/)
[<img src="https://uber.github.io/ludwig/images/ludwig_logo.svg" align="center" width="650">](https://uber.github.io/ludwig/images/ludwig_logo.svg)

* Ludwig is a toolbox that allows to train and test deep learning models 


### Install
pip install ludwig

### Train
ludwig train
--data_csv file.csv
--model_definition definition.yaml

### Predict
ludwig predict
--data_csv data.csv
--model path_to_model

### Visualize
ludwig visualize
--visualization learning_curves
--training_statistics train_statistics.json

## Programmatic API
from ludwig import LudwigModel

'# train a model
model_definition = {...}
model = LudwigModel(model_definition)
train_stats = model.train(training_dataframe)
'# or load a model
model = LudwigModel.load(model_path)

'# obtain predictions
predictions = model.predict(test_dataframe)


# [Ludwig](https://uber.github.io/ludwig/)
* Ludwig is a toolbox that allows to train and test deep learning models 


### Install
```python
pip install ludwig
```
### Train
```python
ludwig train
--data_csv file.csv
--model_definition definition.yaml
```
### Predict
```python
ludwig predict
--data_csv data.csv
--model path_to_model
```
### Visualize
```python
ludwig visualize
--visualization learning_curves
--training_statistics train_statistics.json
```
## Programmatic API
```python
from ludwig import LudwigModel

# train a model
model_definition = {...}
model = LudwigModel(model_definition)
train_stats = model.train(training_dataframe)
# or load a model
model = LudwigModel.load(model_path)

# obtain predictions
predictions = model.predict(test_dataframe)
```

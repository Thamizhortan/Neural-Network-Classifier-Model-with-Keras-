# Neural-Network-Classifier-Model-with-Keras.
Setup:
1.Confirm that you have the latest version of Keras installed .
2.sudo pip install h5py

Save Your Neural Network Model to JSON
JSON is a simple file format for describing data hierarchically.

Keras provides the ability to describe any model using JSON format with a to_json() function. This can be saved to file and later loaded via the model_from_json() function that will create a new model from the JSON specification.

The weights are saved directly from the model using the save_weights() function and later loaded using the symmetrical load_weights() function.

The example below trains and evaluates a simple model on the Pima Indians dataset. The model is then converted to JSON format and written to model.json in the local directory. The network weights are written to model.h5 in the local directory.

The model and weight data is loaded from the saved files and a new model is created. It is important to compile the loaded model before it is used. This is so that predictions made using the model can use the appropriate efficient computation from the Keras backend.

Save Your Neural Network Model to YAML
This example is much the same as the above JSON example, except the YAML format is used for the model specification.

The model is described using YAML, saved to file model.yaml and later loaded into a new model via the model_from_yaml() function. Weights are handled in the same way as above in HDF5 format as model.h5.

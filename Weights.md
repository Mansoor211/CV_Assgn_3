# Weights Settings
The weights in below link are the final weights of VGG19 model after traning. These weights can be used by simply loading the model through the file 'model.json' using the below commands.
json_file = open('model.json', 'r')

loaded_model_json = json_file.read()

json_file.close()

loaded_model = model_from_json(loaded_model_json)

Then load the weights as given in the link below using these commands:

loaded_model.load_weights("model.h5")

Then compile the model and use it on the the test dataset to extract results.
loaded_model.compile(loss='categorical_crossentropy', metrics=['accuracy'])

Weights link Google drive : https://drive.google.com/file/d/1-3p2K83qj9UbqvcLty3XZTx10rmsJKPR/view?usp=sharing


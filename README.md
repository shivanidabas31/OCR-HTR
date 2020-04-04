Sequence diagram represents lifecycle or sequence of operations for a single instance (one image)

Input image is the data object represented here as an actor.

The diagram -

The main class in the python program will load the first image and pre-process it by performing certain operations like cropping/slicing, reshaping/flipping, and applying filters to generate multiple images to train the model

These generated images are 'processed_image'. It is not just one image but generating a lot of images using original to train model on small number of training data

After generating these images we move on to prepare our model which is the initialization step

Then you pass the array of your training images to train the model for specified steps and epochs

After training and getting the desired accuracy, we can start feeding the model with our new images to be read and extract the handwritten text

The output method will check if output_path has been specified or not. If not specified then it prints the output in consoler else it writes the output to text file at output path

Important point - The benefit of preprocessing is that we can train our model on limited dataset

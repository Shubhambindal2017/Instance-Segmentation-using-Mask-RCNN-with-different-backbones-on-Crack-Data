
### Task 2. Build a simple AI API

I built a simple REST-API for model created in task-1, I have kept it simple by using the implementation code to get the architecture and then load the weights, I might saved it into a frozen graph format and then do the inference on it.

To use flask on colab, I make use of flask-ngrok.

Dependencies :

    tensorflow  : 1.15.2
    keras       : 2.3.1
    flask       : 1.1.2
    flask-ngrok : 0.0.25

Now a bit about different folders.

Folders:

    static                : it will conntain the images uploaded to get the output from the MASK-RCNN model and also their output masked images.
    templates             : it contains 2 html files, home.html to get the uploaded image, while result.html to show the results as described in the task 2 sample api image.
    output_samples_of_api : it contains some screenshots of api samples
    input_images          : input images for which the output samples of api screenshots are taken.
  
 **task2_Rest_API_using_flask.ipynb** run each cells in this notebook, after executing the last cell you will get a *.ngrok.io link, click on it, to run the api.<br/>
 Example link - http://62678689f13b.ngrok.io/ (the actual link will differ from it)
 
 As the process is asynchronous, I have used a sleep time in flask app (last cell), increase this time a bit, if no output image is shown.
 

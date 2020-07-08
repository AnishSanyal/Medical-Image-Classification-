# flask/gunicorn web app for pneumonia detection

------------------
## About the app
> This example features code for online deployment of a binary medical image classification model, based on convolutional neural network architecture. The CNN has two hidden layers and has been trained on the following chest x-ray image dataset for pneumonia curated by Kermany Daniel, Zhang Kang, Goldbaum Michael (2018). Chest X-Ray Images for Classification. The trained model achieved accuracy of more than 86% on the test set and its weights have been saved in the Models folder (see file: trained_model.h5) in the very useful HDF5 format. You may use your own saved trained model! Just make sure you put it in the Models folder and name it appropriately so that the flask app may call it.

> A JavaScript app running on the browser calls the Flask app (app.py) to load the model weights and return results to the JavaScript  app (through the 'GET' and 'POST' methods).
<ul>

<li>As per Heroku requirements for stability and reproducibility, versions of all required python environments were specified in the requirements.txt file</li>
<li>Inclusion of gunicorn to the requirements.txt file</li>
<li>Changed the app.py (flask app) file to adapt it to the required functionality according to the trained binary image classification model. The program was also modified to delete every uploaded image after providing the prediction. This will prevent exceeding capacity limits. The last lines of the file have been modified to work with gunicorn.
<li>The Index.html and base.html files have been modified accordingly to include references and information about the model</li>
<li>


### UI Modification

Modify files in `templates` and `static` directory.

`index.html`, `base.html` for the UI and `main.js` for all the behaviors

### Installation 

Install the requirements in requirements.txt file

### Run

In terminal type  'python app.py' after locating to this directory


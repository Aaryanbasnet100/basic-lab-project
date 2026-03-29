Weather Prediction Group Project (LSTM vs CNN)

We wrote the code to be easy to run. Basically it is a automated pipeline that does everything from data prep to visualization.

What You Need (Libraries)
To get this running, you need a standard Python enviroment.

just pip install these librarys:

Bash
pip install pandas numpy torch matplotlib scikit-learn
(Tip: If you have a GPU, PyTorch will use it. If not, dont worry it run fine on CPU, just a bit slower.)

Setting Up The Folder

This is the most important part. For the script to work without errors, the folder need to look exactly like this:

temp_prediction_LSTM_vs_CNN.py: The python code we provided.

jena_climate_2009_2016.csv: The dataset file. Make sure it is in the same folder as the script, or Python wont find it.
Write that if we use the code in colab then upload the jena_csv file in that 

Or if you have both (the python script and the jena_csv file) in the same folder and make sure that your working directory and script are in same folder, in this case you don’t really need to need to provide the full path, just the filename ‘jena_csv…’ is enough

How to Run It
We designed this script so you dont need to run cell-by-cell.

If using Spyder (Recommended):

Open the script(temp_prediction_LSTM_vs_CNN.py) in Spyder.

Check the top-right corner to make sure the Working Directory matches the folder.

Hit the big Run Button (F5).

What happens next? The script will do these steps:

Load and normalize the weather data automaticly.

Train the LSTM model for 30 epochs.

Train the CNN model for 30 epochs.

Auto-Save: It check the error rate and saves the best version of the models as best_LSTM.pt and best_CNN.pt in the folder.

Results: Finally, it will show some graphs of the cnn and lstm losses w.r.t epoch. also, prediciton vs reality.
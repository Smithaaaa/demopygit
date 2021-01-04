# demopygit
This ia a demo

from flask_ngrok import run_with_ngrok
from flask import Flask
##Running the flask app
app = Flask(__name__)
#We need to start ngrok when the app is run
run_with_ngrok(app)
@app.route("/")
def index():
  return "<h1>Trail Of Flask on Google Colab!</h1>"
@app.route("/get_details")
def get_details():
  return "<h1>This is the get details page!</h1>"
@app.route("/test")
def test_page():
  return "<h1>This is Test Page!</h1>"

app.run()      


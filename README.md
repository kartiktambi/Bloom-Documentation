# Bloom Documentation
Bloom is a Back-to-School helping app, which provides access to the Student of features like Recent Notices, Latest Events, a Translator, and much more surprising features!

## Airtable Spreadsheet Usage
The Airtable Spreadsheet is used as the primary Database for the App. Only 1 Spreadsheet is used.
The Spreadsheet consists of the following Tables, with their respective Column headers written under them : 
- Students : This store the data of the Students after their Registration/Sign up.
  * Name - This stores the Student's entered Name. *(Column field type : Single_line_text)*
  * Grade - This stores the Student's selected Grade which he/she studies. *(Column field type : Single_line_text)*
  * Email - This stores the Student's entered Email. *(Column field type : Single_line_text)*
- Teachers : 
  * Name - This stores the Teacher's entered Name. *(Column field type : Single_line_text)*
  * Grade - This stores the Teacher's selected Grade which he/she teaches. *(Column field type : Single_line_text)*
  * Email - This stores the Student's entered Email. *(Column field type : Single_line_text)*

## Web API Usage
There are 2 Web API components used in App. One is used for the special feature in app - the Dictionary. It is powered by The Webster's Learners Dictionary API.
* For the best usage of Dictionary API, please ensure that you apply your Learner's Dictionary; You can apply for API Key here : https://dictionaryapi.com/register/index
(Please make sure you apply for only 1 key - the Learner's Dictionary)
After the Registration, you can find the Learner's API key here - https://dictionaryapi.com/account/my-keys

* The Second API, is used for returning a book's details by inputting the book's ISBN no. The API's documentation can be found here - https://developers.google.com/books/docs/v1/using.
To get best results, please replace my own API Key's with your keys; You can get your own Google Books API Key here : https://console.developers.google.com
After creating a project on Google Developer's Console, Select the Project from the "Spinner" on top left corner of the page. Then on the Dashboard, tap "Enable APIs and Services", then search & select the "Google Books API".
Next, click the "Enable" button. You will be redirected to Dashboard; After this, in the message - "To use this API, you may need credentials." click "Create Credentials" button.
After that, please select the "Google Books API" from the API spinner, then select "Other UI - e.g.: Windows" and then "Public Data".
Now you will get the API key by clicking "What credentials do I need?". Please paste the API key in the "when books_btn clicked" block (there is a comment written on the block for ease.) on the "dict and books" screen in the project.

# Bloom Documentation
Bloom is a Back-to-School helping app, which provides access to the Student of features like Recent Notices, Latest Events, a Translator, and much more surprising features!

## All features
* Recent Notices - the student has the ability to view the notices published by his/her teacher.
* Moments - A photo wall for the whole school, where any "Teacher" can post his/her class activities/events photos to whole school.
* Projects - The student also has the ability to browse the assigned projects to the class & can also take a look at wha projects are other classes getting.
* Notes - The student can also take his important notes on the go; with the abiliy of deleting/viewing them later.
* ToDo(s) - The student can also organize his work with the ToDo(s) feature, similar to the Notes, he can also view/delete them later.
* Dictionary - This feature allows the student to access the Learner's Dictionary, (powered by the Webster's Dictionary) where he/she gets the word type, defination, plural of the given word.
* Translator - The student can also Translate English to any supported language he/she wishes.
* My Feed - The student can also get his feed, which consits of top articlesfor students, suggested books to read, helpful sites, and more.
* Search a book's details - This is a very advanced and useful feature for a student. He/She can the book's main & important deails of the book he/she is holding by jus entering the "ISBN" number of the book (which is found at the back side of the book).

## Types of Users
* Students - These have access to *view* everything - dictionary, translator, read notices, projects, etc. (They cannot add/edit anything like notices, projects & moments)
* Teachers - They are the content providers; i.e., they only can give Notices, Projects, & Moments.

## Airtable Spreadsheet Usage
The Airtable Spreadsheet is used as the primary Database for the App. Only 1 Spreadsheet is used.
The Spreadsheet consists of the following Tables, with their respective Column headers written under them : 
- Students : This store the data of the Students after their Registration/Sign up.
  * Name - This stores the Student's entered Name. *(Column field type : Single_line_text)*
  * Grade - This stores the Student's selected Grade which he/she studies. *(Column field type : Single_line_text)*
  
- Teachers : 
  * Name - This stores the Teacher's entered Name. *(Column field type : Single_line_text)*
  * Teaching Grade - This stores the Teacher's selected Grade which he/she teaches. *(Column field type : Single_line_text)*
  
- Notices : 
  * Notice - This stores the Notice Body given by the teacher. *(Column field type : Single_line_text)*
  * Date - This stores the date of when the notice was published. *(Column field type : Single_line_text)*
  
- Notices : 
  * Description - This stores the Project Description given by the teacher. *(Column field type : Single_line_text)*
  * Due Date - This stores the submission date of the project. *(Column field type : Single_line_text)*
  * Class - This stores the projects's grade (what grade students are applicable for this project). *(Column field type : Single_line_text)*
  
- Moments : 
  * Pic - This stores the Cloudinary URL of the image picked by the teacher. *(Column field type : Single_line_text)*
  * Caption - This stores the caption for the moment (the image). *(Column field type : Single_line_text)*

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
Now you will get the API key by clicking "What credentials do I need?". Please paste the API key in the "when books_btn clicked" block (there is a comment written on the block for ease) on the "dict and books" screen in the project.
## Other Keys
* For the Yandex Translator, I have applied my own key; to make sure app runs perfectly, please apply your key.
* For Cloudinary DB, I have applied my own cloud credentials; to make sure photos upload perfectly, please apply your credentials.

## Designing
The app's design was made with the help of https://www.material.io website. Almost whole of the app uses *card type* designs, according to Google's Material Designing Principles.

## Color Pallete
* #00B8FF - The app's primary color.
* #4A4A4A - Text colors for the app.
* #E67373 - Notices' screen theme color.
* #1B97F3- Projects' screen theme color.
* #40024E - Moments' screen theme color.

## Credits
* Icons from - Flaticon. Thanks to https://www.flaticon.com for amazing icons!
* Design ideas from - MaterialX app on playStore. This app is very useful for designing ideas, with example templates provided.
* Thunkable X Platform, the back-bone of the app. If this was not there, this great design, such features and the whole app was not possible. Huge thanks to Thunkable X.

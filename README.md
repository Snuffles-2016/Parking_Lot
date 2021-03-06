# Snuffles Parking Lot


## Description

The information in this markdown is intended to expand on your questions we were not able to cover during lecture periods. It will also include best practices on how to approach programming. 

---

## Lecture Parking Lot

#### What the hell do the `dunders` mean

* `_name` vs `__name` vs `__name__`
* `_name` - If you see this, it means you shouldn't have access to this method. 
	* Similar to how programmers use `private methods` inside Ruby. 
* `__name` - This is used to indicate that this method should NOT be overridden by a subclass. 
* `__name__` - This is to tell you that these methods are being used by Python so don't create any with these names
* If you would like further examples of these three check out [this link](http://igorsobreira.com/2010/09/16/difference-between-one-underline-and-two-underlines-in-python.html)

#### Default Instance Variables in Classes

* When we instantiate a class we are creating a instance of that class
* Every instance can be unique with it's own unique variables. These are set using the `self` keyword
* You may recognize the example below

```
class Vehicle:
	def __init__(self, make, model, year):
		self.make = make
		self.model = model
		self.year = year

my_car = Vehicle("Bugatti", "Veyron", 2015)

my_car.make == "Bugatti"
my_car.year == 2015
```
* Now what happens if we want to set a `default value` to an instance variable
* We will assign it the default value inside the parenthesis where we declare our parameters

```
class Vehicle:
	def __init__(self, make, model, year = 2012):
		self.make = make
		self.model = model
		self.year = year

my_car = Vehicle("Bugatti", "Veyron")
my_car.year == 2012

your_car = Vehicle("Mazda", "Protege", 1990)
your_car.year = 1990
```
* Now every instance of that class will have a year set to `2012` UNLESS we decide to pass in an argument for `year`

---

## Jason's Best Practices

***`Know your computer` - Learning to program takes a lot of time. Knowing how to navigate your computer quickly will help you to write code, test code, and overall learn faster. Below are some best practices that you should be implementing into your programming learning***

* `Keep a Clean Workspace` - Yes your desk should be clean but also your **`DESKTOP`**. Keep the amount of browser tabs, Sublime Windows, terminal tabs to a MINIMUM. This will:
	* Save you time from looking at windows you don't need
	* Prevent you from making errors such as changing the wrong file and wondering why it's not working
	* MOST OF ALL - helps you focus on the task at hand
* `Version Control` - Always push working code to github. Do not wait until you have "completed" the exercise. Version Control is meant to SAVE your progress. You wouldn't write a novel on microsoft word and only save it when the novel is done. 
* `Pseudo Code` - Think about your application before you start to code anything. Pseudo code what your objects will look like. Also make sure to write as many user stories as possible, and build out a detailed ERD if you are utilizing a database
* `DO NOT copy old code from a previous assignment.` If you want to use an old assignment for reference that's fine, but type out EVERYTHING. Repeat, Practice, Memorize.
* `DO NOT use code you don't understand.` If you decide to copy something you found through your research such as Stack Overflow answers, make sure you understand every letter of that code before using it. 
* `Doc Strings` - Use doc strings to comment out your code. They can also be viewed in the terminal when you `dir()` and `help()` your file. Doc strings can also be used to type out formatted print statements so there's no need to use string commands such as `\n`
* `Debugging with Print()` - Print out all the values you are passing between classes and methods. You want to make sure those values are being passed how you expect it to be passed. 
	* This works along side commenting out your code. You should be commenting every code block so other users and future you will know what the hell was going on
* `Saving and Testing ALL Changes` - This goes along the same lines as Pushing all working versions to Github. If your code works and you add changes TEST AGAIN. Testing and pushing to github should be second nature and should occur dozens of times a day
* `Review` - Use the lesson plans for reference, they were made so you could look back to it for guidance on what you learned today
* `DOING > READING` - Stop looking for things to read and work on your code. Doing something is always better than just reading blogs

---

## Keyboard Shortcuts

##### Macbooks

* `cmd+s` - Save
* `cmd+c` - Copy
* `cmd+x` - Cut
* `cmd+v` - Paste
* `cmd+tab` - change between programs. Hold down command and tap tab to filter through programs
* `cmd+(tilda button)` - change between windows of the same program. Hold down command and press the tilda button to filter through the windows
* `cmd+w` - Quit a tab
* `cmd+q` - Force quit a program

##### Sublime

* `cmd+d` - Target the next showing of whatever word your cursor is already on
* `cmd+option+(press a number)` - This will quickly break up your screen into columns equal to the number you pressed
* `cmd+(press a number)` - Target a specific tab based on a number
* `tab` - tab your line to the right. Default in sublime is 4 spaces, you can customize your tab size to be 2 spaces or anything you like
* `shift+tab` - tab your line to the left. (reverse tab)

---

## Tools and Resources

* Download Sizeup for your Macbook so you can snap your screens into place

##### Sublime Text Packages

* `Emmet`
* `Color Picker`
* `Bracket Highlighter`

##### CSS Resources

* [http://caniuse.com/](http://caniuse.com/)
* [https://coolors.co/](https://coolors.co/)
* [http://css3buttongenerator.com/](http://css3buttongenerator.com/)

##### JS Resources

* [http://javascriptissexy.com/](http://javascriptissexy.com/)
	* Read about:
	* Callbacks, Closures, Higher Order Functions
	* JS This
	* JS Bind Call Apply

##### APIs

* Free Public APIS - [https://github.com/toddmotto/public-apis](https://github.com/toddmotto/public-apis)

##### Django 

* Common URL Patterns - [https://github.com/codingforentrepreneurs/Guides/blob/master/all/common_url_regex.md](https://github.com/codingforentrepreneurs/Guides/blob/master/all/common_url_regex.md)


## Lunch Spots

* Chipotle - 
	* Madison Ave, btw 40th and 39th str
* Dig Inn - 
	* Madison Ave, btw 40th and 39th str
* Pret A Manger - Ready to go salads and wraps
	* Madison Ave, 39th str
* Cafe Zaiya - Japanese Cafe
	* 41st street between Madison and 5th
* Sunrise Mart - Japanese Cafe and Grocery Store
	* 41st street between Madison and 5th
* Mcdonalds - Doo Doo
	* Madison and 40th street
* Num Pang - Viet Sandwiches
	* 41st street between Lexington and 3rd
* Choza - Taqueria
	* 41st street between Park and Madison (Next Door)
* Shake Shack - American
	* 40th street and 3rd avenue
* Norikoh - Japanese
	* 39th street, between Madison and 5th ave
* Nirvana - Indian Buffet
	* Lexington between 40th and 39th street
* Hunan Manor - Chinese
	* Lexington between 40th and 39th street
* Rhong-Tiam - Thai
	* 39th street and Lexington
* Essen - American 
	* Madison Avenue between 41st and 40th
	
---

## Calendar

| Weeks | Day 1                                            | Day 2                                                          | Day 3                                                   | Day 4                                               | Day 5                                          | Weekend  Assignments                                                 |
|-------|--------------------------------------------------|----------------------------------------------------------------|---------------------------------------------------------|-----------------------------------------------------|------------------------------------------------|----------------------------------------------------------------------|
| 1     | Python Fundamentals One                          | Python Fundamentals Two                                        | Intro to Object Oriented Programming                    | OOPs Part  Two                                      | Review                                         | RPG Version One                                                      |
| 2     | Big O Linked List Stacks Queues                  | Binary Search Linear Search Insert Sort Bubble Sort            | MVC Intro Views Controller SQL Intro                    | Full MVC Sqlite3 CreateDB SeedDB                    | Review No Class                                | RPG  Version Two                                                     |
| 3     | RPG Review                                       | Foreign Keys Relational Databases                              | Relational Databases Part Two SQL JOINS Bank Software   | API Intro OMDB Movie Search                         | API Part Two Markit API Terminal Trader        | Terminal Trader Trader to Bank                                       |
| 4     | Advanced Python Args + Kwargs List Comprehension | Review                                                         | Review                                                  | Review                                              | Phase 1 Assessment                             | Intro HTML  CSS JavaScript                                           |
| 5     | Star Wars Vanilla  DOM                           | Star Wars jQuery DOM Image Slider                              | CSS Positions JS This Tic Tac Toe                       | CSS Grids CSS Animations Weekend HW                 | CSS Grids CSS Animations Weekend HW            | Black Jack Connect Four Tic Tac Toe Battle Foundation Star Wars Blog |
| 6     | JS AJAX OMDB API Node Whiskey API                | Django Intro / Set up Virtual Env Forms and Request Simple ORM | Django CRUD Multiple Tables                             | Django Forms Class Based Views Forms Request Object | Template  Inheritance Static Files Model Forms | UserLESS  Blog                                                       |
| 7     | Django User Class User Sessions UserFUL blog     | UserFul Blog Day 2                                             | Custom Validation Form Validation Building Your Own API | Building an API Day 2                               | Building Front End  To Consume Real Estate API | Real Estate  Projects                                                |
| 8     | Real Estate Projects                             | AJAX with Django Mustache Templating                           | Hacker News Review                                      | Review                                              | Assessment                                     |                                                                      |
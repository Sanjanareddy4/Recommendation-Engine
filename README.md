==>  Files in the repo
foodiereco zip file contains all the code in flutter can be directly uploaded in online IDE to run.

.csv files are the files from the database which are always remains same unless the food items changed.
# ______  FOODIE APP  ______

=>Food recommendation system.
=>Recommends food based the food items clicked on the application.
=>Basically these recommendations can be used in food delivery apps based on the previously ordered food items.
=>Only the database provided by the back4app is used all the code is written in the flutter in various dart files.


# ______ HOW TO RUN A FLUTTER APPLICATION ______

Download the zip file available with the name foodiereco. Which is a zip file contains flutter source code
required for project.

#### FLUTTER ONLINE IDE ####

To open an existing Flutter project:
1. On the website "https://flutlab.io/profile" click on the upload flutter project zip.
2.Browse to the directory holding your existing Flutter source code files.
3.Click Open.


#### TO RUN FLUTTER FROM VS CODE ####

To install updates manually:
1.Click the Extensions button in the Side Bar.
2.If the Flutter extension is shown with an available update, click the update button and then the reload button.
3.Restart VS Code.

To open an existing Flutter project:
1.Click File -> Open from the main IDE window.
2.Browse to the directory holding your existing Flutter source code files.
3.Click Open.

==> wait for 5 sec to get updated recommendations. If recommendations are ont updating please click for second time and check.

# ______ ABOUT PROJECT ______


1.This project is a mobile application which recommends food items based on food items clicked before.
2.The upper part of this application consists of list of food items available. On clicking those cards it is 
  assumed that the food item is liked or one wants to order that food item (similar to swiggy an other apps).
3.Based on this the recommendations will be provided for the user in the second half of the application.
4.It is assumed that only one user uses this particular app and no sign is provided.
5.There is also a refresh button available on the top right corner of the app on clicking that old recommendations
  will get erased an new ones will appear based on selected items after refresh.
6.The algorithm use for recommendations is based on cosine distances. These distances are calculated based on
  whether the item is veg, fry, has masala and level of spice it contains.
7.Nearest neighbours of the selected items are displayed.
8.Note that recommendations are purely based on the properties provided for the items in the database but not on the 
  users mood or rating provided.


# ______ TIME COMPLEXITY ______

1. Let 'p' be the number of selected items from the list.
2. Let 'k' be the minimum number of recommendations expected to be there always.
3. Let 'n' be the total number of items in the list i.e. in the menu.

==> The time complexity of the algorithm I used is O( nk + p ).


# ______ SPACE COMPLEXITY ______

1. With n, p, k having same meanings as before:
==> Space used O(n + p) in the database of back4app.
2. Space used in the dart files in the form of lists and variables is O(n+p+k).


# _______ ADD FOODITEMS TO THE MENU ______

1. Firstly the item name and types are to be added in the data base.
   Can be done from the dart file with ..set.
2. Add the same in the items array in main.dart file 
3. And lastly image of the should be added in the images folder with appropriate naming
   i.e. img_(item number)
4. That's all the item will get added to the menu.

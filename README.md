# Configuring Product Flavors 
A few weeks back I started experimenting and tried to configure product flavors in my app.
So basically I wanted an activity to behave and change the ui depending on the api level the user has.
So i made product flavors minApi21 and minApi16 and added the activity class and its respective layout file in proper packages, below is the
file structure.

### File structure for Java classes
<pre> 
 ┬  
 ├ src
    ├ main   
    |  └ java
    |     └ com.example.sunnyjain.productflavortest
    |                                         └ MainActivity.java
    ├ minApi16  
    |  └ java
    |     └ com.example.sunnyjain.productflavortest
    |                                         └ DisplayActivity.java
    ├ minApi21  
       └ java
          └ com.example.sunnyjain.productflavortest
                                              └ DisplayActivity.java  
  
  </pre>
  
  ### File structure for res files
  <pre>
 ┬  
 ├ src
    ├ main   
    |  └ res
    |     └ layout
    |         └ activity_main.java
    ├ minApi16  
    |  └ res
    |     └ layout
    |         └ activity_display.java
    ├ minApi21  
       └ res
          └ layout
              └ DisplayActivity.java 
</pre>

Now, the DisplayActivity.class is imported in MainActivity.
Make a change in the DisplayActivity.java file. any change would do even a comment.
try and run the app. it will crash. dont do anything and re-run the app it will work fine.
so everytime we make a change in any of the displayactivtiy files, it will crash the first time and on re-running will work fine.

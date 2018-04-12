# Display subcategory titles in category blogs (Joomla 3)  
On Joomla 3,this simple override adds the subcategory title above the relevant articles in category blogs. The result looks like this:

````
Subcat title A
Article 1
Article 2
Article 3
…

Subcat title B
Article 1
Article 2
Article 3
…

Subcat title C
Article 1
Article 2
Article 3
…
````

For an example see [http://svictor.net/anthropology/publications] (Books, Edited volumes, Articles etc. are all subcategories of Publications). Stock Joomla can sort the articles by subcategory, but doesn’t output the subcategory title above the relevant set of articles. 

# Usage
Place the file in `/templates/your-template/html/com_content/category/`

The override is only applied on pages with the "subcats" page class. To set the page class to "subcats" head to the options of the relevant menu item. 
There is a short snippet at the begining of the file to check whether the override is active or not (commented out by default). 

The article set of each subcategory is wrapped in a `div` of class "accordion". As the name suggests, this can be used in conjunction with an accordion effect plugin.

# Limitations
The templates on which I tested this are very close to stock Joomla. Most of them are just html and css on top of the core files. I don’t use any additional framework. My override may not work if you use more sophisticated template systems, especially if they already have their own overrides for blog.php.

It is a very simple override. My additions to the stock file are indicated by comments starting with "V.".

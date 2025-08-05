# Web-Development-day-68
JavaScript DOM method
getElementbyId
The getElementById() method is a part of the JavaScript document object and it allows developers to access a specific element on a web page by its unique ID. This method returns the first element that matches the specified ID, or null if no such element is found.

For example, consider the following HTML code:

<div id="myDiv">This is my div</div>

The following JavaScript code can be used to access the element with the ID "myDiv" and change its text:

let myDiv = document.getElementById("myDiv");
myDiv.innerHTML = "This is my new text";

The getElementById() method is a convenient way to access a specific element on a web page, as it saves developers from having to traverse the entire DOM tree to find the element. This method is especially useful when working with large and complex web pages, as it allows developers to quickly and easily access the elements they need.

It's important to note that the ID of an element must be unique within the web page, as the getElementById() method only returns the first element that matches the specified ID. Also, the getElementById() method is case-sensitive, meaning that "myDiv" and "mydiv" are considered to be different IDs.

In conclusion, the getElementById() method is a powerful tool for accessing specific elements on a web page by their unique ID. Understanding how to use this method is essential for creating dynamic and interactive web pages, as it allows developers to quickly and easily access the elements they need. However, it's important to keep in mind that the ID of an element must be unique within the web page and the method is case-sensitive.

getElementsByClassName
The getElementsByClassName() method is a part of the JavaScript document object and it allows developers to access multiple elements on a web page by their class name. This method returns a live HTMLCollection of elements with the given class name, or an empty HTMLCollection if no such elements are found.

For example, consider the following HTML code:

<div class="myClass">This is my div</div>
<div class="myClass">This is my div</div>
<div class="myClass">This is my div</div>

The following JavaScript code can be used to access the elements with the class name "myClass" and change their text:

let elements = document.getElementsByClassName("myClass");
for (let i = 0; i < elements.length; i++) {
    elements[i].innerHTML = "This is my new text";
}

The getElementsByClassName() method is a convenient way to access multiple elements on a web page, as it allows developers to select elements based on their class name rather than their unique ID. This method is especially useful when working with large and complex web pages, as it allows developers to quickly and easily access multiple elements that share the same class name.

It's important to note that the getElementsByClassName() method returns a live HTMLCollection, which means that the collection is updated automatically as elements are added or removed from the web page. Also, this method is case-sensitive, meaning that "myClass" and "myclass" are considered to be different class names.

In conclusion, the getElementsByClassName() method is a powerful tool for accessing multiple elements on a web page by their class name. Understanding how to use this method is essential for creating dynamic and interactive web pages, as it allows developers to quickly and easily access multiple elements that share the same class name. However, it's important to keep in mind that the method returns a live HTMLCollection and is case-sensitive.


getElementsByName
The getElementsByName() method is a part of the JavaScript document object and it allows developers to access multiple elements on a web page by their name attribute. This method returns a live HTMLCollection of elements with the given name attribute, or an empty HTMLCollection if no such elements are found.

For example, consider the following HTML code:

<input type="text" name="myName" value="">
<input type="text" name="myName" value="">
<input type="text" name="myName" value="">

The following JavaScript code can be used to access the elements with the name attribute "myName" and change their value:

let elements = document.getElementsByName("myName");
for (let i = 0; i < elements.length; i++) {
    elements[i].value = "This is my new value";
}

The getElementsByName() method is a convenient way to access multiple elements on a web page, as it allows developers to select elements based on their name attribute, which is a common way to group elements with similar functionality. For example, radio buttons or checkboxes that are related to a certain topic should have the same name attribute. This method is especially useful when working with large and complex web pages, as it allows developers to quickly and easily access multiple elements that share the same name attribute.

It's important to note that the getElementsByName() method returns a live HTMLCollection, which means that the collection is updated automatically as elements are added or removed from the web page. Also, this method is case-sensitive, meaning that "myName" and "myname" are considered to be different name attributes.

In conclusion, the getElementsByName() method is a powerful tool for accessing multiple elements on a web page by their name attribute. Understanding how to use this method is essential for creating dynamic and interactive web pages, as it allows developers to quickly and easily access multiple elements that share the same name attribute. However, it's important to keep in mind that the method returns a live HTMLCollection and is case-sensitive. Additionally, this method is mostly used for form elements like radio buttons, checkboxes, and input fields.


getElementsByTagName
The getElementsByTagName() method is a part of the JavaScript document object and it allows developers to access multiple elements on a web page by their HTML tag name. This method returns a live HTMLCollection of elements with the given tag name, or an empty HTMLCollection if no such elements are found.

For example, consider the following HTML code:

<p>This is my paragraph</p>
<p>This is my paragraph</p>
<p>This is my paragraph</p>

The following JavaScript code can be used to access the <p> elements on the web page and change their text:

let elements = document.getElementsByTagName("p");
for (let i = 0; i < elements.length; i++) {
    elements[i].innerHTML = "This is my new text";
}

The getElementsByTagName() method is a convenient way to access multiple elements on a web page, as it allows developers to select elements based on their HTML tag name. This method is especially useful when working with large and complex web pages, as it allows developers to quickly and easily access multiple elements of the same type.

It's important to note that the getElementsByTagName() method returns a live HTMLCollection, which means that the collection is updated automatically as elements are added or removed from the web page. Also, this method is case-sensitive, meaning that "p" and "P" are considered to be different tag names.

In conclusion, the getElementsByTagName() method is a powerful tool for accessing multiple elements on a web page by their HTML tag name. Understanding how to use this method is essential for creating dynamic and interactive web pages, as it allows developers to quickly and easily access multiple elements of the same type. However, it's important to keep in mind that the method returns a live HTMLCollection and is case-sensitive. It's a good practice to use this method in combination with other methods like getElementById and getElementsByClassName to target specific elements on the web page.

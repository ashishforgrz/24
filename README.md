# 24/05/2022
=> Class - 

Class is a blueprint that defines a nature of a future object

We can add methods inside class 

eg:

class ashish{
    constructor(name,age,town,company){
        this.name=name;
        this.age=age;
        this.town=town;
       this.company=company;
    }
afterFive(){
    return this.age + 5;
}
}
let person=new ashish("Ashish",22,"Panchkula","Grazitti")
console.log(person.afterFive())



=> Prototype -
Add properties to the object
eg:
Person.prototype.gender = 'male';
Person.prototype.age=22;


=> Inheritance - 
Inheritance enables you to define a class that takes all the functionality from a parent class and allows you to add more.
Syntax - class newClass extends oldClass

=> Getter and Setter -
Getter -
This example uses a 'lang' property to get the value of the 'language' property
const person = {
  firstName: "Ashish",
  lastName: "Sharma",
  language: "Hindi",
  get lang() {
    return this.language;
  }
};
document.getElementById("demo").innerHTML = person.lang;

Setter -
This example uses a 'lang' property to set the value of the 'language' property.
 const person = {
  firstName: "Ashish",
  lastName: "Sharma",
  language: "",
  set lang(lang) {
    this.language = lang;
  }
};
person.lang = "Hindi";
document.getElementById("demo").innerHTML = person.language;


=> Set -
Collection of values that are unique
1. new Set() - Creates a new set
   eg: const newSet = new Set([21, 34, 35, 56, 23]);
                      
2. .add()  - Add new element at the end
   eg: cont newSet();
       newSet.add("Hello")
       newSet.add("World")
       
3. .clear() -Removes all elements and returns undefined
    
4. .delete() - deletes particular
5. .has() - check if the element exists
6. .forEach() - method invokes a function for each Set element
   eg: const letters = new Set(["a","b","c"]);
       let text = "";
       letters.forEach (function(value) {
       text += value;
       })  

=> Map -  creates a new array from calling a function for every array element

Map Property -
Map.prototype.size – It returns the number of elements or the key-value pairs in the map

Map Methods -
1. Map.prototype.set() –  adds the key and value to the Map Object
  Syntax - map1.set(k, v);
2. Map.prototype.has() –  return a boolean value depending on whether the specified key is present or not
  Syntax - map1.has(k);
3. Map.prototype.get() – returns the value of the corresponding key 
  Syntax - map1.get(k); 
4. Map.prototype.clear() – Removes all the elements from the Map object
  Syntax - map1.clear();
5. Map.prototype.forEach() – executes the callback function once for each key/value pair in the Map
  Syntax - map1.forEach(callback[, thisArgument]);


Error Handling -
--try and catch statement -
try statement allows you to define a block of code to be tested for errors while it is being executed
catch statement allows you to define a block of code to be executed, if an error occurs in the try block
Syntax - 
try {
  Block of code to try
}
catch(err) {
  Block of code to handle errors
}

--throw statement -
throw statement allows you to create a custom error.

Error Name Values - 

RangeError   -   out of range number has occurred
ReferenceError  -   if we use a variable that has not been declared
SyntaxError    -	A syntax error has occurred
TypeError	 -   thrown if you use a value that is outside the range of expected types

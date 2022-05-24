# 24/05/2022
Class - 
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



Prototype -
Add properties to the object
eg:
Person.prototype.gender = 'male';
Person.prototype.age=22;


Inheritance - 
Inheritance enables you to define a class that takes all the functionality from a parent class and allows you to add more.
Syntax - class newClass extends oldClass

Getter and Setter -

1. Getter -
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

2. Setter -
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
 

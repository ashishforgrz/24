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

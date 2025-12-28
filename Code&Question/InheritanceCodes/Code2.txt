class Parent{
      constructor(){
            console.log("Parent constructor called");
      }
//add the method later on
      pMethod(){
          console.log("Parent Method");    
      }
 
}
class Child1 extends Parent{
     
}
const obj = new Child1();
obj.pMethod();

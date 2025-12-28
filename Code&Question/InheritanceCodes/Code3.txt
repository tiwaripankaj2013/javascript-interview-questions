class Parent{
      constructor(a){
            console.log("Parent constructor called",a);
      }
      pMethod(){
          console.log("Parent Method");    
      }
 
}
class Child1 extends Parent{
     constructor(){
        console.log("Child...");
     }
}
const obj = new Child1(4);
obj.pMethod();
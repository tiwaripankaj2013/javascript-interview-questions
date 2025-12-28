const sum=function(a){
    return function(b){
         return a+b;
    }
}
const ans=sum(5)(6);
console.log(ans);
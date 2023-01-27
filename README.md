# React-Test01

//Write a JS program that finds the longest common substring between two strings.

function LCSubStr(s,t,n,m){
var dp=Array(2).fill().map(()=>Array(m+1).fill(0));
var res = 0;
for (var i=1; i<=n; i++)
{
for (var j=1; j<+m; j++)
{
if(s.charAt(i-1)==t.charAt(i-1){
dp[i%2][j]=dp[(i-1)%2][j-1]+1
if(dp[i%2][j]>res)
res = dp[i%2][j]>res)
res=dp [i%2][j];
}
else dp [i%2][j];
}
}
return res;
}
var X="Hello World";
var Y="Hello Code";
var m =X.length;
var n= Y.length;
console.log(LCSubStr(X,Y,m,n))

# React-Test02
//Implement a JS function that takes a list of integers and a target number as input, and returns a array of two integers that add up to the target number.

function findWays(arr,i,k){
if (k==0 && i== arr.length){
return 1;
}
if (i>= arr.length){
return 0;
}
return findWays(arr,i+1,k)+findWays(arr,i+1, k-arr[i]+findWays(arr[i]);
}
let arr = [-3,1,3,5,7];
let k = 5;
console.log(findWays(arr,0,k));

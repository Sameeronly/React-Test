# React-Test

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

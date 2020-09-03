Write a function that when given a URL as a string, parses out just the domain name and returns it as a string. For example:

`domainName("http://github.com/carbonfive/raygun")` == "github" 
`domainName("http://www.zombie-bites.com")` == "zombie-bites"
`domainName("https://www.cnet.com")` == "cnet"

```
function domainName(url){
  let first = url.replace(/https?:\/\//, "")
  let second = first.replace(/www./,"")
  return second.split('.').slice(0,1).join('')
}
```
`domainName("http://github.com/carbonfive/raygun")` 
domainName("http://www.zombie-bites.com")
domainName("https://www.cnet.com")
domainName("www.xakep.ru")

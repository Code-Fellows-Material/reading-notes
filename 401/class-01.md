# 401 - Class 01 Reading Notes

---

1. Describe (in plain English) what Array.map() does:

> Array.map() is a method built into the Array object in Javascript. It iterates over a given array one index at a time and passes the value at that index to a callback function.
The callback function acts on that value in whatever way we define. Then places that returned value into a new array at the same index as the first array.




1. Describe (in plain English) what Array.reduce() does:

> Array.reduce() is a method built into the Array object in Javascript. Array.reduce() acts on a given array via a callback function we define. In it's most basic form, the callback function takes a 'previous value' and a 'current value' as arguments. If not defined otherwise, on the first iteration, the 'previous value' and the 'current value' will be set to the first two indices of the array. The callback function will then be run, and the value returned from that function will be set as the 'previous value' for the next iteration. The next index in the array will then be passed in as the 'current value', and the callback function will be ran again.The cycle will continue until array.reduce() hits the end of the array, at which point it will return the 'previous value' as the final return value.



1. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:

 - With normal Promise .then() syntax:

  
        function getCharacters(){
          superagent.get('https://swapi.dev/api/people/1')
          .end((err, obj) => {  
            console.log(obj.body)
          })
        }

  -  Again with async / await syntax:

 
          async function cityGetter(city){
            try {
              const res = await superagent.get(`https://geocode.xyz/${city}?json=1`)
              console.log(res.body)
            } 
            catch(err) {
              console.log(err)
            }
          }

2. Explain promises as though you were mentoring a Code 301 level student:

> Javascript is what you would call a "single threaded language". What that means is that at any give time, only one piece of your program can be running. As you get into things like API calls, you're going to start seeing that we need our code to be able to continue running while we do certain things- like reaching out to other computers or servers for information. Reaching out like this and waiting for a reply can take some time and can therefore cause our code to execute out of order, or it can completely halt our program while we wait. Promises allow us to get around these issues by allowing some code to execute in the proper order only after some give condition is received.

1. Are all callback functions considered to be Asynchronous? Why or Why Not?

> No, 'synchronous' callbacks are used in many higher-order functions and execute as expected in the normal flow of our code. Asynchronous callback functions are used in things like promises to execute some code after our promise is resolved or rejected.
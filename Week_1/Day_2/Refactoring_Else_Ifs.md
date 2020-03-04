  ## Refactoring Else Ifs...
  
  Take a look at this else ifs.

  ```javascript
  if (char === "a") {
    returnChar = "4";
  } else if (char === "e") {
    returnChar = "3";
  } else if (char === "o") {
    returnChar = "0";
  } else if (char === "l") {
    returnChar = "1";
  } else {
    returnChar = "self";
  }
  return returnChar;
  };
  ```

  This is what I actually wrote, and as soon as I realized my source was approaching to 50++ lines,
  I decided to tidy things up and decided to use an object so it getes more readable.

  ```javascript 
  let charMap = {
    "a" : 4,
    "e" : 3,
    "o" : 0,
    "l" : 1
  }
  ```
  What I did was to iterate the map
  by accessing the key and values like below and iterate

  ```javascript
  Object.keys()
  Object.values()


  let result = "";

  for (i = 0; i < Objet.keys(charMap).length; i++) {
    if (Object.keys(charMap)[i] === "a"){
      result += 4; 
    }
  }
  ```

  It was getting even worse when I tried to come with nested loops.
  One of LHL mentors taught me a smarter way to handle this,
  without all those re-iterations and getting key:values.

  ```javascript
  return charMap[char] || char;
  ```

  this saved so many lines and is really readable.

  Should really focus on basic properties of data types.


  object[key] = value.
  return what you just received.
  

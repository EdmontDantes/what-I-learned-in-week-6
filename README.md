# what-I-learned-in-week-6

During the week we have strengthen understanding of using various techniques for array modification.  
below is the list of assignment we practiced for using arrays to our advantage in order to achieve various interesting results of solutions to specific problems.

## Array of RadioActive Mutants
during this exercise we mutated directly an array using these methods:  
* _for(let i=0; i<someStr.length;i++)_ - to loop through items and satisfy condition
* _while(satisfyCondtion)_ - to loop through items until condition is satisfied
* _.push()_ - append to an end of an array an item
* _.unshift()_ - append to the beginning of an array an item
* _.pop()_ - remove last item from an array and returns that array with removed items
* _.splice(start, countOfItemsToRemoveFromStart, itemToAdd1, itemToAdd2 ...)_ - using this method we could replace an item via loop with 'odd' or 'even' word stead of numbers and changeNextThreeValues.  
  
## Hip-Hip Array
* _.repeat()_ - can repeat item from an array without a loop
* _.push()_ / _.shift()_ - for removing first and last items from an array
* _.unshift()_ - append to the beginning of an array an item.
* _.splice(start, countOfItemsToRemoveFromStart, itemToAdd1, itemToAdd2...)_ - using splice we can remove items from start of index, count of items to remove and then also add items at the beginning of that start index after the count removed.
* _.slice(start, end)_ - based on zero start index if start is specified removes that item all the way up to end index ei. .slice(1,3) removes from index 1, 2, 3. Returns new array with extracted items.
* _.concat()_ - concatonates two or more arrays together and returns new array with all items from both or more array together.
* _.join('CharacterToJoinWith')_ - using this method we can join items together into one string. Basically we are making a string out of items from an array and if passing a string inside paranthesis we can join items with any character or string between items of an array.

## MapMaker-MapMaker
This exercises taught us how to "map" arrays into a new array without modification of the original array and making a function that can return new array without modifying the original.
example of achieving this as follow:  
```
function doubleAll(numbers) {
    let separateMutatedDoubleNums = [];

    for (i = 0; i < numbers.length; i++) {

        separateMutatedDoubleNums.push(numbers[i] * 2);
    }
    return separateMutatedDoubleNums;
}
```
What we are doing in this function is: 
* create an array separateMutatedDoubleNums
* loop through items and _.push_ double numbers at _i_ index doubled
* return that array.

Most of manual map methods are made like the example above.
## Method-to-My-Madness
Methds to my Madness was the hardest so far exercise that required us to create our own methods of string manupilations without relying on in-built functionality of javascript. below is the list of methods we had to create from scratch:  
* _slice_ - given three parameters of string, start of index to cut string and end index to slice to string. 
* _repeat_ - given a string and repetitions number; return that string repeated that many repetitions given in the parameter.
* _startsWith_ - compare two parameters of two strings and return either true or false if both strings comparatively start with same characters.
* _endsWith_ - compare two parameters of two strings and return true or false if both strings ends With same characters.
* _includes_ - compare arrays items to the second parameter of an item and return true or false if given parameter item is in the arrays items.
* _split_ - given string parameter and separator return new array splitted of a string based on the separator parameter. The way we achieved this is to create an empty array and empty zero number variable looping through the string while comparing each character with separator parameter and then nesting another for loop where index equals previously made empty zero number variable along with making an empty string variable where we would add string index of the second loop and at the end .push empty array with result string of the second loop.
* _trimStart_ - trim spaces from beginning of a given string. We achieve this via creating intermediate empty array then using for loop with indexes and using if conditional statement to check the given string for spaces in the beginning, we return string with previously established and built function _slice_ at the string and index of last ' ' (space) of the for loop.
* _trimEnd_ - same as above only we return _slice_ function with a bit different paramaters meanwhile our for loop looks like this:  
  ```
  for (let i = str.length-1(we reverse the order); i >= 0; i--)
  ```
  _slice_ function using str, 0(starts with index Zero) ,  i + 1 (this index of last space plus one to return that index of string character without space).
## No-filter
## 4-of-4-lyfe
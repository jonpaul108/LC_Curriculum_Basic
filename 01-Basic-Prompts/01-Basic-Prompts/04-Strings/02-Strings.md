### !challenge

* type: code-snippet
* id: strings-1
* language: javascript
* title: First And Third

### !question

Given a string `str`, return the first and third character combined into a single string.  
    
Note:
*Do not split or iterate to solve this prompt.*
      
```js
 
    console.log(firstAndThird("angel")) //=> 'ag'
  
``` 

### !end-question

#### !placeholder

```js
function firstAndThird(str) {


}
```

#### !end-placeholder


### !tests

```js
describe('firstAndThird', function() {

    it("should return a string", function() {
      expect(firstAndThird('hello')).to.be.a('string');
      expect(firstAndThird('jumanji')).to.be.a('string');
    })

    it("should return the correct string", function() {
      expect(firstAndThird('hello')).to.deep.eq('hl');
      expect(firstAndThird('jumanji')).to.deep.eq('jm');
      expect(firstAndThird('worth')).to.deep.eq('wr');
      expect(firstAndThird('tell')).to.deep.eq('tl');
      expect(firstAndThird('scary')).to.deep.eq('sa');
    })

    it("should not split the string", function() {
     expect(firstAndThird('hello').toString()).to.not.include('.split');    
    })

    it("should not iterate", function() {
     expect(firstAndThird('hello').toString()).to.not.include('for');   
    })

})
```
### !end-tests

### !end-challenge

### !challenge

* type: code-snippet
* id: strings-2
* language: javascript
* title: Length Of Strings Multiplied

### !question

Given two strings `str1` and `str2`, return their lengths multiplied together.

 

```js

  console.log(lengthOfStringsMultiplied('cat', 'mat')) //=> 9

``` 

### !end-question

#### !placeholder

```js
function lengthOfStringsMultiplied(str1, str2) {


}
```

#### !end-placeholder


### !tests

```js
describe('lengthOfStringsMultiplied', function() {

    it("should return a number", function() {
      expect(firstAndThird('hello', 'hello')).to.be.a('number');
    })

    it("should return the correct number", function() {
      expect(lengthOfStringsMultiplied('hello', 'hello')).to.deep.eq(25);
      expect(lengthOfStringsMultiplied('cash', 'money')).to.deep.eq(20);
      expect(lengthOfStringsMultiplied('a','b')).to.deep.eq(1);
    })

    it("should not split the string", function() {
     expect(lengthOfStringsMultiplied('hello').toString()).to.not.include('.split');    
    })

    it("should not iterate", function() {
     expect(lengthOfStringsMultiplied.toString()).to.not.include('for');   
    })

})
```
### !end-tests

### !end-challenge


### !challenge

* type: code-snippet
* id: strings-3
* language: javascript
* title: Length As Index

### !question

Given two strings `str1` and `str2`, return the character of `str1` that exists at the index matching the length of `str2`.  
  
Note:  
The length of`str1` will always be greater than the length of `str2`

```js

    console.log(engthAsIndex('cyclone', 'chair')) //=> "n"
        
``` 

### !end-question

#### !placeholder

```js
function lengthAsIndex(str1, str2) {


}
```

#### !end-placeholder


### !tests

```js
describe("lengthAsIndex", function () {
  
  it("should return a string", function () {
    expect(lengthAsIndex("hello", "hell")).to.be.a("string");
  });

  it("should return the character of str1 found at the length of str2", function () {
    expect(lengthAsIndex("hello", "hell")).to.deep.eq("o");
    expect(lengthAsIndex("cash", "mo")).to.deep.eq("s");
    expect(lengthAsIndex("ab", "b")).to.deep.eq("b");
  });

  it("should not split the string", function () {
    expect(lengthAsIndex("hello", "h").toString()).to.not.include(".split");
  });

  it("should not iterate", function () {
    expect(lengthAsIndex.toString()).to.not.include("for");
  });
});
```
### !end-tests

### !end-challenge


### !challenge

* type: code-snippet
* id: strings-4
* language: javascript
* title: Sum Index

### !question

Given a string `str`, return the sum of the string's indexes.


```js

  console.log(sumIndex('s')) //=> 0
  
  console.log(sumIndex('str')) //=> 3

  
  console.log(sumIndex('str1')) //=> 6
      
        
``` 

### !end-question

#### !placeholder

```js
function sumIndex(str) {


}
```

#### !end-placeholder


### !tests

```js
describe('sumIndex', function() {

    it("should return a number", function() {
      expect(sumIndex('hello')).to.be.a('number');
    })

    it("should return the correct character", function() {
      expect(sumIndex('hello')).to.deep.eq(10);
      expect(sumIndex('s')).to.deep.eq(0);
      expect(sumIndex('str1')).to.deep.eq(6);
    })

    it("should not split the string", function() {
     expect(lengthAsIndex.toString()).to.not.include('.split');    
    })

})
```
### !end-tests

### !end-challenge

### !challenge

* type: code-snippet
* id: strings-5
* language: javascript
* title: Is Mirror

### !question

Given two strings `str1` and `str2`, return `true` if `str2` when reversed is the same as `str1`. Return `false` if `str2` is not the same as `str1` when reversed. 



```js

  console.log(isMirror('hello', 'olleh')); //=> true

  console.log(isMirror('str', 'tsr')) //=> false

  console.log(isMirror('s', 's')) //=> true  
        
``` 

### !end-question

#### !placeholder

```js
function isMirror(str1, str2) {


}
```

#### !end-placeholder


### !tests

```js
describe('isMirror', function() {

    it("should return a boolean", function() {
      expect(isMirror('hello', 'olleh')).to.be.a('boolean');
    })

    it("should return true if `str2` is a reversed copy of `str1`", function() {
      expect(isMirror('hello', 'olleh')).to.deep.eq(true);
      expect(isMirror('s', 's')).to.deep.eq(true);
      expect(isMirror('str1', 'trs1')).to.deep.eq(false);
    })

    it("should return false if `str2` is not a reversed copy of `str1`", function() {
      expect(isMirror('hello', 'oll')).to.deep.eq(false);
      expect(isMirror('s', 'a')).to.deep.eq(false);
      expect(isMirror('str1', 'trs1')).to.deep.eq(false);
    })

})
```
### !end-tests

### !end-challenge

### !challenge

* type: code-snippet
* id: strings-6
* language: javascript
* title: Hidden Word

### !question

Given a string `str` and an array of index numbers `indexes`, use the index numbers to combine characters in the string into a new word.  

Note: 
The indexes are in order from left to right.

```js



  console.log(hiddenWord( 'lejfmdofne2', [0, 1, 4, 6, 8])) //=> "lemon"

  console.log(hiddenWord( 'inner till gift', [6, 0, 11, 3, 4])) //=> "tiger"

  console.log(hiddenWord('same', [1, 2])) //=> "am"
      
        
``` 

### !end-question

#### !placeholder

```js
function hiddenWord(str, indexes) {


}
```

#### !end-placeholder


### !tests

```js
describe("hiddenWord", function () {
   
   it("should return a string", function () {
     expect(hiddenWord("hello", [0,1])).to.be.a("string");
   });

   it("should return the correct word", function () {
     expect(hiddenWord("lejfmdofne2", [0, 1, 4, 6, 8])).to.deep.eq("lemon");
     expect(hiddenWord("inner till gift", [6, 0, 11, 3, 4])).to.deep.eq("tiger");
     expect(hiddenWord("same", [1, 2])).to.deep.eq("am");
   });

 });
```
### !end-tests

### !end-challenge


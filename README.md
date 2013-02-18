javascript-questions
====================

JavaScript Interview Questions

Q: Add the class of 'threes' to every third row without using a library.

A: 

Solution 1:
  var thirdRows = document.querySelectorAll('tr:nth-of-type(3n)'),
       count,
       i;
  count = thirdRows.length;
  for(i = 0; i < count; i++){
    thirdRows[i].classList.add('threes');
  }
  
Solution 2: 
  /* old school method */
  var rows = document.getElementsByTagName('tr'),
      count,
      i;
  count = rows.length;
  for(i = 0; i < count; i += 3){
     rows[i].setAttribute('class', 'threes');
  }
  
  Bonus points if they say there's no need to add closs odd, just style based on the selector
  tr:nth-of-type(3n) 
  
   

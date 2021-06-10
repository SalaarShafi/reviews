Check it out here: https://reviews-salaarshafi.netlify.app/

This project displays some reviews which you can sift through or read randomly by clicking on the surprise me button. The react icons library was installed and used to display icons shown in the project.

The data for the displayed reviews is imported from a file to pass in data for every single review in order to display it on the webpage. A useState has been set which provides a numeric value state and an index state that can be manipulated by functions to increase or decrease it's value which inturn is used to obtain previous or next data object to be passed into another function from another file which returns a component having integrated these data values into html tags.

The button icons in the main components are acquired from react icons library installed and on click these run functions which increment or decrement the index state which inturn can be used to access the next or previous review data object of array that is imported as data.The increase and decrease buttons increment the current index state or decrement it and a constant automatically stores the next or previous data object in the array corresponding to the new index state. Conditional statements are used to loop through data and not cause an error when exceeding or receeding the indexes of data array when functions changing the index state are run. The constant is destructured and used in a function which returns the desired component displaying the review on the webpage.

The surprise me button just uses the Math.random and Math.floor functions to get a random number less than or equal to the length of the array and sets the index state to this random number which displays a random review. To avoid recurringly getting the same review every time this function checks whether the new value is same as the previous one, if so it gets another number otherwise returns the result.



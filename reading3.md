# Lists and Keys

source: https://reactjs.org/docs/lists-and-keys.html

#### What does .map() return?

It returns an array with a different set of values depending on what you do to it.

#### If I want to loop through an array and display each value in JSX, how do I do that in React?

You can build collections of elements and include them in JSX using curly braces {}.

#### Each list item needs a unique?

list items need a unique key.

#### What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed.

# The Spread Operator

source: https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

#### What is the spread operator?

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

#### List 4 things that the spread operator can do.

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array

#### Give an example of using the spread operator to combine two arrays.

//Concatenating arrays

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

#### Give an example of using the spread operator to add a new item to an array.

//Adding an item to a list

const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

#### Give an example of using the spread operator to combine two objects into one.

//Combining objects

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

#### In the video, what is the first step that the developer does to pass functions between components?

in the video, the first step the developer does is create a function to pass.

#### In your own words, what does the increment function do?

The function keeps track of the clicks + 1 every time its clicked.


#### How can you pass a method from a parent component into a child component?

You have to create a reference to it.



#### How does the child component invoke a method that was passed to it from a parent component?

In the function that is being used.

# List and Keys
Map is another way of iterating in the array and it will always return you a new array of the same length as the original array comprised of your return values.

Well to display the JSX You can build collections of elements and include them in JSX using curly braces {}.
Each list item needs a unique key prop

Keys are very important they help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity. And  The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys

# Spread Operator:

## What is the spread operator?
It is a quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

## List 4 things that the spread operator can do.
1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Adding an item to a list

## Give an example of using the spread operator to combine two arrays.
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩


## Give an example of using the spread operator to add a new item to an array.
const fruitStand = ['🍏','🍊','🍌']
const sellFruit = (f1, f2, f3) => { console.log(`Fruits for sale: ${f1}, ${f2}, ${f3}`) }
sellFruit(...fruitStand) // Fruits for sale: 🍏, 🍊, 🍌
fruitStand.pop()
fruitStand.pop()
fruitStand.push('🍉')
fruitStand.push('🍍')
sellFruit(...fruitStand) // Fruits for sale: 🍏, 🍉, 🍍
fruitStand.pop()
fruitStand.pop()
sellFruit(...fruitStand,'🍋') // Fruits for sale: 🍏, 🍋, undefined

## Give an example of using the spread operator to combine two objects into one.
[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }





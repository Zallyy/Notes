# Spread ...
---

*All examples with arrays can be utilized with objects*

##### Note to self: 
* Spread shakes out an array element by element
* Rest takes in an array and compresses it 

#### Copying an array
>`
>let copy = [...Array]
`

---

#### Combining two arrays 
```
const arr = [1, 2, 3]
const arr2 = [4, 5, 6]
const arr3 = [...arr, ...arr2]
result = [1,2,3,4,5,6]
```
---

#### Creating a new object based on another
```
let anime_info = {
    show_name: 'Sword art Online',
    episodes: 24
}
const anime_info_ver2 = { ...anime_info, genre: 'Adventure' }
```
---

#### REST pattern (Left side of =) + Array Destructuring 

```
	let [anime1, anime2, ...rest] = ["Sao", "AoT", "A Silent Voice", "Naruto"]
	anime1 = "Sao"
	anime2 = "Aot"
	rest = ["A Silent Voice", "Naruto"]
	console.log (anime1, anime2, rest)
```

---

#### REST Functions & Spread
```
const add = (...numbers) => {
	sum = numbers.reduce((sum, num) => num + sum)
	console.log(sum)
}

//Using An Arbitrary amount of arguments
add(2,3)
add(5,3,7,2)

const nums = [1, 2, 3, 4]
add(...nums)
```
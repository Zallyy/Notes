# Spread ...
___
*All examples with arrays can be utilized with objects*
#### Copying an array
>`
>let copy = [...Array]
`

#### Combining two arrays 
```
const arr = [1, 2, 3]
const arr2 = [4, 5, 6]
const arr3 = [...arr, ...arr2]
result = [1,2,3,4,5,6]
```
#### Creating a new object based on another
```
let anime_info = {
    show_name: 'Sword art Online',
    episodes: 24
}

const anime_info_ver2 = { ...anime_info, genre: 'Adventure' }
```



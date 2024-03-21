# 0x03. ES6 Data Manipulation

## JavaScript - ES6

## Resources

- Read or watch:
  - [Array](#)
  - [Typed Array](#)
  - [Set Data Structure](#)
  - [Map Data Structure](#)
  - [WeakMap](#)

## Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

- How to use map, filter, and reduce on arrays
- Typed arrays
- The Set, Map, and Weak link data structures

## Requirements

- All your files will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x
- Allowed editors: vi, vim, emacs, Visual Studio Code
- All your files should end with a new line
- A README.md file, at the root of the folder of the project, is mandatory
- Your code should use the js extension
- Your code will be tested using Jest and the command `npm run test`
- Your code will be verified against lint using ESLint
- Your code needs to pass all the tests and lint. You can verify the entire project running `npm run full-test`
- All of your functions must be exported

## Setup

1. Install NodeJS 12.11.x
   - In your home directory:
     ```bash
     curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
     sudo bash nodesource_setup.sh
     sudo apt install nodejs -y
     nodejs -v
     npm -v
     ```
2. Install Jest, Babel, and ESLint

   - In your project directory, install Jest, Babel, and ESLint by using the supplied package.json and run `npm install`.

3. Configuration files
   - Add the following files to your project directory:
     - [package.json](#)
     - [babel.config.js](#)
     - [.eslintrc.js](#)
   - Don’t forget to run `npm install` when you have the package.json

## Tasks

### 0. Basic list of objects (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `getListStudents` that returns an array of objects.

```javascript
// 0-main.js
import getListStudents from "./0-get_list_students.js";

console.log(getListStudents());
```

### 1. More mapping (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function `getListStudentIds` that returns an array of ids from a list of objects.

```javascript
// 1-main.js
import getListStudentIds from "./1-get_list_student_ids.js";
import getListStudents from "./0-get_list_students.js";

console.log(getListStudentIds("hello"));
console.log(getListStudentIds(getListStudents()));
```

### 2. Filter (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function `getStudentsByLocation` that returns an array of objects located in a specific city.

```javascript
// 2-main.js
import getListStudents from "./0-get_list_students.js";
import getStudentsByLocation from "./2-get_students_by_loc.js";

const students = getListStudents();

console.log(getStudentsByLocation(students, "San Francisco"));
```

### 3. Reduce (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function `getStudentIdsSum` that returns the sum of all the student ids.

```javascript
// 3-main.js
import getListStudents from "./0-get_list_students.js";
import getStudentIdsSum from "./3-get_ids_sum.js";

const students = getListStudents();
const value = getStudentIdsSum(students);

console.log(value);
```

### 4. Combine (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function `updateStudentGradeByCity` that returns an array of students for a specific city with their new grade.

```javascript
// 4-main.js
import getListStudents from "./0-get_list_students.js";
import updateStudentGradeByCity from "./4-update_grade_by_city.js";

console.log(
  updateStudentGradeByCity(getListStudents(), "San Francisco", [
    { studentId: 5, grade: 97 },
    { studentId: 1, grade: 86 },
  ])
);

console.log(
  updateStudentGradeByCity(getListStudents(), "San Francisco", [
    { studentId: 5, grade: 97 },
  ])
);
```

### 5. Typed Arrays (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `createInt8TypedArray` that returns a new ArrayBuffer with an Int8 value at a specific position.

```javascript
// 5-main.js
import createInt8TypedArray from "./5-typed_arrays.js";

console.log(createInt8TypedArray(10, 2, 89));
```

### 6. Set data structure (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `setFromArray` that returns a Set from an array.

```javascript
// 6-main.js
import setFromArray from "./6-set.js";

console.log(setFromArray([12, 32, 15, 78, 98, 15]));
```

### 7. More set data structure (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `hasValuesFromArray` that returns a boolean if all the elements in the array exist within the set.

```javascript
// 7-main.js
import hasValuesFromArray from "./7-has_array_values.js";

console.log(hasValuesFromArray(new Set([1, 2, 3, 4, 5]), [1]));
console.log(hasValuesFromArray(new Set([1, 2, 3, 4, 5]), [10]));
console.log(hasValuesFromArray(new Set([1, 2, 3, 4, 5]), [1, 10]));
```

### 8. Clean set (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named

`cleanSet` that returns a string of all the set values that start with a specific string (`startString`).

```javascript
// 8-main.js
import cleanSet from "./8-clean_set.js";

console.log(
  cleanSet(new Set(["bonjovi", "bonaparte", "bonappetit", "banana"]), "bon")
);
console.log(
  cleanSet(new Set(["bonjovi", "bonaparte", "bonappetit", "banana"]), "")
);
```

### 9. Map data structure (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `groceriesList` that returns a map of groceries with the following items (name, quantity):

```javascript
// 9-main.js
import groceriesList from "./9-groceries_list.js";

console.log(groceriesList());
```

### 10. More map data structure (mandatory)

- **Score: 0.0% (Checks completed: 0.0%)**
- Create a function named `updateUniqueItems` that returns an updated map for all items with an initial quantity at 1.

```javascript
// 10-main.js
import updateUniqueItems from "./10-update_uniq_items.js";
import groceriesList from "./9-groceries_list.js";

const map = groceriesList();
console.log(map);

updateUniqueItems(map);
console.log(map);
```

### 11. Weak link data structure (advanced)

- **Score: 0.0% (Checks completed: 0.0%)**
- Export a const instance of WeakMap and name it `weakMap`.

```javascript
// 100-main.js
import { queryAPI, weakMap } from "./100-weak.js";

const endpoint = { protocol: "http", name: "getUsers" };
weakMap.get(endpoint);

queryAPI(endpoint);
console.log(weakMap.get(endpoint));

queryAPI(endpoint);
console.log(weakMap.get(endpoint));

queryAPI(endpoint);
queryAPI(endpoint);
queryAPI(endpoint);
queryAPI(endpoint);
```

---

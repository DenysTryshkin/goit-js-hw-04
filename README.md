**Homework Task 6. Arrays and Object Methods**

Create a repository `goit-js-hw-04` and clone it to your computer.\
In the `goit-js-hw-04` folder, create the project structure as shown in the diagram below.\
**NOTE:**\
The file and folder names, as well as their nesting structure, must match the specified diagram. Otherwise, the work will not be accepted.

Read each task and complete it in the corresponding file.\
Make sure the code is formatted with Prettier and there are no errors or warnings in the console when opening the live page of the task.\
Submit the homework for review.

**Submission Format:**\
The homework contains two links: one to the repository with the code, and the other to the live page on GitHub Pages.\
Attach the zip file of the repository.

**IMPORTANT:**\
Review the Instructions on uploading the working file from the repository to GitHub.

**Evaluation Format:**\
Pass / Fail

* * * * *

### **Task 1. Packaging Products**

**EXECUTE THIS TASK IN THE FILE task-1.js**

Write a function `isEnoughCapacity(products, containerSize)` that calculates whether all products will fit in the container during packing.

The function has two parameters:

-   `products` --- an object where the keys contain product names and the values represent the quantity of those products, e.g., `{ apples: 2, grapes: 4 }`.
-   `containerSize` --- a number that represents the maximum number of items that the container can hold.

The function should return the result of checking if all products fit in the container. That is, calculate the total number of items in the `products` object and return `true` if it's less than or equal to `containerSize`, and `false` otherwise.

Here's the code to check your function:

js

КопіюватиРедагувати

`console.log(
  isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
  isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
  isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)
); // true

console.log(
  isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)
); // false`

Leave this code for mentor verification.

**Mentor Check Criteria:**

-   The `isEnoughCapacity(products, containerSize)` function is declared.
-   The function returns `true` for `isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)`.
-   The function returns `false` for `isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)`.
-   The function returns `true` for `isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)`.
-   The function returns `false` for `isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)`.

* * * * *

### **Task 2. Calorie Calculation**

**EXECUTE THIS TASK IN THE FILE task-2.js**

Write a function `calcAverageCalories(days)` that returns the average daily calorie intake of an athlete throughout the week. The function expects one parameter: `days` --- an array of objects. Each object represents a day of the week and the number of calories consumed by the athlete on that day.

Here's the code to check your function:

js

КопіюватиРедагувати

`console.log(
  calcAverageCalories([
    { day: "monday", calories: 3010 },
    { day: "tuesday", calories: 3200 },
    { day: "wednesday", calories: 3120 },
    { day: "thursday", calories: 2900 },
    { day: "friday", calories: 3450 },
    { day: "saturday", calories: 3280 },
    { day: "sunday", calories: 3300 }
  ])
); // 3180

console.log(
  calcAverageCalories([
    { day: "monday", calories: 2040 },
    { day: "tuesday", calories: 2270 },
    { day: "wednesday", calories: 2420 },
    { day: "thursday", calories: 1900 },
    { day: "friday", calories: 2370 },
    { day: "saturday", calories: 2280 },
    { day: "sunday", calories: 2610 }
  ])
); // 2270

console.log(
  calcAverageCalories([])
); // 0`

Leave this code for mentor verification.

**Mentor Check Criteria:**

-   The `calcAverageCalories(days)` function is declared.
-   The function returns `3180` for `calcAverageCalories([...])`.
-   The function returns `2270` for `calcAverageCalories([...])`.
-   The function returns `0` for `calcAverageCalories([])`.

* * * * *

### **Task 3. Player Profile**

**EXECUTE THIS TASK IN THE FILE task-3.js**

The `profile` object describes the user's profile on a gaming platform. It contains properties such as the profile name (`username`) and the number of active hours played in the game (`playTime`).

js

КопіюватиРедагувати

`const profile = {
    username: "Jacob",
    playTime: 300,
};`

Add methods to the `profile` object to work with its properties.

-   The `changeUsername(newName)` method should accept a string (the new name) in the `newName` parameter and change the value of the `username` property to the new name. It should not return anything.
-   The `updatePlayTime(hours)` method should accept a number (the number of hours) in the `hours` parameter and increase the value of the `playTime` property by that number. It should not return anything.
-   The `getInfo()` method should return a string in the format: `<Username> has <amount> active hours!`, where `<Username>` is the profile name, and `<amount>` is the number of active hours.

Here's the code to check your function:

js

КопіюватиРедагувати

`console.log(profile.getInfo()); // "Jacob has 300 active hours!"

profile.changeUsername("Marco");
console.log(profile.getInfo()); // "Marco has 300 active hours!"

profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"`

Leave this code for mentor verification.

**Mentor Check Criteria:**

-   The `profile` variable is declared.
-   The value of `profile` is an object with properties `username`, `playTime`, `getInfo`, `changeUsername`, and `updatePlayTime`.
-   The `getInfo` property is a function.
-   The `changeUsername` property is a function.
-   The `updatePlayTime` property is a function.
-   The `this` keyword is used correctly to refer to object properties within its methods.
---------------------------------------------------------------------------------

Час швидко летить, правда ж?

Нещодавно ти й уявленя не мав, що то за об'єкти, а тепер вже знаєш як:

-   створити об'єкт у JavaScript
-   додати та змінити значення властивостей об'єкта
-   реалізувати перебирання об'єкту
-   працювати з масивом однотипних об'єктів
-   звертатися до властивості об'єкта в його методах
-   використовувати `spread` і `rest`

Саме час виконати завдання і остаточно закріпити ці вміння!

**Домашнє завдання Тема 6. Масиви та методи об'єкта**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%B4%D0%BE%D0%BC%D0%B0%D1%88%D0%BD%D1%94-%D0%B7%D0%B0%D0%B2%D0%B4%D0%B0%D0%BD%D0%BD%D1%8F-4)

-   Створи репозиторій `goit-js-hw-04` та склонюй його собі на комп'ютер.
-   У папці `goit-js-hw-04` створи структуру проєкта, як показано на схемі нижче.

**ЗВЕРНИ УВАГУ!**
Імена файлів та папок, а також їх структура вкладеності, мають відповідати вказаній схемі. В іншому разі робота не буде прийнята.

![](https://s3.eu-north-1.amazonaws.com/lms.goit.files/ccc45738-84ce-4e90-bb34-6d45c78753e74.jpg)

-   Прочитай кожне завдання і виконай його у відповідному файлі.
-   Переконайся, що код відформатований за допомогою `Prettier`, а в консолі відсутні помилки й попередження під час відкриття живої сторінки завдання.
-   Здай домашнє завдання на перевірку.

**Формат здачі:**

-   Домашня робота містить два посилання: на вихідні файли (посилання на репозиторій з кодом) і живу сторінку на `GitHub Pages`.
-   Прикрiплений файл репозиторію у форматi zip

☝ **ВАЖЛИВО**
Переглянь [**Iнструкцію щодо завантаження робочого файлу з репозиторію на Github**](https://drive.google.com/file/d/1UBw9IkvLmk4hO73ji1ScNkj3_H_vKNvT/view?usp=sharing)

**Формат оцінювання:**

-   Залiк / Незалiк

**Задача 1. Пакування товарів**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-1-%D0%BF%D0%B0%D0%BA%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F-%D1%82%D0%BE%D0%B2%D0%B0%D1%80%D1%96%D0%B2)

ВИКОНУЙ ЦЕ ЗАВДАННЯ У ФАЙЛІ `task-1.js`

Напиши функцію `**isEnoughCapacity(products, containerSize)**`, яка обчислює, чи помістяться всі товари в контейнер при пакуванні.

**Функція оголошує два параметри:**

-   `products` --- об'єкт, у якому ключі містять назви товарів, а їхні значення --- кількість цих товарів. Наприклад, `{ apples: 2, grapes: 4 }`.
-   `containerSize` --- число, максимальна кількість одиниць товарів, яку в себе може вмістити контейнер.

Функція має повернути результат перевірки, чи помістяться всі товари в контейнер. Тобто порахувати загальну кількість товарів в об'єкті `products` і повернути `true`, якщо вона менше або дорівнює `containerSize`, і `false`, якщо ні.

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її викликів.

console.log(
  isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
  isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
  isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)
); // true

console.log(
  isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)
); // false

Залиш цей код для перевірки ментором.

**На що буде звертати увагу ментор при перевірці:**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%BD%D0%B0-%D1%89%D0%BE-%D0%B1%D1%83%D0%B4%D0%B5-%D0%B7%D0%B2%D0%B5%D1%80%D1%82%D0%B0%D1%82%D0%B8-%D1%83%D0%B2%D0%B0%D0%B3%D1%83-%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D1%80-%D0%BF%D1%80%D0%B8-%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D1%96%D1%80%D1%86%D1%96)

-   Оголошена функція `isEnoughCapacity(products, containerSize)`
-   Виклик `isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)` повертає `true`
-   Виклик `isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)` повертає `false`
-   Виклик `isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)` повертає `true`
-   Виклик `isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)` повертає `false`

**Задача 2. Розрахунок калорій**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-2-%D1%80%D0%BE%D0%B7%D1%80%D0%B0%D1%85%D1%83%D0%BD%D0%BE%D0%BA-%D0%BA%D0%B0%D0%BB%D0%BE%D1%80%D1%96%D0%B9)

ВИКОНУЙ ЦЕ ЗАВДАННЯ У ФАЙЛІ `task-2.js`

Напиши функцію `**calcAverageCalories(days)**`, яка повертає середньодобове значення кількості калорій, які спортсмен споживав протягом тижня. Функція очікує один параметр: `days` --- масив об'єктів. Кожен об'єкт описує день тижня та кількість калорій `calories`, спожитих спортсменом, у цей день. Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її викликів.

console.log(
  calcAverageCalories([
    { day: "monday", calories: 3010 },
    { day: "tuesday", calories: 3200 },
    { day: "wednesday", calories: 3120 },
    { day: "thursday", calories: 2900 },
    { day: "friday", calories: 3450 },
    { day: "saturday", calories: 3280 },
    { day: "sunday", calories: 3300 }
  ])
); // 3180

console.log(
  calcAverageCalories([
    { day: "monday", calories: 2040 },
    { day: "tuesday", calories: 2270 },
    { day: "wednesday", calories: 2420 },
    { day: "thursday", calories: 1900 },
    { day: "friday", calories: 2370 },
    { day: "saturday", calories: 2280 },
    { day: "sunday", calories: 2610 }
  ])
); // 2270

console.log(
  calcAverageCalories([])
); // 0

Залиш цей код для перевірки ментором.

**На що буде звертати увагу ментор при перевірці:**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%BD%D0%B0-%D1%89%D0%BE-%D0%B1%D1%83%D0%B4%D0%B5-%D0%B7%D0%B2%D0%B5%D1%80%D1%82%D0%B0%D1%82%D0%B8-%D1%83%D0%B2%D0%B0%D0%B3%D1%83-%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D1%80-%D0%BF%D1%80%D0%B8-%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D1%96%D1%80%D1%86%D1%96-1)

-   Оголошена функція `calcAverageCalories(days)`
-   Такий виклик функції `calcAverageCalories` повертає `3180`

calcAverageCalories([
  { day: "monday", calories: 3010 },
  { day: "tuesday", calories: 3200 },
  { day: "wednesday", calories: 3120 },
  { day: "thursday", calories: 2900 },
  { day: "friday", calories: 3450 },
  { day: "saturday", calories: 3280 },
  { day: "sunday", calories: 3300 }
])

-   Такий виклик функції `calcAverageCalories` повертає `2270`

calcAverageCalories([
  { day: "monday", calories: 2040 },
  { day: "tuesday", calories: 2270 },
  { day: "wednesday", calories: 2420 },
  { day: "thursday", calories: 1900 },
  { day: "friday", calories: 2370 },
  { day: "saturday", calories: 2280 },
  { day: "sunday", calories: 2610 }
])

-   Такий виклик функції `calcAverageCalories` повертає `0`

calcAverageCalories([])

**Задача 3. Профіль гравця**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-3-%D0%BF%D1%80%D0%BE%D1%84%D1%96%D0%BB%D1%8C-%D0%B3%D1%80%D0%B0%D0%B2%D1%86%D1%8F)

ВИКОНУЙ ЦЕ ЗАВДАННЯ У ФАЙЛІ `task-3.js`

Об'єкт `profile` описує профіль користувача на ігровій платформі. У його властивостях зберігається ім'я профілю `username` та кількість активних годин `playTime`, проведених у грі.

const profile = {
 username: "Jacob",
 playTime: 300,
};

Доповни об'єкт `profile` методами для роботи з його властивостями.

-   Метод `changeUsername(newName)` повинен приймати рядок (нове ім'я) в параметр `newName` та змінювати значення властивості `username` на нове. Нічого не повертає.
-   Метод `updatePlayTime(hours)` повинен приймати число (кількість годин) у параметр `hours` та збільшити на нього значення властивості `playTime`. Нічого не повертає.
-   Метод `getInfo()` має повертати рядок формату `<Username> has <amount> active hours!`, де `<Username>` --- це ім'я профілю, а `<amount>` --- кількість ігрових годин.

Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(profile.getInfo()); // "Jacob has 300 active hours!"

profile.changeUsername("Marco");
console.log(profile.getInfo()); // "Marco has 300 active hours!"

profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"

Залиш цей код для перевірки ментором.

**На що буде звертати увагу ментор при перевірці:**[​](https://textbook.edu.goit.global/lms-js-homework-v3/uk/docs/hw-04/#%D0%BD%D0%B0-%D1%89%D0%BE-%D0%B1%D1%83%D0%B4%D0%B5-%D0%B7%D0%B2%D0%B5%D1%80%D1%82%D0%B0%D1%82%D0%B8-%D1%83%D0%B2%D0%B0%D0%B3%D1%83-%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D1%80-%D0%BF%D1%80%D0%B8-%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D1%96%D1%80%D1%86%D1%96-2)

-   Оголошена змінна `profile`
-   Значення змінної `profile` --- це об'єкт з властивостями `username`, `playTime`, `getInfo`, `changeUsername` і `updatePlayTime`
-   Значення властивості `getInfo` --- це функція
-   Значення властивості `changeUsername` --- це функція
-   Значення властивості `updatePlayTime` --- це функція
-   Для звернення до властивостей об'єкта в його методах використовується `this`
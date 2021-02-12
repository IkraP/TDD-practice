# TDD Practice

## Get started

Fork this repo so you have a copy of your own to push solutions to.

Then npm install and you can start working through the problems!

- Each set of problems has its own spec file and if you want to test out individual problems add `.only` after the describe keyword.

## Section 1 Post-Covid party

### 1 - formatGuestList

We have defeated the coronavirus! The world is celebrating and you have been put in charge of the entire extended family BBQ night. The guest list has arrived but each name is in the wrong format!

Write a function that takes an array of guests, and returns a new array of guests with their first letter capitalised.

```js
const guestList = ["ikra", "harry", "jenny", "bob"];

formatGuestList(guestList); //returns ["Ikra", "Harry", "Jenny", "Bob"]
```

### ADVANCED - formatFullName

Write a function that takes an array of guest name objects with their full name, and return a new array of guest name objects with their first and last name capitalised.

```js
const guestList = ["ikra p", "harry styles", "jenny block", "bob builder"];

formatFullName(guestList); //returns ["Ikra P", "Harry Styles", "Jenny Block", "Bob Builder"];
```

### 2 - removeDuplicates

Each family member has been given the option to add a plus one to bring to the family BBQ. As you have a close knit family, some members have decided to invite the same person to the party. Your guest list now has duplicates.

Write a function that takes an array of guests and returns an array without the duplicates

```js
const guestList = ["Ikra P", "Jenny Block", "Bob Builder", "Jenny Block"];

removeDuplicates(guestList); //returns ["Ikra P", "Jenny Block", "Bob Builder"]
```

### 3 - isThereEnoughFood

Write a function that takes an array of foods and the number of guests that will be coming and return true or false whether the food will be enough for the party.

```js
const foodList = ["shrimp", "kebabs", "biryani"];
const numberOfGuests = 3;

isThereEnoughFood(foodList, numberOfGuest); //returns true

const foodList = ["shrimp", "kebabs", "ice-cream", "biryani"];
const numberOfGuests = 12;

isThereEnoughFood(foodList, numberOfGuest); //returns false
```

### 4 - bringPresents

This party is a chance to exchange gifts that were missed during Christmas/Eid. Not all guests will be bringing a gift so your family wants to be ready if they do so they can give one in return.

Write a function that takes an array of guest objects with their name and whether they will be bringing a present and return an array of objects with only the guests that will be bringing presents.

```js
const guestList = [
  { name: "Ikra P", bringPresent: true },
  { name: "Jenny Block", bringPresent: false },
  { name: "Bob Builder", bringPresent: false },
];

bringPresents(guestList); //returns  [{ name: "Ikra P", bringPresent: true }]
```

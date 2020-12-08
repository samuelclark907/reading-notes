# READ-09-REFACTORING

## Concepts of Functional Programming in Javascript

- Functional Programming - is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### Pure Functions

- It returns the same result if given the same arguments.

- It does not cause any observable side effects.

- If our function reads external files, it’s not a pure function — the file’s contents can change.

- Any function that relies on a random number generator cannot be pure.

### Immutability

- When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

### Referentially Transparent

- If a function consistently yields the same result for the same input.

## Refactoring JavaScript for Performance and Readability

### Unrefactored

const friendlyWords = require('friendly-words');

function randomPredicate() {
  const choice = Math.floor(Math.random() * friendlyWords.predicates.length);
  return friendlyWords.predicates[choice];
}

function randomObject() {
  const choice = Math.floor(Math.random() * friendlyWords.objects.length);
  return friendlyWords.objects[choice];
}

async function createUser(email) {
  const user = { email: email };
  user.url = randomPredicate() + randomObject() + randomObject();
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}

### Refactored

const friendlyWords = require('friendly-words');

const generateURL = user => {
  const pick = arr => arr[Math.floor(Math.random() * arr.length)];
  user.url = `${pick(friendlyWords.predicates)}-${pick(friendlyWords.objects)}` +
    `-${pick(friendlyWords.objects)}`; // This line would've been too long for linters!
};

async function createUser(email) {
  const user = { email: email };
  // The URL-creation algorithm isn't important to this function so let's abstract it away
  generateURL(user);
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}


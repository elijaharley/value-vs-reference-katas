**Northcoders Fundamentals Value Vs Reference Katas**

_Each kata should be completed with full TDD._

**Learning Objectives**

- Practice Test Driven Development.
- Testing that the original input is unchanged
- Testing that new objects & arrays have their own reference in memory.

**Tasks**

**pineapplePizzaParty**

![pineapple](https://ychef.files.bbci.co.uk/976x549/p0ctz0wr.jpg?width=275&height=488)
Following a heated debate in the zoom chat about whether pineapple on pizza is
'Yay' or 'Nay' a prankster has infiltrated the NC Graduation Day pizza orders
and added pineapple to all of the orders. Create a function that takes a single
pizza ingredients array and returns a _new_ array without pineapple _unless_
it's pineapple paired with ham. This function should not mutate the input array
.

```js
pineapplePizzaParty([ham, pineapple, mozzarella]);

//should return

[ham, pineapple, mozzarella];
```

```js
pineapplePizzaParty([pepperoni, chilli, mozzarella, pineapple]);

//should return

[pepperoni, chilli, mozzarella];
```

**isItVegan**

The Graduation Day Pizzas can now be ordered but the ordering system has
changed. Create a function that takes a single person object and changes the
'isVegan' key to a key of 'dietaryRequirements' returning a _new_ object. This
function should not mutate the original tutor object.

```js
isItVegan({Tutor: 'Doug', isVegan: true})

// should return

{ Tutor: 'Doug', dietaryRequirements: 'vegan' };
```

```js
isItVegan({Tutor: 'Paul', isVegan: false})

// should return

{ Tutor: 'Paul', dietaryRequirements: 'none' };
```

**sameOrCopy**

![Spiderman](https://images.news18.com/ibnlive/uploads/2021/12/spiderman-meme-16401651633x2.png?impolicy=website&width=255&height=178)

<!-- write this one -->

This function should take an array of objects and a single object, it should
find any matching objects in the array and check if they are in fact the same
object or whether they are a copy of the original.

```js
const spiderman = { name: 'Spiderman' };
sameOrCopy(
  [spiderman, { name: 'Wonderwoman' }, { name: 'Wolverine' }],
  spiderman
);

//should return

("Peter Parker! It's you!");
```

```js
sameOrCopy(
  [{ name: 'Spiderman' }, { name: 'Wonderwoman' }, { name: 'Wolverine' }],
  { name: 'Spiderman' };
);

//should return

'Holy Smokes Batman, it\s just a Joker in a Halloween Costume'
```

**rickRoll**

![Rick](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRzz0BMm1ZoaAXqRLMRVqi4XbXNqUX1lup-ow&usqp=CAU)

Eli has an evil plan RickRoll the NC Staff by to changing everyone's favourite
song on the NC Playlist to be Rick Astley 'Never Gonna Give You Up'.

Create a function that takes an array of tutor objects, and changes the _song_
property on each object to be 'Never Gonna Give You Up' returning a _new_ array
of the same length. This function should not mutate the original staff playlist.

```js
rickRoll([
  { name: 'Danika', song: 'Rebel Girl' },
  { name: 'Verity', song: '7 wonders' },
  { name: 'Emily', song: 'Under the Bridge' },
  { name: 'Carrie', song: 'The Chain' },
  { name: 'Cat', song: 'Yoshimi Battles the Pink Robots pt 1' }
]);

//should return

[
  { name: 'Danika', song: 'Never Gonna Give You Up' },
  { name: 'Verity', song: 'Never Gonna Give You Up' },
  { name: 'Emily', song: 'Never Gonna Give You Up' },
  { name: 'Carrie', song: 'Never Gonna Give You Up' },
  { name: 'Cat', song: 'Never Gonna Give You Up' }
];
```

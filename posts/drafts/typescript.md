---
title: 'What is TypeScript'
description: 'Just going to explain simple topics using basic logics here'
createdAt: '2024-02-01'
topic: 'WEB_DEVELOPMENT'
subTopic: null
author: 'Ghislain Genay'
updatedAt: 'xxxx-xx-xx'
readTime: '2 min read'
keywords: []
tags: ['web-development', 'javascript']
language: 'en'
level: 'BEGINNER'
series: 'TYPESCRIPT'
series_num: 1
---

# What is TypeScript ?

TypeScript is a language which is a vanilla Javascript language with types.

This types allows to avoid typing errors during code compiling time.

Examples of errors:

1. This variable name doesn't exists
2. You requested a type of string but this is number
3. You didn't provide the type, please provide one

That is why TypeScript is soo powerful. So powerful that I don't use vailla Javascript anymore
For those who don't know how to use TypeScript, let's do a simple reminder.

> I won't talk abouyt inference here. Inference is where you didn't specify the type but TypeScript is smarking enough to know what is it.

When using Typescript, you use semi colon and the type between the variable name and equals sign
Some primitives types (non echanst) are: `boolean`, `string`, `number`, `object`, `null`, `undefined`, `any`

```ts
let text: string = 'Hello';
let age: number = 20;

let adultAge = 18; // in France
let isAdult: boolean = age >= adultAge;

// If ou try to assign the wrong type, TypeScript will complain and you won't be able to run your code
let age = '20'; // '20' is a string type and not a number
```

Let's see the examples of errors I mentioned above with examples.
But before, i want to explain what is interface. If you have an object with differents properties (keyèvalues âit), you can use an interface or type to specify this

```ts
interface UserInterface {
	name: string;
	age: string;
	lastName: boolean;
}

type UserType = {
	name: string;
	age: string;
	lastName: boolean;
};

const user: UserInterface = {
	name: 'Peter',
	age: 25,
	lastName: 'Doe'
};

const user: UserType = {
	name: 'Emma',
	age: 32,
	lastName: 'Tival'
};
```

Interface or type have similar roles in this case ad you can interchange it most of the time.

Main differences betwsen interfaces or type

```ts
// interface can be extends
ed;
```

Interface
API : object might changes

Do you want a more in-depth TypeScript post, please let me know in the comments.

```ts
// This variable name doesn't exists
```

### Introduction to TypeScript

1. the TypeScript has `static types`, instead JavaScript has `dynamic types`
2. The types in TS are always written in a lower case
3. In TypeScript there are core types, such as: `number`, `string`, `boolean`, `object`,
   **An Example with object typization in TS**

```tsx
const person: {
  name: string;
  age: number;
} = {
  name: "Vitalii",
  age: 20,
};
```

4. Nested object types
   Let's say you have this JavaScript object:

```tsx
const product = {
id: 'abc1',
price: 12.99,
tags: ['great-offer', 'hot-and-new'],
details: {
    title: 'Red Carpet',
    description: 'A great carpet - almost brand-new!'
}
}
```
This would be the type of such an object:

```tsx
{
  id: string;
  price: number;
  tags: string[];
  details: {
    title: string;
    description: string;
  }
}
```
So you have an object type in an object type so to say.

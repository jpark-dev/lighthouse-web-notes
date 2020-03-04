## JS typeof vs Array.isArray() for arrays

typeof always return object for arrays, objects... etc.
isArray() returns boolean which is more type specific.

```javascript
typeof([]) // => "object"
```

```javascript
typeof([{}]) // => "object"
```
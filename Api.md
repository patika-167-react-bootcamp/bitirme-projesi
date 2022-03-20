# Auth

## POST Register

`/auth/register`

**Body**

```js
{
  username: "string" require,
  password: "string" require,
  passwordConfirm: string require
}
```

## POST Login

`/auth/login`

**Body**

```js
{
  username: "string" - require,
  password: "string" - require
}
```

# Board

## POST Create

`/board`

**Body**

```js
{
  title: string - require,
  members: array[number] - optional
}
```

## PUT Update

`/board/:id`

**Body**

```js
{
  title: string - require,
  members: array > number - optional
}
```

## DEL Destroy

`/board/:id`

## GET Get By Id

`/board/:id`

## GET Get List

`/board`

# List

## POST Create

`/list`

**Body**

```js
{
  title: "string" - require,
  boardId: number - require,
}
```

## PUT Update

`/list/:id`

**Body**

```js
{
  title: "string" - optional
  boardId: number - optional,
  order: number - optional
}
```

## DEL Destroy

`/list/:id`

## GET Get By Id

`/list/:id`

## GET Get List

`/list`

**Query**

```js
{
  boardId: number - optional;
}
```

# Card

## POST Create

`/cart`

**Body**

```js
{
  title: "string" - require,
  listId: number - require,
  description: string - optional,
  duedate: date - optional,
}
```

## PUT Update

`/cart/:id`

**Body**

```js
{
  title: "string" - optional,
  listId: number - optional,
  description: "string" - optional,
  duedate: date - optional,
  order: number - optional
}
```

## DEL Destroy

`/cart/:id`

## GET Get By Id

`/cart/:id`

## GET Get List

`/cart`

**Query**

```js
{
  listId: number - optional;
}
```

# Board Member

## POST Create

`/board-member`

**Body**

```js
{
  username: "string" - require,
  boardId: number - require,
}
```

## DEL Destroy

`/board-member/:id`

## GET List

`/board-member`

**Query**

```js
{
  boardId: number - optional;
}
```

# Cart Label

## POST Create

`/card-label`

**Body**

```js
{
  cardId: number - require,
  labelId: number - require,
}
```

## DEL Destroy

`/card-label/:id`

## GET List

`/card-label`

# Comment

## POST Create

`/comment`

**Body**

```js
{
  cardId: number - require,
  message: string - require,
}
```

## DEL Destroy

`/comment/:id`

# Check List

## POST Create

`/checklist`

**Body**

```js
{
  cardId: number - require,
  title: "string" - require,
}
```

## PUT Update

`/checklist/:id`

**Body**

```js
{
  title: "string" - require,
}
```

## DEL Destroy

`/checklist/:id`

# Check List Item

## POST Create

`/checklist-item`

**Body**

```js
{
  checklistId:  number - require,
  isChecked:  boolean - require,
  title:  "string" - require
}
```

## PUT Update

`/checklist-item/:id`

**Body**

```js
{
  isChecked: boolean - optional,
  title: "string" - optional,
}
```

## DEL Destroy

`/checklist-item/:id`

# Label

## GET List

`/label`

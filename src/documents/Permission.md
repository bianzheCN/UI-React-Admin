# Permission

## Why

Different should have different permission to do CRUD(create, read, update, delete) on resources.

## Strategy

Assign each user different permission keys to allow them enjoy the actions on resources, such as a user has permission to click button, I will assign the user `create`.
And The reason for it's 'create' is that this action will add a record in the back-end.

So for each user, there will be a array in the end to decide whether they are allowed to do something. If your backend has different strategy, you should do a mapping to make it the way we are implementing.

## API

```javascript
{ 
    user1:  {
        name: 'user1',
        feature1: ['create', 'delete', 'update', 'remove']
        feature2: ['create', 'delete']
    },
    user2: {
        name: 'user2',
        feature1: ['create', 'delete', 'update', 'remove']
    }
}
```

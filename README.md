# CS568 - Assignment 3, 4 - Props, State, Event Handler, List, Conditionals

## Micro tasks
1. Implement the Counter example with increment and decrement, both class-based and functional (using a hook) way.
2. Implement the [Updater function in setState](https://react.dev/learn/adding-interactivity#queueing-a-series-of-state-updates) example.

## Main task
Implement the Todo app. All your data is in your App.js. Pass `todoItems` array down to TodoItem component. When click on the delete button, remove the todo item from the todo list.
```
App (tasks, addTask(), deleteTask())
├─ TodoAdd (newTask, addTaskOnClick())
├─ TodoList (isShown)
│  └─ TodoItem
│     ├─ TodoDeleteButton
│     └─ TodoEditButton
└─ TodoFooter
```

##

* Implement the [Lift-state-up](https://react.dev/learn/sharing-state-between-components#lifting-state-up-by-example) example.

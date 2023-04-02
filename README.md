# CS568 - Assignment 3, 4 - Props, State, Event Handler, List, Conditionals

## Micro tasks
1. Implement the Counter example with increment and decrement, both class and functional (using a hook) way.
2. Implement the "Lift-state-up" example that I demonstrated in class.
3. Implement the "Updater function in setState" example that I demonstrated in class.

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

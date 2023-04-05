# CS568 - Assignment 3 - State, Event Handler

## Micro tasks
1. Understand the "Snapshot" example.
```
console.log(count); // 0
setCount(count + 1); // Request a re-render with 1
console.log(count); // Still 0!
```

2. Understand the "Updater function" example.
```
import { useState } from 'react';
import './App.css';

function App() {
  const [cntr, setcntr] = useState(0);

  return (
    <div className="App">
      <p>Counter: {cntr}</p>
      <button onClick={
        () => {
          setcntr(cntr => cntr + 1);
          setcntr(cntr => cntr + 1);
          setcntr(cntr => cntr + 1);
        }
      }>+3</button>
    </div>
  );
}

export default App;
```
3. Understand the following. Don't copy and paste. Try to understand what happens under the hood.
```
import { useState } from "react";
import "./App.css";

function App() {
  const [student, setStudent] = useState({ id: 1234, name: "s1", age: 12 });

  function incrementAge() {
    const newStudent = { ...student };
    newStudent.age = newStudent.age + 1;
    setStudent(newStudent);
  }

  return (
    <div className="App">
      <Student
        id={student.id}
        name={student.name}
        age={student.age}
        incrementAge={incrementAge}
      />
    </div>
  );
}

function Student({ id, name, age, incrementAge }) {
  return (
    <>
      <p>
        student id: {id}, name: {name}, age: {age}
      </p>
      <button onClick={incrementAge}>increment by one</button>
    </>
  );
}

export default App;
```

## Extra

* Implement the [Lift-state-up](https://react.dev/learn/sharing-state-between-components#lifting-state-up-by-example) example.

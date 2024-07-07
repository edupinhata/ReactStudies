# ReactStudies
Repository with react course studies

## Imports

### Import images

```react
import reactImage from './assets/example_image.jpg'

...


function App(){
  return (
    <header>
      <img src={reactImage} alt="Image description" />
      ...
    </header>
  );
}
```

## Props

Example:

```
export function CourseGoal(concept) {
  return (
    <li>
      <h2>{concept.title}</h2>
      <p>{concept.description}</p>
    </li>
  );
}

function App() {
  return (
    <div id="app" data-testid="app">
      <h1>Time to Practice</h1>
      <p>One course, many goals! 🎯</p>
      <ul>
        <CourseGoal {...DEFAULT_COURSES[0]}/>
        <CourseGoal {...DEFAULT_COURSES[1]}/>
        {/* One of them should have a title of “Learn React” and a description of “In-depth” */}
      </ul>
    </div>
  );
}
```

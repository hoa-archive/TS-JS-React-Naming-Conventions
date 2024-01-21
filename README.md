# TS-JS-React-Naming-Conventions


#### React Project File Structure
```
src/
├── App.tsx
├── main.tsx
├── main.css
├── assets/
├── components/
│   └── InputButton/
│       └── InputButton.tsx
├── contexts/
│   ├── modal.context.ts
│   └── todo-list.context.ts
├── hooks/
│   ├── use-auth.hook.ts
│   └── use-modal.hook.ts
├── services/
├── pages/
└── utils/
```

 - assets - images, global styles
 - layouts - header, footer, sidebar, navbar (components available to entire project)
 - components - ui elements: buttons, modals, inputs, loaders etc (used across many files)
 - pages - each page in a project
 - middleware - side effects in app; store redux actions
 - routes - private, protected, public, sub routes in app
 - config - env variables in config.js, other configs
 - services - with redux (actions, reducers, constant), apis
 - utils - utility functions
 - data - objects, dropdown options, regex conditions, formatting, constants
 - hooks - custom hooks
 - context - useContext hook
 - lib - facades for imported libraries
 - features - manage new features in app


#### Case Styles
 -  Pascal case (e.g. FirstName) 
 -  Camel case (e.g. firstName) 
 -  Snake case (e.g. first_name) 
 -  Kebab case (e.g. first-name)


#### File Naming Convention
 - React components and folders, pascal case: ./InputButton/InputButton.tsx
 - React events, camel case: onUsernameInputChange, onAlertClick, onFormSubmit
 - React event handlers, camel case: handleUsernameInputChange, handleAlertClick, handleFormSubmit
 - React hooks/context/tests, kebab case dot append: todo-list.test.ts 
 - General JS files, kebab-case or snake_case: pick one and be consistent


#### General Naming Convention
 - variables - camelCase: firstName 
 - boolean - camelCase with keywords: isAvailable
 - class - PascalCase: class Person {}
 - functions/methods - camelCase with action verbs: getFullName()
 - constants - uppercase SNAKE_CASE: FIRST_NAME = "Greg";
 - immutable global variables - uppercase SNAKE_CASE
 - mutable global variables - lowercase camelCase


#### ASCII Box Drawing Characters
```
 179  │    185  ╣
 180  ┤    186  ║
 191  ┐    187  ╗
 192  └    188  ╝
 193  ┴    200  ╚
 194  ┬    201  ╔
 195  ├    202  ╩
 196  ─    203  ╦
 197  ┼    204  ╠
 217  ┘    205  ═
 218  ┌    206  ╬
```


#### References
 - https://www.bigscal.com/blogs/frontend-technology/understanding-react-project-structure-and-folder-setups/
 - https://www.xenonstack.com/insights/reactjs-project-structure
 - https://blog.webdevsimplified.com/2022-07/react-folder-structure/
 - https://medium.com/@kthamodaran/react-8-best-practices-folder-structure-5dbda48a69e
 - https://www.joshwcomeau.com/react/file-structure/
 - https://profy.dev/article/react-folder-structure
 - https://maxrozen.com/guidelines-improve-react-app-folder-structure
 - https://jaketrent.com/post/naming-event-handlers-react/
 - https://stackoverflow.com/questions/60048249/what-is-the-right-name-of-event-handler-onclick-or-handleclick
 - https://www.makeuseof.com/tag/10-tips-writing-cleaner-better-code/
 - https://elser.hashnode.dev/javascript-naming-convention-for-beginners
 - https://www.syncfusion.com/blogs/post/top-javascript-naming-convention.aspx


#### Notes
Git Naming Conventions
 - https://dev.to/varbsan/a-simplified-convention-for-naming-branches-and-commits-in-git-il4

React Project Structure
 - https://github.com/alan2207/bulletproof-react/blob/master/docs/project-structure.md

Git Commit Standards
 - https://karma-runner.github.io/1.0/dev/git-commit-msg.html
 - https://medium.com/@naandalist/creating-a-git-commit-message-convention-for-your-team-acb4b3edfc44


#### types:
 - feat - new features
 - fix - bug fixes
 - docs - changes to documentation
 - style - formatting and styling; no prod changes
 - refactor - changes to prod code; i.e. renaming a variable
 - test - add tests, refactor tests; no prod changes
 - chore - file changes that dont affect user; updating gitignore or prettier etc
 - build - changes to build system or external dependencies
 - perf - changes to code that improve performance

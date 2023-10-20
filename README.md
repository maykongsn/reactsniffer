# ReactSniffer 

## Installation

Use the package manager [npm](https://www.npmjs.com/) to install locally.

```bash
npm install -g git+https://github.com/maykongsn/reactsniffer.git
```

## Usage

To use this tool you need to provide the repository directory (e.g., myproject/src)

```bash
reactsniffer myproject/src
```

### Output

The output will show the smells into two summarized tables.

Two CSV files (one per file and another by component) with more details about each smell will be generated.

## Supported Smells

ReactSniffer supports the following smells: 

| Smell      | Description                                                                             |
|------------|-----------------------------------------------------------------------------------------|
| Large Component                    | Component with too many props, attributes, and/or lines of code |
| Too Many Props                     | Passing too many properties to a single component               |
| Inheritance Instead of Composition | Using inheritance to reuse code among components                |
| Props in Initial State             | Initializing state with props                                   |
| Direct DOM Manipulation            | Manipulating DOM directly                                       |
| Force Update                       | Forcing the component or page to update                         |
| JSX outside the render method      | Implementing markup in multiple methods                         |
| Uncontrolled Components            | A component that does not use props/state to handle form's data |
| Large File                         | A file with several components and lines of code                |
| Any Type                           | Defining the type any for an element in the code |
| Many Non-Null Assertions           | Using non-null operator to indicate that a property will not be null or undefined |
| Missing Union Type Abstraction     | When union types are not used with type aliases |
| Enum Implicit Values               | Using enums without defining explicit values for them |
| Multiple Booleans for State        | Defining many boolean-type states to define the component's state |
| Children Props Pitfall             | Children props using any or types that can restrict JSX elements and affect readability      |

## License

[MIT](https://choosealicense.com/licenses/mit/)
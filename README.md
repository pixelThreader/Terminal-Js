# Terminal.js

`Terminal.js` is a lightweight JavaScript library that enables you to create interactive and customizable terminal interfaces directly on your webpage. With built-in reserved commands and a fully customizable user interface, `Terminal.js` brings the charm of terminal interactions to the web.

## Features

- **Predefined Commands**: Includes a set of reserved commands such as:
  - `cat`
  - `date`
  - `time`
  - `/contact`
  - `/resume`
- **Customizable Interface**: The library allows users to override the default settings to create a unique and personalized terminal UI.
- **Interactive Experience**: Simulates a terminal-like environment, providing an engaging way to interact with your webpage.

## Installation

To get started, include the library in your project:

```html
<script src="path/to/terminal.js"></script>
```

Or, install it via npm:

```bash
npm install terminal.js
```

## Usage

### Basic Setup

Initialize the terminal by attaching it to a DOM element:

```javascript
const terminal = new Terminal({
  element: document.getElementById("terminal-container"),
});
```

### Adding Commands

You can extend the terminal by adding custom commands:

```javascript
terminal.addCommand("greet", (args) => {
  terminal.print(`Hello, ${args.join(" ")}!`);
});
```

### Customizing the UI

Override the default styles to create a unique appearance:

```javascript
terminal.setOptions({
  prompt: "> ",
  theme: {
    background: "#000000",
    color: "#00FF00",
  },
});
```

### Reserved Commands

The following commands are predefined and ready to use:

- `cat`: Display file contents.
- `date`: Show the current date.
- `time`: Show the current time.
- `/contact`: Provide contact information.
- `/resume`: Show the resume or related details.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

# Umbral

**Master the Multiverse of Code**

Umbral is a powerful, multi-language programming environment that allows you to integrate, execute, and manage code across various programming languages seamlessly. By bridging the gap between different languages, Umbral provides a unified platform to reveal the hidden connections in your code, enhancing productivity and collaboration in multi-language projects.

## Features

- **Multi-language Execution**: Run code from Python, JavaScript, TypeScript, and more within a single script.
- **Unified Variable Sharing**: Seamlessly share variables and data across different language blocks without manual conversions.
- **Integrated Import System**: Import libraries and modules specific to each language, simplifying the setup of complex environments.
- **Advanced Control Flow**: Utilize if statements, loops, and functions across multiple languages with coherent and consistent syntax.
- **TypeScript Support**: Leverage TypeScript’s type safety and advanced features alongside Python and JavaScript.
- **Error Handling and Debugging**: Catch and manage errors across languages in a unified way to ensure robust execution.

## Usage

### Basic Structure

Umbral scripts are divided into shared variables, import blocks, language-specific code blocks, and control structures. Here’s a quick example:

```umbral
# Shared variables
shared {
    var x = 10
    var message = "Hello from Umbral!"
}

# Python imports
python::pckages {
    import numpy as np
}

# Python block
python {
    x = np.sum([x, 20])
    print(f"Python says: {x}")
}

# JavaScript imports
javascript::pckages {
    const fs = require('fs');
}

# JavaScript block
javascript {
    fs.writeFileSync('output.txt', message);
    console.log("JavaScript wrote the message to file.");
}

# TypeScript imports
typescript::pckages {
    import { format } from 'date-fns';
}

# TypeScript block
typescript {
    const now = new Date();
    console.log(`Current time: ${format(now, 'yyyy-MM-dd HH:mm:ss')}`);
}

# Main block with control flow
main {
    if (x > 20) {
        print("All blocks executed successfully with x > 20.")
    }
}
```

### Advanced Features

1. **Functions Across Languages**:
   Define and call functions across different language blocks, passing arguments and returning values.

2. **Error Handling**:
   Use try-catch blocks to manage exceptions across language executions for robust and reliable scripting.

3. **Async and Parallel Execution**:
   Utilize async/await patterns and parallel processing capabilities within and across language blocks for high-performance workflows.

## Contributing

We welcome contributions from the community! Here's how you can get involved:

1. **Fork the Repository**: Start by forking the repo and cloning it locally.
2. **Create a Branch**: Use feature branches (`git checkout -b feature/your-feature`) for your work.
3. **Commit Your Changes**: Write clear commit messages (`git commit -m 'Add new feature'`).
4. **Submit a Pull Request**: Push your branch to GitHub and submit a pull request to the main branch.

Please make sure your contributions align with our [Code of Conduct](CODE_OF_CONDUCT.md) and include appropriate tests and documentation.

## Roadmap

- **Expand Language Support**: Add support for additional languages like Ruby, Go, and more.
- **Enhanced Debugging Tools**: Improve the debugging experience with integrated tools and better error messages.
- **Community Plugins**: Allow for plugins and extensions to further customize and enhance Umbral’s capabilities.

## License

Umbral is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

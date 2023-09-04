# Link Extractor Program 🌐

Welcome to the Link Extractor program documentation! This guide will introduce you to a powerful tool for extracting links from web pages. Whether you're a developer or just curious, you'll find this program useful. Let's dive in and explore its features! 🚀

## Table of Contents

- [Introduction](#introduction)
- [Error Handling](#error-handling)
- [How it Works](#how-it-works)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Link Extractor program is a Rust application that allows you to extract hyperlinks from a web page. It utilizes popular Rust libraries such as `reqwest` for making HTTP requests and `select` for HTML parsing.

## Error Handling

We've implemented error handling using the `error_chain` crate to provide clear and concise error messages. Here are the main error types:

- `ReqError`: Represents errors from the `reqwest` library when making HTTP requests.
- `Io`: Represents errors related to input and output operations.

## How it Works

This program:

1. Sends an HTTP GET request to a specified URL (in this case, "https://www.rust-lang.org/en-US/").
2. Retrieves the HTML content of the web page.
3. Parses the HTML content to find all anchor (`<a>`) elements.
4. Extracts the `href` attribute of each anchor element.
5. Prints the extracted links to the console.

## Usage

To use the Link Extractor program, follow these steps:

1. Ensure you have Rust installed on your system.

2. Clone the repository and navigate to the project directory:

   ```bash
   git clone https://github.com/your-username/link-extractor.git
   cd link-extractor
   ```

3. Build and run the program:

   ```bash
   cargo build
   cargo run
   ```

   This will execute the program and print the extracted links to the console.

## Contributing

Contributions are welcome! If you have ideas for improvements or find any issues, please feel free to open a pull request. Let's work together to enhance this useful tool.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the program according to the terms of the license.

---

Explore the Link Extractor program, empower your web scraping projects, and unlock the world of hyperlinks with ease. Happy link extracting! 🌐🔗

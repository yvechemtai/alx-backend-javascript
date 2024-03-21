# 0x00. ES6 Basics

## Overview

This project focuses on fundamental concepts in ES6 (ECMAScript 2015), with an emphasis on modern JavaScript and software linting. The tasks cover topics such as arrow functions, default parameters, rest parameters, string templating, object creation, iterators, and more.

## Project Details

- **Author:** Johann Kerbrat, Engineering Manager at Uber Works
- **Weight:** 1
- **Start Date:** Nov 27, 2023 6:00 AM
- **End Date:** Nov 28, 2023 6:00 AM
- **Checker Release:** Nov 27, 2023 12:00 PM
- **Auto Review:** Will be launched at the deadline

## Concepts Covered

- Modern JavaScript
- Software Linter

## Resources

Read or watch the following resources before starting the tasks:

- [ECMAScript 6 - ECMAScript 2015](link-to-resource)
- [Statements and declarations](link-to-resource)
- [Arrow functions](link-to-resource)
- [Default parameters](link-to-resource)
- [Rest parameter](link-to-resource)
- [Javascript ES6 — Iterables and Iterators](link-to-resource)

## Learning Objectives

By the end of this project, you should be able to:

1. Explain what ES6 is.
2. Describe the new features introduced in ES6.
3. Understand the difference between a constant and a variable.
4. Grasp the concept of block-scoped variables.
5. Use arrow functions and function parameters defaulting to them.
6. Work with rest and spread function parameters.
7. Implement string templating in ES6.
8. Understand object creation and properties in ES6.
9. Use iterators and for-of loops.

## Requirements

### General

- All files should be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x.
- Allowed editors: vi, vim, emacs, Visual Studio Code.
- Files should end with a new line.
- Include a `README.md` file at the root of the project folder.

### Code

- Use the `.js` extension for your code.
- Code will be tested using the Jest Testing Framework.
- Code will be analyzed using the ESLint linter with specific provided rules.
- All functions must be exported.

## Setup

1. Install NodeJS 12.11.x in your home directory:
   ```bash
   curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
   sudo bash nodesource_setup.sh
   sudo apt install nodejs -y
   ```
   Verify installations:
   ```bash
   nodejs -v
   npm -v
   ```

2. Install Jest, Babel, and ESLint:
   In your project directory, run:
   ```bash
   npm install
   ```

3. Configuration files:
   Add the following files to your project directory:
   - `package.json`
   - `babel.config.js`
   - `.eslintrc.js`

4. Run `npm install` from the terminal in your project folder to install all necessary project dependencies.

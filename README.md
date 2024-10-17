
# Build Instructions

This project uses webpack and npm. Npm helps to install and update all libraries with only one simple command: `npm update`. Webpack helps to bundle many different JS and CSS files into one `bundle.js`, significantly improving page load time.

## Requirements

- **GIT**: Free and open source distributed version control system.
- **npm**: Package manager that helps to manage dependencies. Update it to the latest version using `npm install npm@latest -g`. Make sure you have at least version 6: `npm run build`.

## Build Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/viliusle/miniPaint.git
   ```
2. Navigate into the project directory:
   ```bash
   cd miniPaint
   ```
3. Install all dependencies from `package.json` file into the `node_modules` folder:
   ```bash
   npm install
   ```
4. There are two ways to edit files:
   - Run `npm run server` to create a simple local server (webpack-dev-server) with live reload. You can edit files and debug using `http://localhost:8080/`. This is the recommended way.
   - Edit files and run the command `npm run dev` to generate/update `dist/bundle.js`.

5. To generate minified code for production, run:
   ```bash
   npm run build
   ```
   This command builds the code using webpack.

## Useful Commands

- `npm update`: Installs all required libraries from the `package.json` file into the `node_modules` folder.
- `npm run`: Lists all possible npm run commands (AKA help).
- `npm run server`: Creates a `http://localhost:8080/` server for easy development (also with live reload).
- `npm run dev`: Creates or updates the `dist/bundle.js` file, so your changes will be visible.
- `npm run build`: Builds for production.

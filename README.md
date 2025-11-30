# Template Package

A template repository for creating npm packages quickly and easily.

## What's Included

- Pre-configured `package.json` with common fields
- Source code structure (`src/index.js`)
- Git repository setup
- Basic module export example

## How to Use This Template

1. **Click "Use this template"** button on GitHub (or clone this repo)
2. **Clone your new repository:**
```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-NEW-PACKAGE.git
   cd YOUR-NEW-PACKAGE
```

3. **Update package.json:**
   - Change `name` to your new package name (e.g., `@rffgrayson/my-new-package`)
   - Update `description`
   - Update `repository` URLs
   - Update `homepage` and `bugs` URLs

4. **Write your code** in `src/index.js`

5. **Test locally:**
```bash
   npm link
```

6. **Login to npm** (first time only):
```bash
   npm login
```

7. **Publish your package:**
```bash
   npm publish --access public
```

## Testing Your Package

After publishing, test it:
```bash
mkdir test-directory
cd test-directory
npm install @rffgrayson/YOUR-PACKAGE-NAME
```

Create a `test.js` file:
```javascript
var myPackage = require('@rffgrayson/YOUR-PACKAGE-NAME');
myPackage.printMsg();
```

Run: `node test.js`

## Project Structure
```
.
├── src/
│   └── index.js        # Main entry point
├── package.json        # Package configuration
├── .gitignore         # Git ignore rules
├── .npmignore         # npm ignore rules
└── README.md          # This file
```

## License

MIT
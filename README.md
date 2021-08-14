# Tailwind-CSS-Starter-Pack

## **Two way to start with tailwindcss**

### **Clone From**:

```
git clone https://github.com/Joyontokarmakar/tailwind-css-starter-pack.git
```
#### **Then You need to install and build this repository on your PC**.
```
npm i
npm run build
```

------------------------------------------------------------------------------------------

### **How to Create this**
```
npm init -y
npm i tailwindcss@latest postcss-cli@latest autoprefixer@latest
```

#### Tailwind Full Config
```
npx tailwindcss init --full ( change name to tailwind-default.config.css )
```

#### Tailwind & Postcss Config
```
npx tailwindss init -p
```

#### Edit on your package.json file

```javascript
"scripts": {
    "build": "postcss src/css/tailwind.css -o src/css/tailwind-build.css -w",
    "prod": "NODE_ENV=production postcss src/css/tailwind.css -o src/css/tailwind-build.css"
  }
```

#### To remove unused css => edit the "tailwind.config.js" file

```javascript
  purge: [
    './src/**/*.html',
		'./src/**/*.js',
  ],
```


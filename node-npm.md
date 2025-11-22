<h1> NODE.JS + NPM COMMAND </h1>

---

# ⚡ 1. **Node.js Commands (Professional Level)**

### **Run a JS file**

```
node app.js
```

### **Start REPL shell**

```
node
```

### **Check version**

```
node -v
```

### **Run file with experimental flags**

```
node --experimental-modules app.js
node --trace-warnings app.js
```

### **Run with debugging**

```
node --inspect app.js
node --inspect-brk app.js
```

### **Set environment variables**

```
NODE_ENV=production node app.js
```

Windows CMD:

```
set NODE_ENV=production && node app.js
```

### **Run with increased memory**

```
node --max-old-space-size=4096 app.js
```

---

# 🟦 2. **NPM Commands (Most Common at Work)**

### **Init project**

```
npm init -y
```

### **Install dependency**

```
npm install express
```

### **Install dev dependency**

```
npm install nodemon --save-dev
```

### **Remove dependency**

```
npm uninstall express
```

### **Update all packages**

```
npm update
```

### **Check outdated packages**

```
npm outdated
```

### **Audit security**

```
npm audit
npm audit fix
```

### **Global installs**

```
npm install -g nodemon
```

---

# 🟣 3. **NPM Scripts (Professional Use)**

### **Run script**

```
npm run start
npm run dev
```

### **Pre/Post hooks (automatic)**

NPM automatically runs these:

```
"prestart": "echo Preparing...",
"start": "node server.js",
"poststart": "echo Started",
```

---

# 🟧 4. **Package.json Management**

### **View package config**

```
npm pkg get name
npm pkg get version
```

### **Set values**

```
npm pkg set author="Shubhanjali"
npm pkg set license="MIT"
```

### **Delete key**

```
npm pkg delete scripts.test
```

---

# 🟩 5. **Managing Cache**

```
npm cache verify
npm cache clean --force
```

---

# 🔥 6. **Node Environment Tools (Used Professionally)**

### **nvm – Node Version Manager**

```
nvm ls
nvm install 20
nvm use 18
```

### **Run different Node versions**

```
nvm exec 18 node server.js
```

---

# 🔵 7. **npx Commands (Very Important)**

### **Run a package without installing**

```
npx create-react-app myapp
npx nodemon server.js
```

### **Run local binaries**

```
npx prisma generate
```

---

# 🟪 8. **Testing Tools**

```
npm test
npm run test:watch
npm run test:coverage
```

---

# 🟥 9. **Build Commands (Production)**

```
npm run build
npm run deploy
npm run lint
npm run format
```

---

# 🟫 10. **Professional Full Workflow Example**

```
npm init -y
npm install express mongoose dotenv cors
npm install nodemon --save-dev
npm pkg set scripts.dev="nodemon server.js"
npm pkg set scripts.start="node server.js"
npx eslint .
npm audit fix
npm run dev
```

---


1. Create a folder for the shell app
```bash
mkdir micro-shell
cd micro-shell
```
2. Create the shell app using *create-single-spa* template. The *--layout* specifies the we wanted to use the 'single-spa-layout' package
```bash
npx create-single-spa --layout
```
When the options are displayed input the following,
```bash
? Directory for new project .
? Select type to generate single-spa root config
? Which package manager do you want to use? npm
? Will this project use Typescript? No
? Organization name (can use letters, numbers, dash or underscore) cobssoft
```
3. Install the dependencies
```bash
npm install
```

4. Open src/microfrontend-layout.html, and remove the following line
```html
<application name="@single-spa/welcome"></application>
```

5. Run the project, which will run on port number 9000, you can browse using http://localhost:9000. You don't see anything on the browser as we did not added any micro app yet
```bash
npm start -- --port 9000
```


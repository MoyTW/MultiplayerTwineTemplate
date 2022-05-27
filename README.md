Some notes on setup:
1. Copy websockets.ts / websockets.js into your project
2. Copy websockets.twee into your project
3. Toggle the `DEBUG` value in websockets.ts when you want to build; possibly change the URLs too
4. Change the $imageRoot in StoryInit if you want to use a different image folder
5. Add the following lines to the config.js:
```
/* Disable history tracking to keep file size down */
Config.history.maxStates = 1;
Config.saves.autoload = true;
```

Typescript:
Add a tsconfig.json
Run:
```
npm install --save-dev typescript@latest
npm install --save-dev @types/twine-sugarcube
npm install --save-dev @types/jquery
```

Also, make sure you run redis on 6379
docker run -p 6379:6379 -d redis:5
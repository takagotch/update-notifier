### update-notifier
---
https://github.com/yeoman/update-notifier

```
npm i -g public-ip to update

npm install update-notifier
```

```js
const updateNotifier = require('update-notifier');
const pkg = require('./package.json');
updateNotifier({pkg}).notify();

const updateNotifier = require('update-notifier');
const pkg = require('./package.json');
const notifier = updateNotifier({pkg});
notifier.notify();
console.log(notifier.update);


const notifier = updateNotifier({
  pkg,
  updateCheckInterval: 1000 * 60 * 60 * 24 * 7
});
if(notifier.update){
  console.log(`Update availabel: ${notifier.update.latest}`);
}
```

```
```



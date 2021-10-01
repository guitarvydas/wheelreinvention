from https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Async_await

this code in JS:
```
async function timeTest() {
  const timeoutPromise1 = timeoutPromise(3000);
  const timeoutPromise2 = timeoutPromise(2000);
  const timeoutPromise3 = timeoutPromise(1000);

  await timeoutPromise1;
  await timeoutPromise2;
  await timeoutPromise3;
}
```

can be roughed-in in /bin/bash as:
```
./timeoutPromise 3000 &
pid1=$!
./timeoutPromise 2000 &
pid2=$!
./timeoutPromise 1000 &
pid3=$!

wait $pid1
wait $pid2
wait $pid3
```

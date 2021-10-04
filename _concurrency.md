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

`async function` means `forkable`
`await ...` means fork and wait for child
app runs in thread0, forking a child means to create another thread
`return` from async function returns value when async activity finishes
return on thread0 means function return, return from child thread1 means to return when async activity finishes.
caller must modify how it calls function, e.g. by using await

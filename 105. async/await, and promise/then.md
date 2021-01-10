```
async function f1() {

  let promise = new Promise((resolve, reject) => {
    setTimeout(() => resolve("f1 promise.await"), 5000)
  });

  let result = await promise; 
  console.log(result);
  
  console.log("f1 test")
}

const f2 = () => {
    console.log("f2")
}

const f3 = async() => {
    let promise = new Promise((res, rej) => {
        setTimeout(() => res("f3 promise.then"), 3000)
    });
    promise.then(r => console.log(r))
    console.log("f3 test")
}

const f4 = () => {
    console.log("f4")
}

f1();
f2();
f3();
f4();

// 0 sec
f2
f3 test
f4

// 3 sec
f3 promise.then

// 5 sec
f1 promise.await
f1 test

```

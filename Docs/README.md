# Typechain

```ts
const sayHi = (name: string, age: number, gender: string): string => {
  console.log(`Hello ${name}, You are ${age}, You are a ${gender}`);
};

sayHi("seulhee", 22, "female");
```

void는 빈공간 같은 건데 sayHi의 function들이 어떤 유형의 값을 돌려주는지를 나타내기 위해 존재한다.

sayHi function은 string으로 값을 반환한다.

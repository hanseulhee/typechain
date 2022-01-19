# Typechain

```ts
const sayHi = (name: string, age: number, gender: string): string => {
  console.log(`Hello ${name}, You are ${age}, You are a ${gender}`);
};

sayHi("seulhee", 22, "female");
```

void는 빈공간 같은 건데 sayHi의 function들이 어떤 유형의 값을 돌려주는지를 나타내기 위해 존재한다.

sayHi function은 string으로 값을 반환한다.


### Interfaces

```ts
interface Human {
  name: string;
  age: number;
  gender: string;
}

const person = {
  name: "seulhee",
  age: 22,
  gender: "female",
};

const sayHi = (person: Human): string => {
  return `Hello ${person.name}, You are ${person.age}, You are a ${person.gender}`;
};

console.log(sayHi(person));

export {};
```

인터페이스는 상호 간에 정의한 약속 혹은 규칙을 의미한다. 일반적으로 타입 체크를 위해 사용되며 변수, 함수, 클래스에 사용할 수 있다.


### constructor

생성자는 메소드인데 클래스가 시작할 때마다 호출된다. (클래스로부터 객체를 만들 때)
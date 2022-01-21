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

### Class

```ts
class Human {
  public name: string;
  public age: number;
  public gender: string;
  constructor(name: string, age: number, gender: string) {
    this.name = name;
    this.age = age;
    this.gender = gender;
  }
}

const lynn = new Human("Lynn", 18, "female");
const sayHi = (person: Human): string => {
  return `Hello ${person.name}, You are ${person.age}, You are a ${person.gender}`;
};

console.log(sayHi(lynn));
```

클래스 몸체에 클래스 property를 선언할 수 없고 반드시 생성자 내부에서 클래스 property를 선언한다.

### Constructor

생성자(Constructor)는 메소드인데 클래스가 시작할 때마다 호출된다. (클래스로부터 객체를 만들 때)


### Hash

해쉬는 모든 속성을 수학적으로 이상한 하나의 문자열로 결합한 것이다.

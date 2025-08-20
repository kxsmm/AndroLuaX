```ts
class Person {
   private _name: string;
   private _age: number;
   constructor(name: string, age: number) {
    this._name = name;
    this._age = age;
   }
   get name(): string {
    return this._name;
   }
   set name(name: string) {
    this._name = name;
   }
   get age(): number {
    return this._age;
   }
   set age(age: number) {
    this._age = age;
   }
}

const person = new Person("张三", 25);
console.log(person.name);
person.name = "李四";
```



<details><summary><b>Output</b></summary>

```ts
"use strict";
class Person {
    constructor(name, age) {
        this._name = name;
        this._age = age;
    }
    get name() {
        return this._name;
    }
    set name(name) {
        this._name = name;
    }
    get age() {
        return this._age;
    }
    set age(age) {
        this._age = age;
    }
}
const person = new Person("张三", 25);
console.log(person.name);
person.name = "李四";

```


</details>


<details><summary><b>Compiler Options</b></summary>

```json
{
  "compilerOptions": {
    "strict": true,
    "noImplicitAny": true,
    "strictNullChecks": true,
    "strictFunctionTypes": true,
    "strictPropertyInitialization": true,
    "strictBindCallApply": true,
    "noImplicitThis": true,
    "noImplicitReturns": true,
    "alwaysStrict": true,
    "esModuleInterop": true,
    "declaration": true,
    "target": "ES2017",
    "jsx": "react",
    "module": "ESNext",
    "moduleResolution": "node"
  }
}
```


</details>

**Playground Link:** [Provided](https://www.typescriptlang.org/zh/play/?#code/MYGwhgzhAEAKCmAnCB7AdtA3gKGngDogJYBuYALvNAPppgC28AXNBOcWgOYDcuBxZSjTCdm0NAFd6AIyS880YOjaIJwcikQAKOoxYqiXADTQRYyTKQBKLHzzkAFkQgA6WgyoBecR-kLHzm5m0N5mftAAvnai5D6MWlb67IactgrQiPDkEogYAa7ujOFRChBZcfA6HkkcnDY46fluul4VxdHlZgksFrKIaQqZ2bnQTdRhdiV4ZbFdZj1SffV2o04FwaGi7VHYSmhs0PhIqBjeaPAA7nDH6FoARIAE+oCQcncmAEwArFa8e6gg8C4QChOFojsh0C4Wt9sGCTpCPCFoHdAHLmgG21O7cIA)
      
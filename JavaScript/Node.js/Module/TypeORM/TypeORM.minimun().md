- [[TypeORM]]의 minimun() [[메서드(Method)]]는 해당되는 필드([[열(Column)]])의 값의 최소를 구한다.
- 반대로 [[TypeORM.maximun()]]도 있다.


## 예시

- 아래 코드와 같이 사용하여, 첫번째 [[매개변수(parameter)]]는 최솟값을 찾아 저장할 필드([[열(Column)]])명인 age를 명시하고 firstName 필드([[열(Column)]])이 "Timber"인 필드([[열(Column)]])들의 최소를 구한다.

```ts
const sum = await repository.minimun(
	"age",
	{ firstName: "Timber" }
); 
```

​
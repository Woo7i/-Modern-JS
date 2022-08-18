# <img src="https://velog.velcdn.com/images%2Fsky%2Fpost%2F8910fe85-412e-44b1-b608-8fd817def338%2F1200px-Unofficial_JavaScript_logo_2.svg.png" width="15%" height="90%"></img>. Modern JavaScript / Study

## # 변수(variable)
### - 하나의 값을 저장하기 위해 확보한 '메모리 공간' 자체 또는 그 메모리 공간을 **식별하기 위해** 붙인 '이름'을 말한다 <br>= 값의 위치를 가리키는 상직적인 이름 

```js
var result = 10 + 20;
console.log(result);

30
```
메모리 공간에 저장된 값을 식별할 수 있는 고유한 이름(ex. result)을 변수명(변수이름)이라한다. 그리고 변수에 저장된 값(ex.30)을 변수 값이라 한다.
> <sapn style ="color:#808080">변수에 값을 저장하는 것을 할당(assignment 대입, 저장)이라 하고, 변수에 저장된 값을 읽어 들이는 것을 참조(reference)라 한다.</span>


- 식별자(identifier) : 변수명을 부르는 다른 말. <p>- 어떤 값을 구별해서 식별할 수 있는 고유한 이름.</p>
**식별자는 값이 저장되어 있는 메모리 주소와 매핑(mapping) 관계를 맺으며 이 매핑 정보도 메모리에 저장되어야 한다. <br>"식별자는 값이 아니라 메모리 주소를 기억하고 있다."** 

- 변수 선언 <p>- 변수를 사용하려면 반드시 선언이 필요하다. 변수를 선언 할 때는 "var, let, const" 키워드를 사용한다.</p>
```js
var score; // 변수 선언 
```
> <sapn style ="color:#808080">var 이외의 키워드로 선언한 변수들은 undfined로 암묵적인 초기화가 자동 수행된다. 즉 어떠한 값을 할당하지 않아도 'undfined'라는 값을 갖고있다.</span>

<details>
    <summary>ReferenceError</summary>
ReferenceError에러는 등록된 식별자를 찾을 수 없을 때 생성되는 에러이다.
</details>
<br>
 
- 변수 선언의 실행시점과 변수 호이스팅
```js
console.log(score);
var score;
```
> <div style ="color:#808080">변수 선언이 소스코드가 한줄 씩 순차적으로 실행되는 시점, 즉 런타임이 아니라 그 이상 단계에서 먼저 실행되기 때문이며 <br>변수 선언문이 코드의 선두로 끌어 올려진 것 처럼 동작하는 자바스크립트 고유의 특징을 변수 호이스팅(hoisting)이라고 한다.</div>
<br>

- 값의 할당
# Array.reduce 

## 오늘은 Array.reduce 메소드의 개념을 알게되었다.  
</br>

> ###  콜백함수를 이용해서 Array.reduce 를 작성해보자. 



```js 
const array1 = [1, 2, 3, 4]; //배열


// 0 + 1 + 2 + 3 + 4
const initialValue = 0; // reduce 메소드를 써줄라면 초기값이 존재해야함으로 초기값 그래서 생성을 해줬어 
const sumWithInitial = array1.reduce( 
  (accumulator, currentValue) => accumulator + currentValue, //acc랑 cur이랑 더 한다는 뜻 
  initialValue // 이건 아까 초기(0)값을 불러왔잖아 이걸 기준으로 위에있는 애들이 계산을해줘 근데 const initialValue = 10 경우에는 누산기 값이 10이 기준으로 되어서 초기값도 10이 되버려 이걸 기준으로 누산기 값이 바껴서 계산이 되버려    
); 

console.log(sumWithInitial);
// Expected output: 10
```


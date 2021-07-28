# JavaScript 배열 내장함수

## forEach

배열 안에 있는 모든 원소에 대하여 처리하고 싶을 때 사용

`const world_language = ['한국어' , '일본어' , '중국어'];

world_language.forEach(language => {

console.log(language);

});`

## map

배열 안의 각 원소를 변환 할 때 사용

`const array = [1, 2, 3, 4, 5]

 const example = [];

 for(let i = 0; i < array.length; i++) {
 
 example.push(array[i] + 2);

}`

console.log(example);`

## indexOf

원하는 항목의 원소가 어디인지 알려주는 함수

`const world_language = ['한국어', '일본어', '중국어'];
 
 const index = world_language.indexOf('한국어');
 
 console.log(index);`

## shift, pop

shift와 pop은 굉장히 유사합니다.
shift가 첫번째 원소를 추출하면 pop은 반대로 가장 끝에 있는 원소를 추출합니다.

`const numbers = [10, 20, 30, 40];
 
 const value = numbers.shift();
 
 console.log(value);
 
 console.log(numbers);`

shift의 결과는

 `10

  [20, 30, 40]`

pop의 결과는

`40

 [10, 20, 30]`

반대로 맨 앞에 추가를 하고 싶으면 shift 앞에 un을 붙여 unshift를 사용한다.



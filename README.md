# project_colorflipper

---

![color_Flipper](https://user-images.githubusercontent.com/100138165/177002064-d608abbd-ad70-4a5a-9252-692eaa6d69a9.gif)

### 페이지만 보면 그냥 클릭 할때마다 색깔 바뀌는 별거 아닌거(?) 같은 느낌이 들지만 해보니 쉽지 않았다
### 개발자분들 정말 대단하다는 생각이 든다
### 우선 2개의 html 파일과 2개의 js, 마지막 css 파일 이렇게 구성이 되며, html은 거의 복붙인거 같다
### 


```
const colors = ["green", "red", "rgba(133,122,200)", "#f15025"];   => 4가지 색깔을 배열로 지정.

const btn = document.getElementById("btn");       
const color = document.querySelector(".color");

btn.addEventListener('click', function(){              
  // get random number between 0 - 3 colors[3] //
  const randomNumber = getRandomNumber();    
  
  document.body.style.backgroundColor = colors[randomNumber];
  color.textContent = colors[randomNumber];
});

function getRandomNumber(){
  return Math.floor(Math.random() * colors.length);    => 함수명 getRandomNumber에 colors 배열안의 각 값을 랜덤 및 정수로 리턴.
}
```

쉽지 않지만 화이팅!

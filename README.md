#내용 정리

## this 와 self 의 차이  
  
  ### this
  - 컨텍스트(객체) 자신을 가리키는 참조변수로써, 객체 자신에 대한 참조 값을 가지고 있다는 말이다.
  - 주로 매개변수와 객체 자신이 가지고 있는 변수의 이름이 같을 경우 이를 구분하기 위해 사용된다.
  
  ### self
  - 통상적인 변수 이름이지만, 바깥쪽의 this를 참조하기 위해 사용된다.  
  - 또한 클로저와 결합하여 this의 값을 주고 받는 용도로 사용 또한 가능하다.

---

createElement
인수로 지정한 태그명에 해당하는 태그 요소를 생성하여 반환.
단, 생성 시의 요소는 모두 독립적인 개별 요소가 반환됨에 따라 재활용이 되지 않음에 주의하라.  

appendChild
지정한 부모 요소에 인수로 전달한 부모 요소의 마지막 자식 요소로 추가 후 추가된 자식 요소의 참조를 반환

Ex) for (let i = 0; i < imgAr.length; i++) {
    slide_list.appendChild(document.createElement('li'))
    .style.background = `url(${imgAr[i]}) center / 400px 500px no-repeat`
     }

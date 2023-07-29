---
layout: post
title: JavaScript. [Array] 배열 요소 추가, 제거
date: 2023-07-29 15:33:00 +0900
categories: [공부, Javascript]
tags: [JavaScript]
pin: true
---

**[JavaScript] 배열(array) 요소 추가, 제거**

> [배열 요소 추가하기]
\
> **push(), unshift(), splice()**


> [배열 요소 제거하기]
\
> **pop(), shift(), splice()**


<br>
<br>

## **1. 배열에 요소 추가하기**
### **push(), unshfit(), splice()**
---

* array.**push()** : 배열의 끝에 요소를 추가
* array.**unshift()** : 배열의 앞에 요소를 추가
* array.**splice(인덱스, 개수, 요소..)** : 원하는 위치에 요소를 추가 (인덱스 번째 위치에 개수만큼 요소1, 요소2,.. 추가)

```javascript
  var array = ['2', '3'];
  
  array.push('4');  // array = ['2', '3', '4'];
  array.unshift('1'); // array = ['1', '2', '3', '4'];
  array.splice(2, 2, '12', '34'); // array = ['1', '2', '12', '34', '3', '4'];  
  // 2번째 위치에 12, 34 숫자 2개를 추가.
```


<br>

<br>

## **2. 배열에 요소 제거하기**
### **pop(), shift(), splice(), delete**
---

* array.**pop()** : 배열의 마지막 요소를 제거
* array.**shift()** : 배열의 첫 번째 요소를 제거
* array.**splice()** : 원하는 위치의 요소를 제거 (인덱스 사용)
* **delete** array[i] : i번째 인덱스의 값을 제거. **단, 값만 삭제될 뿐 요소는 그대로 존재한다.**

```javascript
  var array = ['1', '2', '3', '4', '5'];
  
  array.pop('4');  // array = ['1', '2', '3', '4'];
  array.shift('1'); // array = ['2', '3', '4'];
  array.splice(2, 1); // array = ['2', '3'];  
  // 2번째 위치에서 1개를 제거
  delete array[0]; // array = ['3'];
  // array[0]의 요소를 제거
```

<br>

### **splice()**
* 인덱스(index)를 이용하여 특정 요소를 추가하거나 제거하는 방법
* splice는 **접합**이라는 의미로 아래 그림과 같이 특정 요소를 제거한 후 접합을 한다.
* array.**splice(i인덱스, n개수, 요소1, 요소2..)** : i번째 인덱스에 n개수인 요소1, 요소2를 추가한다.
* array.**splice(i인덱스, n개수)** : i번째 인덱스로부터 n개수만큼 제거한다.

![](blog/array_splice.png){: .normal}

<br>

<span style='font-size: 0.8rem; color: #999;'>
[사진 출처 : 혼공, "자바스크립트 배열 생성 요소 추가와 제거"]( https://hongong.hanbit.co.kr/javascript-%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EB%B0%B0%EC%97%B4-%EC%83%9D%EC%84%B1-%EC%9A%94%EC%86%8C-%EC%B6%94%EA%B0%80%EC%99%80-%EC%A0%9C%EA%B1%B0/)
</span>

<br>
<br>


## 배열 요소의 개수
---
* array.**length()** : 배열 요소의 개수


<br>


<span style='font-size: 0.95rem; color: #999;'>
[+] <br>
Java의 배열과는 조금 차이가 있다.<br>
Java에서 배열의 추가는 add로 이루어진다.
</span> 





# TIL : 2주차 한것들

#### 2주차 과제

#### 구구단 출력기
<pre>
<code>
 void main() {
  for (int i = 2; i < 10; i++) {
    for (int j = 1; j < 10; j++) {
      print('$i x $j = ${i * j}');
    }
    print(''); // 각 단 구별
  }
}   
</code>
</pre>

<hr></hr>

#### 정사각형 길이 입력 후 정사각형 출력

<pre>
<code>
void main() {
  var n = 10;
  var result = '';
  for (var y = 0; y < n; y++) {
    for (var x = 0; x < n; x++) {
      var c = f1(x,y,n) || f2(x,y,n);
      if(c){
      result += '=';
      }
       else {
    result += '\n';
    }
  }
  print(result);
}
bool f1(int x, int y, int size){
  return 
    x == 0 
    || y == 0 
    || x == size - 1
    || y == size - 1;
}

bool f2(int x, int y, int size){
  return 
    x == y; 
    || y == 0 
    || x == size - 1
    || y == size - 1;
}
}
</code>
</pre>

<hr></hr>

#### 년/월/일을 입력하면 요일을 출력

<pre>
<code>

void main() {
  var nowtime = DateTime.now();
  var weekday = nowtime.weekday;

  print (weekdays(weekday));
}

 String weekdays(int weekdaynum) {
  switch (weekdaynum) {
    case 1:
      return '월요일';

    case 2:
      return '화요일';

    case 3:
      return '수요일';

    case 4:
      return '목요일';

    case 5:
      return '금요일';

    case 6:
      return '토요일';

    case 7:
      return '일요일';
      
    default:
      return '잘못된 요일 번호';
  }
}

 <hr></hr>
 
</code>
</pre>
Link:[다트][DateTime 사용법][DateTime 사용법2]
[다트]:https://dartpad.dev/
[DateTime 사용법]:https://api.dart.dev/dart-core/DateTime/weekday.html
[DateTime 사용법2]:https://velog.io/@gunwng123/%ED%8A%B9%EC%A0%95-%EB%82%A0%EC%A7%9C%EC%9D%98-%EC%A3%BC-%EC%8B%9C%EC%9E%91%EC%9D%BC%EA%B3%BC-%EB%A7%88%EC%A7%80%EB%A7%89%EC%9D%BC-%EA%B5%AC%ED%95%98%EA%B8%B0

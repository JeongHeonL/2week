# 2week

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
  var input = '2025-03-11';
  var output = DateTime.parse(input);
  print(output.day);
}
 
</code>
</pre>


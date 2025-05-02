>인프런-10주완성 C++ 코딩테스트 | 알고리즘 코딩테스트 참조
>이 내용은 강의 내용을 바탕으로 제 방식대로 정리한 것입니다. 오류가 있을 수 있습니다.

#재귀함수(recursion)의 기본개념과 예제
==================================

## Recursion
재귀함수는 자기 자신을 호출하는 메소드이다.

### 1-1 Factorial(n!)
* 팩토리얼은 n이 자연수일 때, 1부터 n까지의 모든 자연수의 곱을 의미한다.
* 0!, 1! = 1
```
int factorial(int n){
    if(n==0||n==1){
        return 1;
    }
    return n*factorial(n-1);
}
```

### 1-2 Factorial을 반복문으로 표현하기
```
int factorial(int n){
    for(int i=n; i>0; i--){
        result *= i;
    }
    reutn result;
}
```

### 2 Fibonacci
* 피보나치 수는 첫째와 둘째 항이 1이고 그 뒤의 모든 항은 바로 앞 두항의 합인 수열이다.
* F0 = 0, F1 = 1, Fn = Fn-1 + Fn-2
```
int fibonacci(int n){
    if(n==0||n==1){ 
        return n;
    }
    return fibonacci(n-1) + fibonacci(n-2);
}
```






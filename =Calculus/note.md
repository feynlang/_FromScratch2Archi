# Chapter 1. Functions and Model
### Outline

### Flow Diagram

<!-- *** -->
## Main Concepts
### 1.1 function(represent,mathematical model)
#### represent a function(4ways)
1. verbally
2. numerically
3. visually
4. algebraicially

### 1.4 exponential function
#### Sec 3.1(a) Exponential Functions - (1/2)
1. $f=a^x$일때 $x=n,0,-n,\frac{p}{q}$에 따라 어떻게 정의되는지(**a는 양수**)\
-> 유리수일때 q의 값이 odd/even이냐에 따라 양수x 조건이 작용되는 포인트\
-> 실수로 확장하는 방법(유리수x의 샌드위치 극한)\
=> 그래프 개형으로 확인($a\gt1$, $0\lt a\lt 1$, $a=1$),(지수함수$2^x$ vs 다항함수$x^2$)
2. 지수함수 성질(연속함수o,지수법칙o, 양/음의 무한대 극한값)
#### Sec 3.1(b) Exponential Functions - (2/2)
- 오일러수 $e:=\lim_{x\to 0}(1+x)^{\frac{1}{x}}$ (exists, 무리수이자 초월수)\
-> natural exponential function (f(x)=e^x)\
=> guess: $f'(0)=1$ {$e$의 정의에 따라 $(1+h)^{1/h}~=e \Rightarrow e^h-1~=h$ for small $h$} 
or {$e^x$의 테일러 전개를 활용}

### 1.5 inverse functions and Logarithm
#### Sec 3.2(a) Inverse Functions and Logarithms - (1/3)
1. one to one function (injective,단사함수)\
$\Leftrightarrow$ 정의역의 원소$x$가 다르면 함숫값$f(x)$도 다름 (역도 성립, 증명의 key)
2. inverse function: one-to-one function($f$: domain A, **range B**)$\to$($f^{-1}$: **domain B**, range A)\
=> cancellation equation: 모든 B(A)의 원소 x에 대해 $f\circ f^{-1}$ / $f^{-1}\circ f$ $=x$\
=> 그래프 개형 상, y=x(line)에 대칭
    
#### Sec 3.2(b) Inverse Functions and Logarithms - (2/3)
1. $f$가 one-to-one함수 & 연속 $\Rightarrow$ $f^{-1}$도 연속\
*(증명은 <해석학>에서 다룸)*
2. $f$가 one-to-one함수이고 미분가능하며 $f'(f^{-1}(a))\ne 0$이면 역함수의 도함수는 $(f^{-1})'(a)=\frac{1}{f'(f^{-1}(a))}$

- [증명]\
$\lim\limits_{x\to a}\frac{f^{-1}(x)-f^{-1}(a)}{x-a}\\
=\lim\limits_{y\to b}\frac{y-b}{f(y)-f(b)}
=\frac{1}{\lim\limits_{y\to b}\frac{f(y)-f(b)}{y-b}}
=\frac{1}{f'(b)}
=\frac{1}{f'(f^{-1}(a))}$
- [증명에 필요한 것]\
(1) $f^{-1}$의 극한값이 존재하는지, 즉 연속인지 $\to$ 위 1번 정리 이용\
(2) $f^{-1}(a)=b, f^{-1}(x)=y\\ \Rightarrow a=f(b), x=f(y)$
3. Leibniz notation: $\frac{dy}{dx}=\frac{1}{\frac{dx}{dy}}$\
($\because y=f^{-1}(x)\Rightarrow x=f(y)$이기에\
역함수 미분 형태인 $(f^{-1})'(x)=\frac{1}{f'(f^{-1}(x))}$ 에서 좌변은 y를 x로 미분한 것, 우변은 x를 y(=$f^{-1}(x)$)로 미분한 것의 역수가 됨) 
4. implicit differentation: $f^{-1}$가 미분가능하다면, 음함수 미분법을 사용하여 유도 가능\
$f(y)=x$를 x에 대해 미분 -> $f'(y)\frac{dy}{dx}=1\Rightarrow \frac{dy}{dx}=\frac{1}{f'(y)}=\frac{1}{f'(f^{-1}(x))}$

#### Sec 3.2(c) Inverse Functions and Logarithms - (3/3)
1. [정의] $a>0$, $a\ne 1$ 이면, $f(x)=a^x$는 one-to-on function
$\Rightarrow$ 역함수 $f^{-1}=log_ax$ (logarithmic function with base $a$) 존재
- $f(f^{-1}(x))=f^{-1}(f(x))=x$, 따라서 $a^{log_ax}=x$ for all $x\in\R$, $log_a(a^x)=x$ for all $x>0$임.
- log함수 성질: if $x,y>0$, then
    - $log_a(xy)=log_ax+log_ay$
    - $log_a(\frac{x}{y})=log_ax-log_ay$
    - $log_a(x^r)=rlog_ax$ for any $r\in\R$
    - 극한: ($a>1$), $x\to\infty$일때 $\infty$, $x\to0^+$일때 $-\infty$
2. natural logarithms(base $e$): $\ln x:=log_ex$\
=> $\ln(e^x)=x$ for all $x\in \R$,\
=> $e^{\ln x}=x$ for all $x>0$
- 밑 변환 공식(change of base formula): 양수a($\ne 1$)이면 $\log_ax=\frac{\ln x}{\ln a}$ $\to \log_ax=\frac{1}{\log_xa}$ for $x\ne 1$
- [증명]: 역함수인 지수함수 합성 후 밑이 e인 $\ln$을 양변에 취하여 유도\
$y=\log_ax \to a^y=log_ax \to \ln(a^y)=\ln(x) \to y\ln a=\ln x$
<!-- *** -->
## Application
### example review
- 도메인과 range 표현시 주의
### confusing point

### extension point
- 2^x=x^2을 대수적으로 푸는 방법?
## Reference(bookmark)

<!-- ------------------------------ -->

# Chapter 2. Limits and Derivatives
### Outline

### Flow Diagram

<!-- *** -->
## Main Concepts
### Tangent(Velocity Problem)
#### Sec .(a) 

### Limit of a Function
### Calculating Limits (limit laws)
### Continuity
### Limits at Infinity
### Derivative & Rates of change
### Derivative as a Function

<!-- *** -->
## Application
### example(1~2)

### confusing point(~3)

### implement point(1~)
(extension)
### Reference(bookmark)

<!-- ------------------------------ -->

# Chapter 3. Limits and Derivatives
### Outline

### Flow Diagram

<!-- *** -->
## Main Concepts
### Derivatives 1(polynominals, exponential)
### Product & Quotient Rules
### Chain Rule
### Implicit Differentiation

### Derivatives 2(Logarithmic, Inverse Trigonometric)
#### Sec 3.3(a) Derivatives of Logarithmic and Exponential - (1/2)
1. 로그함수의 미분: $f(x)=\log_ax$, $f'(x)=\frac{1}{x}\log_ae=\frac{1}{x\ln a}$ and $\frac{d}{dx}(\ln x)=\frac{1}{x}$\
!!!!!!!!(증명은 전자메모보드에 하고 nextstep으루~)
-> chain rule
2. $\ln |x|$는 미분가능(!)함
#### Sec 3.3(b) Derivatives of Logarithmic and Exponential - (2/2)

#### Sec 3.5(a) Inverse Trigonometric Functions - (1/2)
#### Sec 3.5(b) Inverse Trigonometric Functions - (1/2)
### Exponential Growth & Decay
#### Sec 3.4(a) Exponential Growth and Decay - (1/2)
#### Sec 3.4(b) Exponential Growth and Decay - (2/2)
### Related Rates
### Linear Approximations
### Hyperbolic Functions
#### Sec 3.6(a) Hyperbolic Functions - (1/2)
#### Sec 3.6(b) Hyperbolic Functions - (2/2)

<!-- *** -->
## Application
### example(1~2)

### confusing point(~3)

### implement point(1~)
(extension)
### Reference(bookmark)

<!-- ------------------------------ -->

# Chapter 4. Applications Of Differentiation
### Outline

### Flow Diagram

<!-- *** -->
## Main Concepts
### Maximum/Minimum Values
### The Mean Value Theorem
### Derivatives $\to$ Shape of Graph
### Indeterminate Forms (L'Hospital's Rule)
#### Sec 3.7(a) Indeterminate Forms and L'Hospital's Rule - (1/2) 
#### Sec 3.7(b) Indeterminate Forms and L'Hospital's Rule - (2/2) 
### Curve sketching
### Graphing(calculus/tech)
### Optimization problems
### Newton's Method
### Antiderivatives

<!-- *** -->
## Application
### example(1~2)

### confusing point(~3)

### implement point(1~)
(extension)
### Reference(bookmark)
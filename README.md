# heart 그리기

```python
import turtle as t

t.bgcolor('#FFDCDC')
t.color('#E478E4')
t.shape('turtle')

t.begin_fill()
t.left(60)
t.forward(200)
t.circle(50, 200)
t.left(200)
t.circle(50, 200)
t.forward(200)
t.end_fill()

t.hideturtle()
t.mainloop()
```

# 하트를 어떻게 만들까? 🤔

> 다음과 같이 만들면 되지않을까 생각했습니다.
- 반원 2개를 그린다.
- 역삼각형 하나를 그린다
- 합친다

<br><br>

> 근데 각도 맞추는 것과 거리를 가늠해야하는 것이 어려웠다. 😫

그래서 단순하게 circle(반지름, 각도) 와 forward() (이동할 거리) 등을 통일했다.
그러니까 얼추 모양이 예상하던대로 나왔다.

<br><br>

> 근데 다 작성하고 보니 끝부분에 예상하지 못한 삼각형이 나왔다..💦

아마 각도와 길이가 제대로 맞지 않아서 끝에 나온것 같은데..
처름에는 hideturtle()를 쓰지않아서 터틀이 남아있는걸로 오해했다.

그래서 코드를 추가했음에도 불구하고 삼각형 모양이 없어지지않는 것을 보고 길이가 잘못되서 그런걸 깨달았다.

그건 나중에...!

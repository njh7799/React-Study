# 리액트 피아노



![결과물](https://user-images.githubusercontent.com/40619551/66251251-568b0d00-e789-11e9-9f0a-aa7d34dfdf57.png)



## 디렉토리 구조
```
├─components
│  ├─Piano
│  │  └─Scale
│  │      └─Keyboard
│  └─PianoControl
└─containers
    └─PianoBuilder
```

### Keyboard

- 한 건반을 의미한다.
- 흰 건반과 검은 건반은 class를 이용하여 구분한다.
- 음에 대한 정보를 가지고 있어야 한다.
- 클릭하면 아래로 내려왔다가 다시 올라간다.

### Scale

- C 부터 B 까지 한 옥타브 건반을 모은 것을 의미한다.
- 몇 옥타브인지에 대한 데이터를 가지고 있어야 한다.
- 위 데이터를 기반으로 한 옥타브의 피아노를 구성한다.

### Piano

- Scale 컴포넌트를 이어 붙인 것이다.
- 시작 옥타브에 대한 정보를 가지고 있어야 한다.

### PianoControl

- 시작 옥타브를 높이거나 낮출 수 있다.

### PianoBuilder

- 피아노의 시작 옥타브에 대한 정보를 state에 저장한다.
# node-chat
### Node.js 기반의 실시간 그룹채팅 강좌
- 진행자: 이근혁(lghlove0509@naver.com)
- [블로그 본문 보기](http://codevkr.tistory.com/61)

# Chapter 4 - Socket.io 기초

```javascript
/* 접속이 되면 1번 실행되는 이벤트: connection */
io.sockets.on('connection', function(socket) {
  // sockets는 모든 소켓                 |
  // 콜백으로 전달되는 소켓은 접속된 소켓 <┘

  socket.on('receive', function(data) {
    // on은 이벤트 수신, 'receive'가 수신할 이벤트 명
    // 콜백으로 전달되는 변수에는 상대가 전송한 데이터가 담겨져 옴
    // 상대가 데이터를 전달 할 수도, 안 할 수도 있음
  })

  socket.on('test', function() {
    // test라는 이벤트를 수신하면
    // 접속되어있는 모든 소켓에게 receive 이벤트 전송 + 데이터
    //                                    ┌------------┘ 
    //                                    V
    io.sockets.emit('receive', {data : 'temp'})
  })

  socket.on('disconnect', function() {
    // 접속되어있던 소켓의 연결이 끊기면 호출 됨
  })
})
```


# 강좌
- [전체강좌 보기](https://github.com/leegeunhyeok/node-chat/blob/master/README.md)
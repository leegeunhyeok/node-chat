# node-chat
### Node.js 기반의 실시간 그룹채팅 강좌
- 진행자: 이근혁(lghlove0509@naver.com)
- [블로그 본문 보기](http://codevkr.tistory.com/62)

# Chapter 5 - 채팅 기능 구현

```javascript
/* 접속된 모든 소켓에게 데이터 전달 */
io.sockets.emit('이벤트명', 데이터)

/* 나를 제외한 모든 소켓에게 데이터 전달*/
socket.broadcast.emit('이벤트명', 데이터)
```


# 강좌
- [전체강좌 보기](https://github.com/leegeunhyeok/node-chat/blob/master/README.md)
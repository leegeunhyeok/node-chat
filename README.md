# node-chat
### Node.js 기반의 실시간 그룹채팅 강좌
- 진행자: 이근혁(lghlove0509@naver.com)
- [블로그 본문 보기](http://codevkr.tistory.com/60)

# Chapter 3 - 정적 파일 제공

```javascript
/* 서버 image 폴더의 파일들을 제공(액세스 가능) */
/* 클라이언트는 http://서버주소/test 로 액세스 */
app.use('/test', express.static('./image/'))
```


# 강좌
- [전체강좌 보기](https://github.com/leegeunhyeok/node-chat/blob/master/README.md)
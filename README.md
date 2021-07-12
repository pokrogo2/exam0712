# exam0712

1.pom.xml에 lombok추가
```
  <dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.18.12</version>
    <scope>provided</scope>
  </dependency>
```
2.insert.jsp에 jquery추가
```
<script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
	
```
3.beanConfiguration에 어노테이션 @Configuration 추가

4.board.xml에 mapper namespace 수정
```
<mapper namespace="com.koreait.test1.dao.BoardDAO">
```
5.board.xml에 selectBoardCount select문 추가
```
<select id="selectBoardCount" resultType="int">
		SELECT COUNT(BIDX)
		FROM BOARD
		
	</select>
```
6.view.jsp 에 <input type="hidden" name="bIdx" value="${boardDTO.bIdx }">추가

7.BoardController에 insert @PostMapping으로 변경

### 기능 구현 사항

1. 우선 매개변수에 존재하는 모든 사람을 한 배열에 담기 위해 allPeople 배열을 선언하고 friends와 visitors 매개변수에 존재하는 모든 사람을 for문을 이용하여 담는다.
2. allPeople 배열의 중복을 제거한다.
3. friendsList 객체를 만들어 allPeople 배열에 속한 사람들의 친구목록을 검색이 가능하도록 value에 담는다.
4. 이제 사람 별로 점수를 부여하기 위해 score 객체를 선언하고 모든 점수는 0으로 초기화한다.
5. user의 친구목록을 따로 배열로 선언하여 user의 친구들을 담는다.
6. 친구의 친구는 내가 함께 아는 친구가 존재하는 것이므로 friendsList의 친구목록에서 내 친구의 친구들은 모두 score 객체에 10점씩 부여한다.
7. visitors에 방문기록을 참고하여 방문자에게 1점씩 부여한다.
8. 현재 score 객체에는 user도 포함되어 있는데, 친구 추천에 본인이 나올 수는 없으므로 user를 삭제한다.
9. 또한 score 객체에 현재 이미 친구인 사람도 포함되어 있으므로 usersFriends를 참고하여 이미 친구인 사람도 삭제한다.
10. 이제 점수대로 정렬하여 answer 배열에 담는다.
11. answer를 리턴한다.
# 🔑 How to design key? (Dynamo DB)

### 1. Use case from business
![image](https://user-images.githubusercontent.com/73240332/233829311-18c2f4f1-4536-4431-8807-60f250b96aec.png)
![image](https://user-images.githubusercontent.com/73240332/233580136-f36380a3-35a8-4bdd-91b6-e4a9a3bfe573.png)


### 2. Draw Entity Relation Diagram (ERD)
![image](https://user-images.githubusercontent.com/73240332/233580477-776783ff-0e4f-459f-8de9-fc402c6a4ae7.png)


### 3. Write down access patterns
1. 학교급, 학년, 과목 코드 List를 조회합니다.
2. 학교급, 학년, 과목 코드로 단원 목록을 조회합니다.
3. 학교급, 단원 코드로 각 단원에 해당하는 문항 수를 조회합니다.
4. 난이도 별로 입력한 문항 수를 선택된 문제형태와 과목과 단원에 맞게 조회합니다.
5. 선택한 문항 ID에 해당하는 문항 분류체계와 문항 메타데이터, 문항 HTML을 조회하여 시험지를 생성합니다.
6. 시험지에 포함된 문항ID와 해당하는 분류체계, 메타데이터, HTML을 조회합니다.
7. 선택한 문항 ID에 해당하는 문항 분류체계와 문항 메타데이터, 문항 HTML을 조회하여 셋팅지를 생성합니다.



### 4. Start thinking key design

- 검색 키워드 : dynamodb hierarchical data sort key 어렵당

# UMC-4th-Week-ORM-Mission
- ORM을 활용한 데이터 모델링 및 스키마 동기화

<br>

## 과정
1. 엔티티 클래스 작성 : User, Review, Store, ... 등 도메인 12개를 자바 클래스로 작성 <br>
2. 엔티티 매핑 : @Entity, @Table, @Column 등의 JPA 어노테이션을 사용하여 자바 필드가 데이터베이스의 칼럼과 1:1로 매핑되도록 정의 <br>
3. 연관 관계 설정 : @ManyToOne, @OneToMany 등을 통해 엔티티 간의 복잡한 연관 관계를 SQL 없이 자바 코드로 정의 <br>
4. 스키마 자동 생성 : application.yml에 설정된 ddl-auto: update 옵션을 통해,  <br>
Spring Boot 실행 시 JPA(Hibernate)가 자바 코드를 읽어 데이터베이스에 필요한 SQL 쿼리(CREATE TABLE, ALTER TABLE)를 자동으로 생성 <br>
5. 데이터베이스 반영 확인 : 새로운 데이터베이스(database_week4 등)에서 실행을 통해 12개의 테이블이 실제 MySQL DB에 성공적으로 만들어졌음을 확인 <br>

<br>

## ERD 사진
<img width="556" height="460" alt="스크린샷 2025-10-15 오후 11 27 45" src="https://github.com/user-attachments/assets/7e24f6f0-3cc8-4e90-aaeb-49e348023dfd" /> <br>

<br>

## 파일 .java + .yml(id, password 임의 지정) 첨부
- Food, Location, Mission, Reply, Review, ReviewPhoto, Store, Term, User, UserFood, UserMission, UserTerm
- applcation.yml

<br>

## 빌드 후 새로고침 후 확인
<img width="212" height="35" alt="스크린샷 2025-10-15 오후 11 29 44" src="https://github.com/user-attachments/assets/ef5e0509-034a-4555-a2ba-5d5cd57a32c2" /> <br>
<img width="264" height="335" alt="스크린샷 2025-10-15 오후 11 31 02" src="https://github.com/user-attachments/assets/804ef4bd-802f-496b-a840-5d6b0f4eaebb" /> <br>

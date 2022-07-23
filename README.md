# Auto manage

PK => Primary key(고유 키)
FK => Foreign Key(외래 키)
## User(object)
- id(PK) (string)
- name (string)
- picture (string)
- email (string)
- registered_at (Date)
- updated_at (Date)
- status (가입/ 탈퇴)
- Plant.id
- Manager.id

## Plant(object)
- id (FK, User.id)
- detail information(string)
- name (string)(ex -> 해바라기,장미,선인장,라벤더,오이 )
- temperature (number)
- humity (number)
- light (boolean)
- necessity of wind (boolean)

## Manager(object)
- id (FK, User.id)
- auto watering(o/x)(자동으로 물을 주기를 원하는가?) (boolean)
- wind (o/x)(바람이 필요한가?) (boolean)

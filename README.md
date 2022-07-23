# WebHub db 구조

### PK = Primary Key (고유 키)
### FK = Foreign Key (외래 키)

> ## User
> * id(PK): string
> * name: string
> * picture: string
> * registered_at: string
> * updated_at: string
> * status: "가입" | "탈퇴"
> * followers: User[]
> * followings: User[]
> * username: string
> * password: string
> * email:string
>  
> ## post
> * id(PK):string
> * author: (FK, User.id)
> * date: string
> * title: string
> * code: string
> * description: string
> 
> ## Repository
> * id(PK):string
> * owner: (FK, User.id)
> * name: string
> * description: string
> * Public: boolean
> * tag: string

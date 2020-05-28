# A_Small_Good_Thing API docs

| Method | End Point                        | Request                                         | Response                                             | Usage             |
| ------ | -------------------------------- | ----------------------------------------------- | ---------------------------------------------------- | --------- |
| GET    | /                                | null                                            | `status = 200, { "Success" }`                          |           |
| POST   | /signup                          | `{ body: { "user_name": "test", "email": "test@gmail.com", "password": "12345678" }` | `status = 200, { "id": 3, "user_name": "test", "email": "test2@gmail.com", "password": "12345678" }` | 성공|
|        |                                  |                                                 | `status = 409, { "Already exists user" }` | 실패  |
| POST   | /login                           | `{ body: { "email": "test@gmail.com", "password": "12345678" }` | `{ "user_id": 1, "user_name": "test", "token": "encoded token" }` |로그인 성공|
|        |                                  |                                                 | `status = 403, { "check your email" }`  |실패 이메일|
|        |                                  |                                                 | `status = 401, { "check your password" }` |실패 비밀번호|
|        |                                  | `{ body: {}`                                    | `{id:1,username:'codestates',message:'hello world'}` |자동로그인|
| POST   | /logout                          | `{ body: { "user_id": 1 }`  | `status = 200, { "post logout success" }`   |로그아웃 성공|
| GET    | /monthly-list?user_id=${user_id} | null                                            | `status = 200, {"Success"}`                          |           |
| GET    | /total_list?user_id=${user_id}   | null                                            | `status = 200, {"Success"}`                          |           |
| POST   | /item                            | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| GET    | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| PATCH  | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| DELETE | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| DELETE | /items                           | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| POST   | //image?item_id=${item_id}       | `{username:'codestates',message:'hello world'}` | `{status = 200, {"item_id": "22","image_file": "url"}}` |           |

API 문서 : https://identity.getpostman.com/handover/multifactor?user=11016156&handover_token=747ba966-1e96-47d8-b6b7-cdea81c832b4

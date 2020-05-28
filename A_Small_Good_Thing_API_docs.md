# A_Small_Good_Thing API docs

| Method | End Point                        | Request                                         | Response                                             | Usage     |
| ------ | -------------------------------- | ----------------------------------------------- | ---------------------------------------------------- | --------- |
| GET    | /                                | null                                            | `status = 200, { "Success" }`                          |           |
| POST   | /signup                          | `{username:'codestates',message:'hello world'}` | `status = 200, {"id": 3, "user_name": "test", "email": "test2@gmail.com", "password": "12345678"}` | |
|        |                                  |                                                 | `status = 409, { "Already exists user" }` |           |
| POST   | /login                           | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| POST   | /logout                          | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| GET    | /monthly-list?user_id=${user_id} | null                                            | `status = 200, {"Success"}`                          |           |
| GET    | /total_list?user_id=${user_id}   | null                                            | `status = 200, {"Success"}`                          |           |
| POST   | /item                            | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| GET    | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| PATCH  | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| DELETE | /item?item_id=${item_id}         | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| DELETE | /items                           | `{username:'codestates',message:'hello world'}` | `{id:1,username:'codestates',message:'hello world'}` |           |
| POST   | //image?item_id=${item_id}       | `{username:'codestates',message:'hello world'}` | `{status = 200, {"item_id": "22","image_file": "url"}}` |           |

API 문서 : https://identity.getpostman.com/handover/multifactor?user=11016156&handover_token=747ba966-1e96-47d8-b6b7-cdea81c832b4

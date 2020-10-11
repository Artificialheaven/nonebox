# nonebox

| 字段名 | 数据类型 | 可能的值 | 说明 |
| title | str | - | 帖子标题 |
| content | str | - | 帖子内容 |
| type | str | (版块名) | 版块名 |
| sub_type | str | 热/精 | 是否热帖/精贴 |
| time | num(int64)/str | - | 发布时间戳/发布时间 |
| good | num(int32)/str | - | 帖子赞数 |
| comments_num | num(int64)/str | - | 帖子回复数 |
| sender_name | str | - | 发送者名称 |
| sender_pic | bin/str | - | 发送者头像数据或头像链接 |
| comments | json | - | 回帖数据 |

其中， comments 的数据如下

| 字段名 | 数据类型 | 可能的值 | 说明 |
| com_(2) | json | - | 回复楼层顺序，(2)处应从2开始，每多一层加一 |

其中， com_(2) 的数据如下

| 字段名 | 数据类型 | 可能的值 | 说明 |
| sender_name | str | - | 发送者昵称 |
| word | str | - | 回帖内容 |
| time | num(int64)/str | - | 回复时间戳/回复时间 |
| send_to | str | - | 回复对象 |
| sender_pic | str | - | 发送者头像 

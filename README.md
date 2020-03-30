## 0. 开始

Watermelon Online Judge 线上开发。

## 1. 规约

### 1.1 Java

1. 每个 `*.java` 文件必须加上 `@author` ，代表参与编写的人，多个人用英文逗号分隔，`,` 后面需有空格

2. 每个 ``*.java``   工程文件必须加上 ``@version`` ，在文件变更时对 ``@version`` 进行相应的变更

   - 2.1 小修补之类的对 **末** 位进行更改，如 `1.0.0` -> `1.0.1`
   - 2.2 有功能上的更新，对 **中间** 位进行更改，如 `1.0.0` -> `1.1.0`
   - 2.3 有较大更新，且 **移除** 或 **不兼容** 以往的接口，对 *首位* 进行变更，如 `1.0.0` -> `2.0.0`

```
/**
 * @author Acerkoo, Slanely
 * @version 1.0.0
 */
public class Example {}
```

1. 日志一律使用 `@Slf4j`
2. 不允许直接变更 `dev`、`master` 分支，需 `clone` 至自己的仓库之后进行 `pull request`
3. **请务必遵守阿里巴巴 Java 代码规范 https://github.com/alibaba/p3c**
4. 请使用 Alibaba 代码规约插件 https://github.com/alibaba/p3c/tree/master/idea-plugin
5. 请使用 RESTful API 接口规范 http://www.ruanyifeng.com/blog/2014/05/restful_api.html

### 1.2 Git

1. 请正确配置 `git config user.name` 以及 `git config user.email`
2. `git commit` 时请尽可能使用英文
3. 在进行更改时先将项目克隆至自己的仓库，然后新建一个分支，分支名格式为 `feature/` 或 `bugfix/`，譬如 `feature/check_result_support`、`bugfix/fix_sql_error`，然后发 `pull request` 至项目的 `dev` 分支。

### 1.3 Markdown

https://github.com/ruanyf/document-style-guide

### 1.4 Commits、Issues 等排版

https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-CN.md

### 1.5 Icons

https://fontawesome.com/icons?d=gallery

## 2. 项目说明

| 编号 | 项目                                                         | 作用                                 | 依赖 |
| ---- | ------------------------------------------------------------ | ------------------------------------ | ---- |
| 0    | [WatermelonRoot](https://github.com/WatermelonOj/WatermelonRoot) | 所有项目的 `parent`，作统一版本控制  | 无   |
| 1    | [WatermelonJudger](https://github.com/WatermelonOj/WatermelonJudger) | 用于处理题目评判业务                 | 0    |
| 2    | [WatermelonBackend](https://github.com/WatermelonOj/WatermelonBackend) | 用于处理后端题目、比赛、讨论区等业务 | 0, 1 |
| 3    | [MavenRepo](https://github.com/WatermelonOj/MavenRepo)       | Java 仓库                            | 无   |
| 4    | [WatermelonFrontend](https://github.com/WatermelonOj/WatermelonFrontend) | Watermelon 前端                      | 无   |
| 5    | [README](https://github.com/WatermelonOj/README)             | 规范定义                             | 无   |
| 6    | [WORD-PPT](https://github.com/WatermelonOj/WORD-PPT)         | 答辩材料                             | 无   |


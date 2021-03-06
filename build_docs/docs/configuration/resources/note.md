# スタートアップスクリプト(sakuracloud_note)

---

**全ゾーン共通のグローバルリソースです。**

### 設定例

```hcl
resource sakuracloud_note "mynote" {
  name = "mynote"

  #文字列を直接指定する場合
  content = "#!/bin/sh ..."
  #ファイルから読み込む場合
  #content = "${file("example.sh")}"

  description = "Description"
  tags        = ["tag1", "tag2"]
}
```

### パラメーター

|パラメーター         |必須  |名称                |初期値     |設定値                    |補足                                          |
|-------------------|:---:|--------------------|:--------:|------------------------|----------------------------------------------|
| `name`            | ◯   | スクリプト名           | -        | 文字列                  | - |
| `content`         | ◯   | スクリプト内容           | -        | 文字列                  | - |
| `icon_id`         | -   | アイコンID         | - | 文字列 | - |
| `description`     | -   | 説明  | - | 文字列 | - |
| `tags`            | -   | タグ | - | リスト(文字列) | - |

### 属性

|属性名                | 名称                    | 補足                                        |
|---------------------|------------------------|--------------------------------------------|
| `id`                | スクリプトID             | -                                          |

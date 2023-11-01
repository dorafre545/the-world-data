# DateBase

## 構造

```yaml
Worlds:
  - world_id:
      name: string
      img: string
      players:
        - player_id:
            user_id: string
            email: string
            user_name: string
            role_id: string
            role_name: string
      roles:
        - role_id:
            name: string
            description: string
      areas:
        - area_id:
            name: string
            biome_name: string
      spots:
        - spot_id:
            user_id: string
            user_name: string
            area_id: string
            area_name: string
            name: string
            description: string
            coordinate_x: number
            coordinate_y: number
            coordinate_z: number
            category_id: string
            category_name: string
            image_path: string
            comments:
              - comment_id:
                  user_id: string
                  contents: string
      categories:
        - category_id:
            name: string
            description: string
Biomes:
  - biome_id:
      biome_name: name
      dimension: string
```

## メモ

### 解説

- 親子関係で整合性を保つために、データを冗長化してみたよ
- 整合性が必要なデータの大元が更新された場合はトランザクションで更新するよ

### メモ

正直これが正しいのかよくわからないね  
RDB だったら設計も一瞬なんだけどなー・・・

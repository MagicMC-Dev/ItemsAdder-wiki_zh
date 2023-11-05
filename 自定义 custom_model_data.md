# 自定义 **custom_model_data**

如果你想指定一个物品或方块的 **模型ID** ,你可以使用
``` yaml
    resource:
      material: CLOCK
      model_id: 4000
      generate: false
      model_path: "item/my_custom_item_model"
```

或者让 **ItemsAdder** 来自动生成模型
``` yaml
info:
  namespace: my_items
items:
  my_item_4000_example:
    resource:
      material: DIAMOND
      generate: true
      model_id: 4000
      textures:
      - item/my_custom_texture.png
```
- ⚠️注意：如果你之前创建物品/方块时未指定 模型ID 后使用 /iazip 加载后添加或更改了 模型ID ，需要使用 /iacleancache items 来删除未使用的ID并更新更改后的ID

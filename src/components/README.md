#### 关于定义的Less格式(单纯自我格式约束，非流行规则，使得项目更加整洁有序，节省冗余class)
1. 重复style使用继承：extend; 名称为后续使用的第一个字母，如遇到重复可在其后添加-s
Demo: 
```
.style-v-m {
  vertical-align: middle;
  margin: 10px;
}

<!-- 这是使用了extend的class -->
.background-select {
  &:extend(.style-v-m);
  width: 100px;
}

<!-- 这是未使用extend的class -->
.background-write {
  width: 120px;
  vertical-align: middle;
  margin: 10px;
}

```
# vue drag tree table


[快速体验](https://www.mofazhuan.com/demo/#/ "vue-drag-tree-table")

[API文档](https://www.mofazhuan.com/27.html "vue-drag-tree-table") | [DEMO汇总](https://www.mofazhuan.com/31.html "vue-drag-tree-table") | [常见问题](https://www.mofazhuan.com/29.html "vue-drag-tree-table")

IE10+/Chrome/firefox

## 请更新到```2.0.8```及以上版本
> 基于vue实现的可以拖拽排序的树形表格   

支持拖拽排序、固定头、拖拽改变行宽，checkbox多选、自定义单元格内容、设置行的背景色、动态控制某些行是否可以拖拽等等....

![drag-tree-table](https://www.mofazhuan.com/demo/demo.gif 'drag-tree-table')

## 安装
npm
``` bashs
npm i drag-tree-table --save-dev
```
script
``` bashs
<script src="./dist/dtree-table.js"></script>
```
## 使用方式

```html
<template>
  <div id="app">
    <dragTreeTable
      :data="treeData"
      :onDrag="onTreeDataChange"
      fixed
      border>
    </dragTreeTable>
  </div>
</template>

<script>
import dragTreeTable from "drag-tree-table";
export default {
  name: "app",
  data() {
    return {
      treeData: {
        columns: [...],
        lists: [...]
      }
    };
  },
  components: {
    dragTreeTable
  },
  methods: {
    onTreeDataChange(list) {
      this.treeData.lists = list;
    }
  },
};
</script>

```
更多组件详细功能请参考 [API文档](https://www.mofazhuan.com/27.html "vue-drag-tree-table")

[更新日志-CHANGELOG](CHANGELOG.md 'vue-drag-tree-table')

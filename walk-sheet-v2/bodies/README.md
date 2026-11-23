# 素体数据与页面接口说明

## 1. 数据清单 (`bodies/bodies.js`)

`index.html` 通过 `<script src="bodies/bodies.js"></script>` 引入，脚本挂载全局变量：

```js
window.RM_BASE_BODIES = [
  {
    id: 'floursack-chibi',      // 唯一标识
    name: 'Q版大头',             // 显示名称
    build: 'chibi',             // 体型分类: chibi | child | standard | heavy | tall
    dataUrl: 'data:image/png;base64,...', // 标准 MZ 144x192 透明 PNG
    credit: {
      author: 'Kicked-in-Teeth',
      url: 'https://kicked-in-teeth.itch.io/floursack-base',
      license: 'CC BY-SA'
    }
  }
];
```

## 2. 页面选择接口 (`index.html`)

以下三个函数挂在 `window` 上，统一管理当前选中的素体、自定义素体与 `localStorage` 持久化；界面控件只调用这三个函数：

- `getSelectedBaseBody()`
  返回当前选中的素体对象 `{ id, name, dataUrl }`；未启用素体时返回 `null`。自定义素体的 `id` 为 `'custom'`。
- `setSelectedBaseBody(idOrNull)`
  设置选中项：传入内置素体 `id`、`'custom'`（已上传自定义素体时）或 `null`（不用素体），自动写入 `localStorage` 并刷新控件状态。
- `setCustomBaseBody(dataUrl)`
  设置自定义素体图片（MZ 144×192 PNG data URL），自动切换为选中 `'custom'`、写入 `localStorage` 并刷新控件状态。

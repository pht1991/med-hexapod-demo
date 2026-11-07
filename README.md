# HexaFrame 3D · 六轴外固定架数字化展示平台

**在线演示：https://pht1991.github.io/med-hexapod-demo/**

基于 Three.js 的六轴外固定架（Stewart 平台 / Taylor 支架类结构）Web 3D 交互演示。

## 功能特性

- **实时六柱逆解**：畸形参数（内外翻 / 屈伸 / 旋转 + 三向位移）实时驱动支架形变与骨骼复位动画
- **调整处方输出**：S1~S6 每柱复位 Δ 值、每日 1mm 调节速率下的预计复位周期
- **中英双语**：一键切换全站文案
- **STL 骨骼模型导入**：点击上传或拖拽 `.stl` 文件进页面，自动按断端平面拆分远近骨段并归一化缩放；内置示例股骨一键加载
- **支架规格参数化**：环径 Ø140/160/180mm、环距 250/300/350mm 实时重建

## 定制方向

适用于医疗器械厂商的：官网 3D 交互展示、展会互动大屏、销售演示工具（iPad）、医学教学培训。

联系方式见页面内「器械公司定制」弹窗，或 GitHub: [pht1991](https://github.com/pht1991)

## 运行

纯静态单页，任意静态服务器即可：

```bash
python3 -m http.server 8080
# 或直接访问上面的在线演示
```

## 许可证 / 致谢

- 本仓库代码：MIT
- 示例骨骼模型 `models/femur.stl`：来自 [BoneDensityMapping](https://github.com/Telfer/BoneDensityMapping)（MIT）的 CT 重建测试数据（distal femur）
- 本演示仅用于交互可视化展示，不构成医疗器械或临床计算依据

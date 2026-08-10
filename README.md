# MgDataKit Local Excel

MgDataKit 的本地 Excel 数据源适配器。它读取 Unity 项目内的 `.xlsx` 工作簿，将数据转换为 Core 的 `MgDataSourceReadResult`，并通过统一导入服务写入 `MgDataBase`。

## 要求

- Unity 2022.3
- [MgDataKit Core](https://github.com/MewMewGull/MgDataKit-Core)
- Unity Addressables 1.22.3

## 安装

将仓库检出到 Unity 项目的下列目录：

```text
Assets/MgDataKit/Editor/Adapters/Excel
```

程序集 `MgDataKit.Excel.Editor` 仅在编辑器中启用。仓库包含 NPOI 2.5.6、Portable.BouncyCastle 1.8.9 和 SharpZipLib 1.3.3 的运行时文件；对应许可文本见 `THIRD-PARTY-NOTICES.md`。

## 功能

- Excel 数据源读取与导入
- Excel 资源移动后的路径维护
- 工作表行号引用
- `ColorHex`、列表及常用 Unity 类型解析
- Addressables 资源字段转换

本仓库不保存项目 Catalog、业务表定义或凭据。

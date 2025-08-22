# ARC_Spec

**API 配置与编排运行时引擎规范**

## 简介

ARC_Spec 是一个由 SRON 团队研发的统一API配置解决方案，通过声明式配置文件实现：

- **广泛兼容性**: ARC_Spec 规范自身具有强大的可扩展性，无论是各种参数或响应格式都可以轻松兼容。
- **简明易读性**: ARC_Spec 的标准参数关键词均为日常生活中的通俗用语，简单易懂。
- **描述标准化**: ARC_Spec 专注于解决多个应用程序之间API配置管理中的碎片化问题，让开发者告别重复对接工作，专注于核心业务逻辑。

## 为什么选择 ARC_Spec

更灵活、更强大的可扩展性，和标准规范性。

| 特性 | ARC_Spec 标准规范 | 传统对接方式 |
| --- | --- | --- |
| **开发效率** | 配置文件驱动 | 手工编写调用代码 |
| **维护成本** | 单点配置全局生效 | 多处修改难以同步 |
| **错误处理** | 统一异常规范 | 接口差异处理 |
| **强大生态** | 基于 JSON ：更方便地拓展生态 | 需要单独适配每个API的请求 |

## 编写

我们为您准备了详细的编写指南，请参阅 [Create_An_New_ARC_Spec_Config_File.md](Create_An_New_ARC_Spec_Config_File.md)。通过该指南，你可以详细和准确地编写符合 ARC_Spec 规范的API配置。

## 生态

- **ARC_Spec_Python**：在 Python 上提供对使用 ARC_Spec 规范 格式的文件的进行解析。

## 代码补全

你可以通过引入 Schema 文件，并进行以下配置来启用 JSON 代码的自动补全。

### VS Code 配置方法

在或创建 `.vscode/settings.json` 文件，添加以下配置：

```json
{
  "json.schemas": [
    {
      "fileMatch": ["*.ai.json"],
      "url": "https://raw.githubusercontent.com/SRON-org/ARC_Spec/main/ARC_Spec.Schema.json"
    }
  ]
}
```

### JetBrains IDE 配置方法

1. 打开 `Preferences > Languages & Frameworks > Schemas and DTDs > JSON Schema Mappings`
2. 添加新映射：
   - **Schema file or URL**: `https://raw.githubusercontent.com/SRON-org/ARC_Spec/main/ARC_Spec.Schema.json`
   - **File path pattern**: `*.ai.json`
   - **Schema version**: `Draft 7`

## 标准和示例

- **编码**: UTF-8
- **参考**：[Example.ai.json](Example.ai.json)

## 开放

我们时刻欢迎各位开发者完善和更新协议，欢迎提交 拉取请求 来改进 ARC_Spec ！

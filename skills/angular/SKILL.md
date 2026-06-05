---
name: angular
description: Provides comprehensive guidance for Angular framework including components, modules, services, dependency injection, routing, forms, and TypeScript integration. Use when the user asks about Angular, needs to create Angular applications, implement Angular components, or work with Angular features.
license: Complete terms in LICENSE.txt
---

## When to use this skill

Use this skill whenever the user wants to:
- 用 Angular 构建 SPA、组件、服务、路由与表单
- 使用 CLI、RxJS、依赖注入与模块

## How to use this skill

1. **起步**：ng new、ng generate component/service；模块、组件、模板与绑定。
2. **核心**：路由、HttpClient、表单（响应式/模板）；RxJS 与 async pipe。
3. **参考**：https://angular.io/docs

## Best Practices

- 模块与懒加载；OnPush 与纯管道优化。
- 服务注入与单例；取消订阅防内存泄漏。

## Keywords

angular, 组件, 服务, RxJS, SPA

## 能力边界

### ✅ 适用场景
- 当你需要使用此技能对应的技术栈时
- 当项目需要遵循最佳实践时
- 当需要快速上手或深入理解核心概念时

### ⚠️ 需要注意
- 复杂业务逻辑需要结合具体场景调整
- 性能优化需要根据实际数据量评估

### ❌ 不适用场景
- 不相关的技术栈或框架
- 需要完全自定义的特殊场景

## 常见陷阱 (Gotchas)

1. **版本兼容性**：注意框架版本与依赖库的兼容性，不同版本 API 可能有差异
2. **配置文件格式**：配置文件格式错误是最常见的问题，建议使用编辑器的语法检查
3. **环境变量**：确保所有必要的环境变量已正确设置，敏感信息不要硬编码
4. **依赖冲突**：多版本共存时注意依赖冲突，使用 lock 文件锁定版本
5. **性能陷阱**：大数据量场景下注意性能优化，避免 N+1 查询等常见问题

## 使用流程

### Step 1: 环境准备
确保开发环境已安装必要的依赖和工具。

### Step 2: 配置初始化
根据项目需求进行基础配置。

### Step 3: 核心功能使用
按照示例代码实现核心功能。

### Step 4: 测试验证
运行测试确保功能正常。

### Step 5: 部署上线
完成开发后进行部署和监控。

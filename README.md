# 晨羽智云企业功能文档

基于Mintlify框架构建的晨羽智云企业级AI云算力服务平台完整文档站点。

## 📚 文档概览

本文档站点包含以下主要部分：

- **快速开始** - 5分钟快速上手指南
- **用户指南** - 详细的功能使用说明
- **API参考** - 完整的API接口文档
- **认证指南** - API安全使用最佳实践

## 🚀 快速开始

### 1. 安装Mintlify CLI

```bash
npm install -g mintlify
```

### 2. 本地开发

```bash
# 启动开发服务器
mintlify dev

# 访问 http://localhost:3000 查看文档
```

### 3. 预览构建

```bash
# 构建静态文件
mintlify build

# 预览构建结果
mintlify preview
```

## 📖 文档结构

```
├── mint.json                    # Mintlify 配置文件
├── introduction.mdx             # 主介绍页面
├── quickstart.mdx               # 快速开始指南
├── authentication.mdx           # API认证说明
├── userguide/                   # 用户指南目录
│   ├── introduction.mdx         # 用户指南介绍
│   ├── account-management.mdx   # 账户管理（待添加）
│   ├── instance-management.mdx  # 实例管理（待添加）
│   ├── billing.mdx             # 计费说明（待添加）
│   └── monitoring.mdx          # 监控告警（待添加）
└── api-reference/              # API参考目录
    ├── introduction.mdx        # API参考介绍
    ├── instances/              # 实例管理API
    │   ├── create.mdx          # 创建实例
    │   ├── list.mdx            # 查询实例列表（待添加）
    │   ├── start.mdx           # 启动实例（待添加）
    │   ├── stop.mdx            # 停止实例（待添加）
    │   ├── restart.mdx         # 重启实例（待添加）
    │   └── status.mdx          # 查询实例状态（待添加）
    └── account/                # 账户管理API
        ├── balance.mdx         # 查询余额
        ├── billing.mdx         # 查询账单（待添加）
        └── recharge.mdx        # 查询充值记录（待添加）
```

## 🎨 特色功能

### 响应式设计
- 完美适配桌面端和移动端
- 深色/浅色主题自动切换
- 流畅的用户体验

### 交互式API文档
- 实时API请求测试
- 多语言代码示例（Python、JavaScript、cURL、Go）
- 完整的请求/响应示例

### 丰富的组件
- CardGroup - 卡片组布局
- Tabs - 标签页切换
- Accordion - 折叠面板
- Steps - 步骤指引
- CodeGroup - 代码组
- Mermaid图表 - 流程图支持

## 🔧 配置说明

### 主题配置

在 `mint.json` 中配置主题色彩：

```json
{
  "colors": {
    "primary": "#7C3AED",
    "light": "#A855F7", 
    "dark": "#5B21B6"
  }
}
```

### 导航配置

支持多层级导航和分组：

```json
{
  "navigation": [
    {
      "group": "快速开始",
      "pages": ["introduction", "quickstart", "authentication"]
    },
    {
      "group": "用户指南", 
      "pages": ["userguide/introduction", "userguide/account-management"]
    }
  ]
}
```

## 🌟 设计亮点

### 参考SiliconFlow设计
- 借鉴了SiliconFlow文档的优秀设计理念
- 保持了专业的技术文档风格
- 优化了中文用户的阅读体验

### 企业级功能
- 完整的API权限管理说明
- 详细的安全最佳实践
- 成本控制和预算管理指南

### 开发者友好
- 丰富的代码示例
- 详细的错误处理说明
- 完整的SDK使用指南

## 📝 内容特色

### 🎯 实用性强
- 5分钟快速上手指南
- 真实的业务场景示例
- 完整的故障排除指南

### 🔒 安全为先
- API Key管理最佳实践
- 权限控制详细说明
- 安全事件响应流程

### 💰 成本透明
- 详细的计费规则说明
- 成本优化建议
- 预算控制策略

## 🚀 部署选项

### 1. Mintlify托管
```bash
# 连接到Mintlify
mintlify deploy

# 自动部署到 https://your-docs.mintlify.com
```

### 2. Vercel部署
```bash
# 安装Vercel CLI
npm install -g vercel

# 部署到Vercel
vercel
```

### 3. Netlify部署
```bash
# 构建静态文件
mintlify build

# 将 .mintlify/_next 目录部署到Netlify
```

## 📋 待完善内容

以下页面已规划但待添加：

### 用户指南
- [ ] 账户管理详细说明
- [ ] 实例管理操作指南
- [ ] 计费规则和优化策略
- [ ] 监控告警配置

### API参考
- [ ] 实例列表查询
- [ ] 实例启动/停止/重启
- [ ] 实例状态查询
- [ ] 账单查询
- [ ] 充值记录查询

### 其他功能
- [ ] 搜索功能优化
- [ ] 多语言支持
- [ ] 用户反馈系统
- [ ] 更新日志

## 🤝 贡献指南

欢迎贡献内容和改进建议！

### 添加新页面
1. 在相应目录下创建 `.mdx` 文件
2. 在 `mint.json` 的 `navigation` 中添加页面路径
3. 使用一致的格式和组件

### 改进现有内容
1. 直接编辑相应的 `.mdx` 文件
2. 保持内容的准确性和时效性
3. 遵循现有的写作风格

## 📞 技术支持

如果您在使用过程中遇到问题，请：

1. 查看 [Mintlify官方文档](https://mintlify.com/docs)
2. 提交Issue到项目仓库
3. 联系技术支持团队：support@chenyu.com

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

# MQTTHub 🔗

**[English](README.md) | [中文](README-zh.md)**

一个专业的基于Web的MQTT客户端测试平台，具有现代化界面和全面的功能。

## ✨ 功能特性

### 🔌 连接管理
- **灵活的代理支持** - 通过WebSocket连接任何MQTT代理服务器
- **身份验证** - 支持用户名/密码认证
- **自动生成客户端ID** - 唯一客户端标识符生成
- **实时状态** - 实时连接状态监控

### 📬 主题订阅
- **模式匹配** - 支持MQTT通配符模式（`+`, `#`）
- **多重订阅** - 同时订阅多个主题
- **轻松管理** - 一键订阅/取消订阅
- **QoS支持** - 服务质量等级配置

### 📤 消息发布
- **JSON格式化** - 内置JSON格式化器，支持语法验证
- **QoS等级** - 支持QoS 0、1、2等级
- **内容验证** - 实时JSON语法检查
- **快速发送** - 键盘快捷键提高发布效率

### 📊 消息监控
- **实时显示** - 带时间戳的实时消息流
- **智能折叠** - 接收消息默认折叠
- **消息控制** - 展开/折叠、复制和清空功能
- **语法高亮** - JSON内容格式化显示
- **可滚动内容** - 长消息自动滚动

### 📱 响应式设计
- **移动端优化** - 移动设备标签式导航
- **桌面布局** - 大屏幕多面板布局
- **现代UI** - 渐变背景和流畅动画
- **无障碍访问** - 适当的对比度和语义标记

## 🚀 快速开始

### 在线使用
1. 在任何现代Web浏览器中打开HTML文件
2. 输入MQTT代理WebSocket URL（例如：`ws://broker.emqx.io:8083/mqtt`）
3. 如需要，配置身份验证
4. 点击**连接**
5. 开始订阅主题和发布消息

### 本地开发
```bash
# 克隆仓库
git clone https://github.com/yourusername/mqtthub.git

# 进入项目目录
cd mqtthub

# 使用本地服务器打开（推荐）
python -m http.server 8080
# 或者
npx serve .

# 在浏览器中打开
open http://localhost:8080
```

## 🛠️ 技术细节

### 构建技术
- **HTML5** - 语义化标记
- **Tailwind CSS** - 实用优先的CSS框架
- **原生JavaScript** - 无框架依赖
- **MQTT.js** - 强大的MQTT客户端库

### 浏览器兼容性
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

### 依赖项
- [MQTT.js](https://github.com/mqttjs/MQTT.js) - JavaScript MQTT客户端
- [Tailwind CSS](https://tailwindcss.com/) - CSS框架

## 📋 使用示例

### 连接到代理服务器
```
代理URL: ws://broker.emqx.io:8083/mqtt
客户端ID: mqtt_test_abc123
用户名: (可选)
密码: (可选)
```

### 订阅模式
```
sensor/+/temperature    # 所有温度传感器
device/#                # 所有设备主题
home/living/+          # 所有客厅传感器
```

### 消息发布
```json
{
  "deviceId": "sensor001",
  "temperature": 23.5,
  "humidity": 65.2,
  "timestamp": "2025-05-30T10:30:00Z"
}
```

## 🎯 使用场景

- **物联网开发** - 测试设备连接和消息流
- **MQTT学习** - 动手理解MQTT概念
- **系统集成** - 验证系统间MQTT通信
- **调试** - 故障排除MQTT应用程序
- **原型开发** - 快速测试MQTT场景

## 🔧 配置说明

工具默认连接到公共MQTT代理。生产环境使用时：

1. **安全连接** - 使用WSS（WebSocket安全）URL
2. **身份验证** - 配置适当的凭据
3. **主题权限** - 确保正确的ACL设置
4. **速率限制** - 考虑消息速率限制

## 📱 移动端功能

在移动设备上，界面切换为标签式布局：
- 📡 **连接** - 连接配置
- 📬 **订阅** - 主题订阅管理
- 📤 **发送** - 消息发布
- 📊 **监控** - 实时消息监控

## 🤝 贡献

欢迎贡献！请随时提交Pull Request。

### 开发设置
1. Fork仓库
2. 创建功能分支（`git checkout -b feature/AmazingFeature`）
3. 提交更改（`git commit -m 'Add some AmazingFeature'`）
4. 推送到分支（`git push origin feature/AmazingFeature`）
5. 打开Pull Request

## 📄 许可证

本项目使用MIT许可证 - 详情请查看[LICENSE](LICENSE)文件。

## 🙏 致谢

- [MQTT.js](https://github.com/mqttjs/MQTT.js) 提供优秀的MQTT客户端库
- [Tailwind CSS](https://tailwindcss.com/) 提供实用优先的CSS框架
- [EMQ X](https://www.emqx.io/) 提供用于测试的公共MQTT代理

## 📞 支持

如果您有任何问题或疑问，请：
1. 查看[Issues](https://github.com/yourusername/mqtthub/issues)页面
2. 如需要创建新issue
3. 提供关于环境和问题的详细信息

---

用❤️为物联网社区制作

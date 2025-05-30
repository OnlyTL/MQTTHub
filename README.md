# MQTTHub 🔗

**[English](README.md) | [中文](README-zh.md)**

A professional web-based MQTT client testing platform with a modern interface and comprehensive features.

## ✨ Features

### 🔌 Connection Management
- **Flexible Broker Support** - Connect to any MQTT broker via WebSocket
- **Authentication** - Username/password authentication support
- **Auto-generated Client ID** - Unique client identifier generation
- **Real-time Status** - Live connection status monitoring

### 📬 Topic Subscription
- **Pattern Matching** - Support for MQTT wildcard patterns (`+`, `#`)
- **Multiple Subscriptions** - Subscribe to multiple topics simultaneously
- **Easy Management** - One-click subscription/unsubscription
- **QoS Support** - Quality of Service level configuration

### 📤 Message Publishing
- **JSON Formatting** - Built-in JSON formatter with syntax validation
- **QoS Levels** - Support for QoS 0, 1, and 2
- **Content Validation** - Real-time JSON syntax checking
- **Quick Send** - Keyboard shortcuts for efficient publishing

### 📊 Message Monitoring
- **Real-time Display** - Live message feed with timestamps
- **Smart Collapsing** - Received messages collapsed by default
- **Message Controls** - Expand/collapse, copy, and clear functions
- **Syntax Highlighting** - JSON content with proper formatting
- **Scrollable Content** - Automatic scrolling for long messages

### 📱 Responsive Design
- **Mobile Optimized** - Tab-based navigation for mobile devices
- **Desktop Layout** - Multi-panel layout for larger screens
- **Modern UI** - Gradient backgrounds and smooth animations
- **Accessibility** - Proper contrast and semantic markup

## 🚀 Quick Start

### Online Usage
1. Open the HTML file in any modern web browser
2. Enter your MQTT broker WebSocket URL (e.g., `ws://broker.emqx.io:8083/mqtt`)
3. Configure authentication if required
4. Click **Connect**
5. Start subscribing to topics and publishing messages

### Local Development
```bash
# Clone the repository
git clone https://github.com/yourusername/mqtthub.git

# Navigate to the project directory
cd mqtthub

# Open with a local server (recommended)
python -m http.server 8080
# or
npx serve .

# Open in browser
open http://localhost:8080
```

## 🛠️ Technical Details

### Built With
- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework
- **Vanilla JavaScript** - No framework dependencies
- **MQTT.js** - Robust MQTT client library

### Browser Compatibility
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

### Dependencies
- [MQTT.js](https://github.com/mqttjs/MQTT.js) - MQTT client for JavaScript
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework

## 📋 Usage Examples

### Connecting to a Broker
```
Broker URL: ws://broker.emqx.io:8083/mqtt
Client ID: mqtt_test_abc123
Username: (optional)
Password: (optional)
```

### Subscription Patterns
```
sensor/+/temperature    # All temperature sensors
device/# 	              # All device topics
home/living/+          # All living room sensors
```

### Message Publishing
```json
{
  "deviceId": "sensor001",
  "temperature": 23.5,
  "humidity": 65.2,
  "timestamp": "2025-05-30T10:30:00Z"
}
```

## 🎯 Use Cases

- **IoT Development** - Test device connectivity and message flow
- **MQTT Learning** - Understand MQTT concepts hands-on
- **System Integration** - Validate MQTT communication between systems
- **Debugging** - Troubleshoot MQTT-based applications
- **Prototyping** - Quick testing of MQTT scenarios

## 🔧 Configuration

The tool connects to public MQTT brokers by default. For production use:

1. **Secure Connections** - Use WSS (WebSocket Secure) URLs
2. **Authentication** - Configure proper credentials
3. **Topic Permissions** - Ensure proper ACL settings
4. **Rate Limiting** - Consider message rate limits

## 📱 Mobile Features

On mobile devices, the interface switches to a tab-based layout:
- 📡 **Connect** - Connection configuration
- 📬 **Subscribe** - Topic subscription management
- 📤 **Publish** - Message publishing
- 📊 **Monitor** - Real-time message monitoring

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [MQTT.js](https://github.com/mqttjs/MQTT.js) for the excellent MQTT client library
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [EMQ X](https://www.emqx.io/) for providing public MQTT broker for testing

## 📞 Support

If you have any questions or issues, please:
1. Check the [Issues](https://github.com/yourusername/mqtthub/issues) page
2. Create a new issue if needed
3. Provide detailed information about your environment and the problem

---

Made with ❤️ for the IoT community

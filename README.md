# “时空旋量”智能乒乓球运动分析系统

## 项目介绍
* 赛事： 第十六届服务外包创新创业大赛（企业A类-百度赛道）西部赛区铜奖
* “时空旋量”智能乒乓球运动分析系统是一个利用现代技术对乒乓球运动进行分析和提供反馈的系统。

## 核心功能 🎯

*   **🏓 轨迹与动作检测**: 精确识别乒乓球的轨迹、速度、角度、落点，并对运动员的移动、挥拍、击球姿势进行识别与分类。
*   **📈 事件识别与战术分析**: 基于连续帧分析和事件标签，实现技战术事件的自动分类，并结合文心大模型进行语言分析总结。
*   **📊 数据可视化**: 通过动态轨迹图、热力图等方式呈现训练数据，方便用户清晰把握训练情况。
*   **📂 用户数据管理**: 建立用户数据库，系统化管理训练数据与个人信息，长期跟踪运动进展。
*   **✍️ 个性化建议**: 基于训练数据和分析结果，结合文心大模型生成个性化的改进建议报告。
*   **☁️ 平台支持**: 支持云端与本地部署，覆盖电脑端和移动设备端。

## 技术特色 ✨

*   **🧠 跨模态特征融合**: 整合视觉 (PP-TSM)、音频 (VGGish) 及姿态 (GHUM) 多源数据流，通过门控注意力LSTM实现动态权重分配。
*   **🚀 轻量化时空建模**: 基于SPP-NAS骨干网络，用时序位移模块替代3D卷积，在2D计算复杂度下实现微秒级时空建模。
*   **🦾 生物力学解析**: 通过参数化GHUM模型构建三维运动链拓扑，实现挥拍动作动力学传导路径可视化。
*   **📍 双流时序定位**: 融合BMN边界匹配与VFL损失函数，通过二维置信度图优化动作起止概率与质量评分。
*   **⚙️ 自适应多任务优化**: 构建"检测-姿态-动作"级联训练框架，采用SimOTA动态标签分配，形成端到端智能分析系统。

## 技术栈 🛠️

*   **语言**: Python 🐍
*   **框架与库**: PaddleDetection, PaddleVideo, TensorFlow, MediaPipe, PyTorch, Flask, SQLAlchemy
*   **工具**: PyCharm, Visual Studio Code, 宝塔面板
*   **数据库**: MySQL 🗄️
*   **平台**: Windows, Android 🖥️📱

## 项目部分展示
![Page 1](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0001.jpg)
![Page 4](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0004.jpg)
![Page 7](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0007.jpg)
![Page 8](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0008.jpg)
![Page 9](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0009.jpg)
![Page 10](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0010.jpg)
![Page 20](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0020.jpg)
![Page 39](https://github.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/blob/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0039.jpg)
![Page 11](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0011.jpg)
![Page 14](https://raw.githubusercontent.com/Firefly-ZRK/-Time-Space-Spin-smart-ping-pong-sports-analysis-system/main/JPG/%E2%80%9C%E6%97%B6%E7%A9%BA%E6%97%8B%E9%87%8F%E2%80%9D%E6%99%BA%E8%83%BD%E4%B9%92%E4%B9%93%E7%90%83%E8%BF%90%E5%8A%A8%E5%88%86%E6%9E%90%E7%B3%BB%E7%BB%9F_page-0014.jpg)

## 数据集获取 📥
### 需要P2ANet数据集（乒乓球）的同学可以联系我: 3453743484@qq.com 📧

# EasyTier-Web飞牛套件
- EasyTier是一个由 Rust 和 Tokio 驱动的简单、安全、去中心化的异地组网方案。
- EasyTier-Web是为EasyTier提供web管理页面，让用户更直观地管理组网。
### 使用方法：
1. 打开 Web 管理页：飞牛桌面点击 EasyTier-Web 图标，或浏览器访问 `http://<飞牛IP>:11211`。
2. **首次使用请先注册账号**（点击登录页的注册/Sign up，创建用户名和密码），本版本无内置初始账号，旧的 `admin/admin` 已不再适用。
3. 登录后，在左侧侧边栏进入 **Network（网络）** 页面，点击右上角 **Create Network（创建网络）**，填写 Network Name、Network Secret、虚拟 IP（如 `10.126.126.1`）后保存即可开始组网。
4. 如需自定义 Web 端口，编辑 `[应用文件] - [Easytier-Web] - config.json` 中的 `uiport` 字段，修改后重启应用生效。

### 注意事项：
- 本应用默认占用 **11211**（Web/API 端口）与 **22020**（easytier-core 连接 web-embed 的配置服务端口）。请避免这些端口被其他程序占用。
- 若飞牛本机已运行其他 easytier 程序或容器（默认会占用 11010 等端口），建议先关闭再使用本应用，避免冲突。
- 组网实例由 `easytier-core` 在后台运行，Web 端仅作管理；创建网络后节点状态请在 Network / Nodes 页面查看。
### 界面截图：
<img width="500" height="350" alt="PixPin_2025-11-17_17-53-22" src="https://github.com/user-attachments/assets/bd12cc0c-6ea4-43be-8c94-8de33317880d" /><img width="500" height="350" alt="PixPin_2025-11-17_17-54-12" src="https://github.com/user-attachments/assets/2bea4c7b-17bd-4730-8e8d-8a58a732395f" />

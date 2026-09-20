# Donvis ProLite 修正版安装包 for MacOS

此安装包基于 Donvis 1.7.0，包含已验证的 ChatGPT/Codex ProLite 额度读取、分类与展示修复。

## 本次升级

- 适配 OpenAI 取消 5 小时额度窗口后的新规则。
- 修复原版仍按“5 小时 + 7 天”双窗口解析，导致额度分类与展示错误的问题。
- 兼容 ChatGPT 与 Codex 合并后的新桌面端，恢复额度正常读取。
- 将官方唯一主额度窗口统一映射至「7 天」栏，展示剩余比例与重置时间。
- 将「5 小时」栏及其重置时间保留为空，避免误导。
- 不影响 Claude 监控、刷新机制及其他原有功能。

## 安装

双击 `Donvis-ProLite-Modified-1.7.0.pkg`，按系统提示完成安装。它会安装为 `/Applications/Donvis.app`，因此会替换同路径的 Donvis。

安装前如需保留当前版本，请先复制 `/Applications/Donvis.app`。

## 验证与边界

- 应用载荷使用本机 ad-hoc 签名，安装包未使用 Apple Developer 证书；系统可能显示未签名提示。
- `SHA256.txt` 用于在传输后校验安装包完整性。
- 本版本不调用额度消费或重置接口，不改动账户、网络或代理设置。

菜单栏效果
<img width="597" height="31" alt="Snipaste_20260920_190542" src="https://github.com/user-attachments/assets/e89c055f-33aa-4770-b6e4-0ee2f912147a" />

展开效果
<img width="378" height="426" alt="Snipaste_20260920_190653" src="https://github.com/user-attachments/assets/d6eb3a15-9bdd-4722-a180-9cc0389fdd77" />

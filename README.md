# jianying-headless-SafeFork

这是 [mcncarl/jianying-headless](https://github.com/mcncarl/jianying-headless) 的 SafeFork。创建者已确认取得原作者对公开、持续同步镜像的书面授权。

## 分支用途

- [main](../../tree/main)：保留上游源码、Git 历史、LICENSE、NOTICE 与第三方声明。
- sync-control：默认分支，仅保存自动同步工作流，不属于上游源码。

## 同步规则

- 每小时检查一次，也可在 Actions 中手动执行；GitHub 可能延迟或跳过定时运行。
- 只创建缺失分支、快进已有分支、复制缺失 Tag。
- 遇到分叉历史或同名异 SHA 的 Tag 会停止，不会强制覆盖。
- 不删除 Fork 独有分支或 Tag，不创建自动备份分支。

查看源码请切换到 [main](../../tree/main)。使用或再分发源码时仍须遵守[上游许可证](https://github.com/mcncarl/jianying-headless/blob/main/LICENSE)及第三方声明；SafeFork 不改变这些条款。本控制分支的 SafeFork 工作流采用 [MPL-2.0](https://github.com/CaptainUnhappy/SafeFork/blob/main/LICENSE)。
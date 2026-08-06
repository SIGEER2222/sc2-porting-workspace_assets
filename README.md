# SC2 Porting Workspace Assets

大文件资产仓库（贴图 .dds / 模型 .m3 / 触发器二进制 / 地图遮罩 t3TextureMasks）。

从主仓库 sc2-porting-workspace 拆分而来，保持原相对路径结构。

## 用法

```bash
# 主仓库中作为 submodule 引用
git submodule add <url> assets
git submodule update --init assets
```

## 结构

文件保持从主仓库拆分时的相对路径，例如：
- `src/projects/revolution-overdrive-porting/packages/Commander/Mods/RevolutionOverdrive.SC2Mod/Assets/Textures/*.dds`
- `src/projects/cmre-porting/packages/Mods/CMRE/CMRE_Core_Triggers.SC2Mod/Triggers`

主仓库通过 symlink 或复制到原位置使用。

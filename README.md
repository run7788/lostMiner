# LostMiner Mod 接手包

LostMiner（`com.fsilva.marcelo.lostminer`）内容级 mod 逆向重打包项目。

- Mod 类型：内容级（方块/物品/合成/生物），直接修改 dex 字节码
- 当前状态：fixed15 已重签名验证（apksig verified=true，v1/v2/v3 完整）
- 测试环境：模拟器（无 GMS）

## 仓库内容
| 文件 | 说明 |
|---|---|
| `LostMinerMod_handover_20261005_clean.zip` | 完整接手包（不含签名密钥） |
| `*.part01..part05` | 分块（每份 <20MB），拼接后还原 zip |
| `README.md` | 本文件 |

## 拼接还原
Linux/macOS：
```bash
cat LostMinerMod_handover_20261005_clean.zip.part01 \
    LostMinerMod_handover_20261005_clean.zip.part02 \
    LostMinerMod_handover_20261005_clean.zip.part03 \
    LostMinerMod_handover_20261005_clean.zip.part04 \
    LostMinerMod_handover_20261005_clean.zip.part05 \
    > LostMinerMod_handover_20261005_clean.zip
```

> 签名密钥 `marvis-signing.p12` 未随包上传（公开仓库安全考虑），需要时向维护者索取。

# 内置素体来源与许可

所有内置素体均已规整为 RPG Maker MZ 标准单人行走图规格：144×192（每格 48×48，四行依次为下／左／右／上，三列依次为左步／站立／右步，透明背景，脚底线统一为距格底 2 px）。

| 文件 | 名称 | 体型 (`build`) | 作者 | 来源 | 许可证 | 导出署名要求 |
| --- | --- | --- | --- | --- | --- | --- |
| `chibi-walk.png` | Q版大头·步态 | `chibi` | 本项目原创（参考 Cabbit CC0 步态） | 本仓库 `bodies/tools/make-chibi-walk.py` 逐像素生成 | CC0 | 免署名，可商用、可改编 |
| `floursack-chibi.png` | Q版大头 | `chibi` | Kicked-in-Teeth | https://kicked-in-teeth.itch.io/floursack-base | CC BY-SA | **需要署名** Kicked-in-Teeth；若公开分发基于此素体改编的素材，需以相同许可（CC BY-SA）共享 |
| `cabbit-child.png` | 小孩 | `child` | Cabbit / diamonddmgirl / AntumDeluge | https://opengameart.org/node/84455 | CC0 | 免署名，可商用、可改编 |
| `cabbit-standard.png` | 标准 | `standard` | Cabbit / diamonddmgirl / AntumDeluge | https://opengameart.org/node/84455 | CC0 | 免署名，可商用、可改编 |
| `cabbit-heavy.png` | 壮实 | `heavy` | Cabbit / diamonddmgirl / AntumDeluge | https://opengameart.org/node/84455 | CC0 | 免署名，可商用、可改编 |
| `blazingmagpie-adult.png` | 三头身 | `tall` | BlazingMagpie | https://opengameart.org/node/16122 | CC0 | 免署名，可商用、可改编 |

## 处理说明

- `chibi-walk.png`：由 Python/Pillow 逐像素原创绘制（参考 Cabbit CC0 步态，非 Floursack 衍生），约 1.9 头身，站立帧高 45 px、迈步帧高 44 px，左右步带清晰迈腿与反向摆臂，侧面以明暗区分前后腿，全 12 帧脚底线统一距格底 2 px。
- `floursack-chibi.png`：原图 `pale 02.png`（144×192），行顺序由 下／上／右／左 重排为 下／左／右／上，像素 1:1 保留（高 39 px）。
- `cabbit-child.png`：原图 `SWEN_child_armsA.png`（144×256，48×64/格），1:1 裁入 48×48（高 45 px），统一脚底线至距格底 2 px。
- `cabbit-standard.png`：原图 `SWEN_adult_f_thin_torsoA_armsA.png`（144×256，48×64/格），人物原高 51 px，按最近邻等比缩放至 44 px 放入 48×48，统一脚底线至距格底 2 px。
- `cabbit-heavy.png`：原图 `SWEN_adult_m_heavy.png`（144×256，48×64/格），人物原高 51 px，按最近邻等比缩放至 44 px 放入 48×48，统一脚底线至距格底 2 px。
- `blazingmagpie-adult.png`：原图 `Base.png`（96×192，32×48/格），行顺序由 下／上／右／左 重排为 下／左／右／上，列顺序由 站立／左步／右步 重排为 左步／站立／右步，1:1 居中放入 48×48（高 38–39 px），统一脚底线至距格底 2 px。

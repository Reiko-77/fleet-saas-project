# 大客户车队管理 SaaS

车辆入队、车队运营与权限管理的交互演示。

[项目版本目录](https://reiko-77.github.io/fleet-saas-project/) · [打开最新 v8limit-merge](https://reiko-77.github.io/fleet-saas-project/?version=v8limit-merge)

| 版本 | 演示内容 |
| --- | --- |
| [v8limit-merge](https://reiko-77.github.io/fleet-saas-project/?version=v8limit-merge) | 账号内管理组织与角色、多组织角色组合、集团社会信用代码 |
| [v7limit](https://reiko-77.github.io/fleet-saas-project/?version=v7limit) | 统一权限管理 |
| [v6.2limit](https://reiko-77.github.io/fleet-saas-project/?version=v6.2limit) | 按管理员身份区分账号与角色 |
| [v6.1limit](https://reiko-77.github.io/fleet-saas-project/?version=v6.1limit) | 账号权限与系统权限分区 |
| [v6limit](https://reiko-77.github.io/fleet-saas-project/?version=v6limit) | 账号、角色与组织管理 |
| [v5](https://reiko-77.github.io/fleet-saas-project/?version=v5) | 车辆入队与资料维护 |
| [v4merge](https://reiko-77.github.io/fleet-saas-project/?version=v4merge) | 车队管理合版 |
| [v3](https://reiko-77.github.io/fleet-saas-project/?version=v3) | 车辆列表与状态 |
| [v2](https://reiko-77.github.io/fleet-saas-project/?version=v2) | 车辆分配 |
| [v1](https://reiko-77.github.io/fleet-saas-project/?version=v1) | 待入队车辆 |
| [pre-allocation](https://reiko-77.github.io/fleet-saas-project/?version=pre-allocation) | 车辆分配前快照 |

[原 v6.2limit 发布地址](https://reiko-77.github.io/saas-fleet-demo/)

## v8 development

Source: `versions/v8limit-merge/`. Build: `python3 scripts/build-v8.py`.

Cloud backup branch: `v7limit-backup-20261109`. Source and tests are also archived in `v8limit-merge-source.zip` (extract into repository root).

Local rollback tag: `v7limit-before-v8merge-20261109` (commit `1e09541`). Previous version payloads are preserved. v8 uses separate localStorage. No highest-role permission merging. Group switching uses demo phone `13800000001` and its active memberships, not real authentication.

Test: install Playwright, run `node tests/v8.cjs`; set `DEMO_URL` and optional `CHROME_PATH`.

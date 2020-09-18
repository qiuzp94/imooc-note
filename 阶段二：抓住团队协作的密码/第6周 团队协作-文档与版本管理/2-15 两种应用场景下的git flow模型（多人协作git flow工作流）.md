## 经典模型的问题
* 必须使用dev分支
* 复杂度高:hotfix与release分支
* 多次Merge合并

## Git Flow(模型一)
* 适用于持续集成多环境场景
* 上游分支向下游发展
* 流程:`Bug -> New Branch -> master -> pre branch -> Target Branch`

## Git Flow(模型二)
* 适用于版本项目
* 稳定版本从master检出bug修复在分支
* 流程: `master -> Stable -> new branch -> bug fix -> version`
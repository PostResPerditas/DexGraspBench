# Docs

## 问题
base: /data/Project/DexGraspBench 项目中内容使用 conda 环境 DGbench
base: /data/Project/BODex 项目中内容使用 conda 环境 bodex
DexGraspBench 中使用评估指令 python src/main.py task=format exp_name=debug task.max_num=100 task.data_path=../BODex/src/curobo/content/assets/output/sim_shadow/fc/debug/graspdata
python src/main.py task=eval exp_name=debug task.max_num=1000 [或者 bash script/test_BODex_shadow.sh] 和 bodex 中使用 python example_grasp/evaluate_mujoco_grasps.py -c example_grasp/config/eval_mujoco.yml --mode squeeze 的仿真结果成功率不同，使我们自定义的评估环境哪方面与 dexgraspbench 存在差别呢
anaconda base环境需要管理员权限
直接改owner不能解决
用管理员权限运行conda prompt简单粗暴有效，但是有风险


推荐方案：  用本地用户账户 （not as admin）新建一个环境，
conda create -n sci anaconda
这样的环境有anaconda默认包，但是owner是local用户，不需要管理员权限。




vscode 看不见conda环境
需要 >python:Select Interpreter  手动browze选中conda下面的python.exe




对于生产环境，venv + pip 比conda简洁、可靠性更高。



anaconda默认的opencv不识别

需要conda install -c conda-forge opencv

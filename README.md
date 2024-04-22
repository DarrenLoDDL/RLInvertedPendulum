You can execute this on windows, you need to first install XLauncher and Ubuntu on your computer
OPEN UBUNTU FOR THIS:

First, install all thenecessary mujoco files:

>export MUJOCO_PY_MUJOCO_PATH= ~/.mujoco/mujoco200/
>export MUJOCO_PY_MJKEY_PATH= ~/.mujoco/mjkey.txt

>export LD_LIBRARY_PATH=~/.mujoco/mujoco200/bin:$LD_LIBRARY_PATH
>export MUJOCO_PY_MUJOCO_PATH= ~/.mujoco/mujoco200/
>export MUJOCO_PY_MJKEY_PATH= ~/.mujoco/mjkey.txt

>source ~/.profile
--------------------------

COMMAND SEQUENCE FOR DISPLAYING

Set up XServer-> multi windows, disable checking (makes you vulnerable exit after session)
(If on desktop, try "open large window")

>export LIBGL_ALWAYS_INDIRECT=0;
>export DISPLAY=localhost:0
export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2}'):0
>conda activate gym;
>export LD_LIBRARY_PATH=~/.mujoco/mujoco200/bin:$LD_LIBRARY_PATH;
>jupyter notebook --no-browser --port=9998

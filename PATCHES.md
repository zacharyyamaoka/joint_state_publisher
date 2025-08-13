1. Deleted joint_state_publisher as will be using system install
2. Renamed from joint_state_publisher_gui to -> joint_state_publisher_gui_local
    - This helps prevent any naming issues with underyling package, which you can always easily still access now
    - Make sure to change import names within the package as well
3. Added cmake and edit package xml based on py_ws examples so that colcon build works. Colcon wasn't working on the setup.py that came with the package
4. Installed Pyside, etc. so modules that needed to be installed.
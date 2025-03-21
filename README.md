# Wifi-and-Sensor-data
Start/Modify a project in STM32 IoT node to read the sensor value, such as 3D Accelerator or 3D gyro, and send the data (using wifi with http or a tcp protocol) to a Linux(RPi)/Windows/Mac host and Visualize with some kind of GUI tools (such as using Python）

在完成这个任务时，首先需要按照Sensor reading and communication using wifi client.pdf完成相关配置，该文件针对的目录为C:\Users\yourname\STM32Cube\Repository\STM32Cube_FW_L4_V1.18.1\Projects\B-L475E-IOT01A\Applications\WiFi\WiFi_Client_Server\STM32CubeIDE。

建立python文件，运行 Python socket server.py。

修改main.c的相关配置，主要包括网络，ip和端口配置。并连接Python socket server，手机sensor资料后，透过sokect送出。（参考mian.c）

注意：如果是连接手机热点，需要保证手机WIFI处在2-4G频段。

最后得到图形化展示：
![image](https://github.com/user-attachments/assets/500a5cbc-624d-4b95-9837-d3b1771b72e6)


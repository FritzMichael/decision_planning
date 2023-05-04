#### **Linux**

Unfortunately we havent found a way to run CARLA in linux without GPU, so we highly recommend to use Windows if you dont have access to a GPU.

### Repository Setup with Docker

1. Install Visual Studio Code.
2. Install remote ssh extension of Visual Studio Code.
3. Install [Docker for Linux](https://docs.docker.com/engine/install/ubuntu/).
4. Install the latest NVIDIA driver
5. Install [NVIDIA docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)

6. Open project in VSCode folder (ctrl+k ctrl+o).
7. Open controls panel clicking the green buttom in the lower left part of vs code.
8. Select the option, **Reopen in container**.
9. Start developing your algorithms.

### Repository Setup with Anaconda

You can use Ananconda for this, however it only will work for **Ubuntu 18.04**, please follow these instructions.

1. Install Visual Studio Code.
2. Install [Ananconda](https://docs.anaconda.com/free/anaconda/install/windows/).
3. Open **Anaconda Prompt** and type:
    
    <code>conda init</code>
4. Open Anaconda and create a new environment called **decision** with python **3.7** (IMPORTANT).

    <code>conda create -n decision python=3.7</code>

5. Open Visual Studio Code in the root of this repository.
6. Open a new terminal and type:   

    <code>conda activate decision</code>
    
    P.S: check that the terminal activated the environment. Usually you should see the name of the environment at the beggining of the command prompt, Like it is shown in the following picture:

    ![command_prompt](https://user-images.githubusercontent.com/27258035/234564451-b9e5dad9-926d-421c-87f7-59756e685081.png)


7. Install the requirements:

    <code>pip install -r requirements.txt</code>

If you want to use a later Ubuntu version please follow the [docker](#repository-setup-with-docker) instructions

### CARLA Setup

1. Open a new terminal without docker running. <code> ctrl + shift + t </code>
2. Run the [run_carla.sh](../run_carla.sh) script.
    <code>./run_carla.sh</code>

3. In this case the simulator will not open a new window, just stay running.

----
## Test that everything works

1. Run the [CARLA simulator](#carla-setup).
2. On Visual Studio Code run the docker container if you are using docker or activate the decision environment if you are using Anaconda.

3. Navigate to the PythonAPI/examples folder:
    
    <code>cd {Repository ROOT FOLDER}/Project/PythonAPI/examples</code>

4. Run [manual_control.py](../Project/PythonAPI/examples/manual_control.py)

    <code>python manual_control.py</code>

5. A new window with the simulator should open. On this window there should be a vehicle that you can control using your keyboard. Press **h** for more information on how to control the simulation.  
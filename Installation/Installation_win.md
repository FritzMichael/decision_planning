# Project Set Up Windows

## Set up

### Repository Setup
1. Install Visual Studio Code.
2. Install [Ananconda](https://docs.anaconda.com/free/anaconda/install/windows/).
3. Open **Anaconda Prompt** and type:
    
    <code>conda init cmd.exe</code>
4. Open Anaconda and create a new environment called **decision** with python **3.7** (IMPORTANT).
5. Open Visual Studio Code in the root of this repository.
6. Open a new terminal and type:   

    <code>conda activate decision</code>
    
    P.S: check that the terminal activated the environment. Usually you should see the name of the environment at the beggining of the command prompt, Like it is shown in the following picture:

    ![command_prompt](https://user-images.githubusercontent.com/27258035/234564451-b9e5dad9-926d-421c-87f7-59756e685081.png)


7. Install the requirements:

    <code>pip install -r requirements.txt</code>

### CARLA Setup

1. Download the simulator [CARLA 0.9.10](https://carla-releases.s3.eu-west-3.amazonaws.com/Windows/CARLA_0.9.10.zip)
2. Decompress the file in a directory of your preference.
3. Enter the decompressed folder, open a new terminal and type:

    <code>.\CarlaUE4.exe -quality-level=Low </code>

4. The simulator should open a windows like the one shown if the following image.

![carla](https://user-images.githubusercontent.com/27258035/234566270-f40a6ee6-aff7-473c-b1bc-2cfe2d983eee.png)

----
## Test that everything works

1. Run the CARLA simulator on [**Low Level quality**](#carla-setup).
2. On Visual Studio Code open a new terminal and activate your **decision** environment.

    <code>conda activate decision</code>

3. Navigate to the PythonAPI/examples folder:
    
    <code>cd {Repository ROOT FOLDER}/Project/PythonAPI/examples</code>

4. Run [manual_control.py](../Project/PythonAPI/examples/manual_control.py)

    <code>python manual_control.py</code>

5. A new window with the simulator should open. On this window there should be a vehicle that you can control using your keyboard. Press **h** for more information on how to control the simulation.  
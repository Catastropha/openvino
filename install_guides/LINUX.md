## Linux install

1. Go to https://software.seek.intel.com/openvino-toolkit?os=linux complete the form and click Submit

2. Click on Full Package to download OpenVINO

3. `cd Downloads/` - cd to folder where the file was downloaded. By default, the file is saved as l_openvino_toolkit_p_<version>.tgz

4. `tar -xvzf l_openvino_toolkit_p_<version>.tgz` - unpack. The files are unpacked to the l_openvino_toolkit_p_<version> directory

5. `cd l_openvino_toolkit_p_<version>` - cd to l_openvino_toolkit_p_<version> directory 

6. `sudo ./install_GUI.sh` - launch the installation GUI

7. Click Next to install. The installation directory will be `/opt/intel/openvino_<version>/`

8. `cd /opt/intel/openvino/install_dependencies` - cd to this folder to install dependencies

9. `sudo -E ./install_openvino_dependencies.sh` - install dependencies

10. `source /opt/intel/openvino/bin/setupvars.sh` - activate environment variables, or save this line in .bashrc file to always have them activated

11. `cd /opt/intel/openvino/deployment_tools/model_optimizer/install_prerequisites` - cd to this folder to install prerequisites

12. `sudo ./install_prerequisites.sh` - install prerequisites, or install for each framework separately for example `sudo ./install_prerequisites_mxnet.sh`

13. (Optional) `cd /opt/intel/openvino/deployment_tools/demo` - cd to this folder to run a demo for verification

14. (Optional) `./demo_security_barrier_camera.sh`




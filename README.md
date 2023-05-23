# ComfyUI Manager

# Installation

1. cd custom_nodes
2. git clone https://github.com/ltdrdata/ComfyUI-Manager.git
3. Restart ComfyUI

# Changes

* **V0.6** Support extension installation for missing nodes.
* **V0.5** Removed external git program dependencies.


# How To Use

1. Click "Manager" button on main menu

![mainmenu](misc/main.png)


2. If you click on 'Install Custom Nodes' or 'Install Models', an installer dialog will open.
![menu](misc/menu.png)

* When the 'Use local DB' feature is enabled, the application will utilize the data stored locally on your device, rather than retrieving node/model information over the internet

3. Click 'Install' or 'Try Install' button.

![node-install-dialog](misc/custom-nodes.png)

![model-install-dialog](misc/models.png)

* Installed: This item is already installed.
* Install: Clicking this button will install the item.
* Try Install: This is a custom node of which installation information cannot be confirmed. Click the button to try installing it.


# Custom node support guide

* Currently, the system operates by cloning the git repository and sequentially installing the dependencies listed in requirements.txt using pip, followed by invoking the install.py script. In the future, we plan to discuss and determine the specifications for supporting custom nodes.

* Please submit a pull request to update either the custom-node-list.json or model-list.json file.

# Support of missing nodes installation

![missing-menu](misc/missing-menu.png)

* When you click on the ```Install Custom Nodes (missing)``` button in the menu, it displays a list of extension nodes that contain nodes not currently present in the workflow.

![missing-list](misc/missing-list.png)

* Currently, support is only provided for extension nodes that can be installed in the form of "git-clone".



# TODO: Unconventional form of custom node list

* https://github.com/bmad4ever/ComfyUI-Bmad-Custom-Nodes
* https://github.com/diontimmer/Sample-Diffusion-ComfyUI-Extension


# Roadmap

* installation from git url
* 3rd party repository
* category/keyword filter
* Specification of custom nodes
* Specification scanner
* Search extension by node name
* Automatic recognition of missing custom nodes
* Automatic installation suggestion of missing custom nodes
* workflow downloader

# Disclaimer

* This extension simply provides the convenience of installing custom nodes and does not guarantee their proper functioning.
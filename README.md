# HoudiniToolkit

A collection of custom Houdini scripts, tools, and Houdini Digital Assets (HDAs) designed to streamline workflows, automate processes, and enhance productivity for VFX artists. This repository includes various utilities that simplify common tasks in Houdini, improving the efficiency of production and previs pipelines.

---

## Key Tools & Features

### 1. **Texture Assigner (HDA)**  
An HDA for browsing and assigning textures directly from **PolyHaven** using a **PySide-built GUI** in Houdini.

**Features**:
- Browse and assign textures directly from PolyHaven.
- Automates texture downloading, UV setup, and material assignment.
- Supports resolutions from 1k to 8k in formats like PNG, JPG, and EXR.
- Ideal for quick iterations and previs workflows.
- Provides an intuitive interface for easy texture management.
- **PolyHaven Public API Integration**: Uses the PolyHaven API to retrieve textures and materials in a variety of formats.

#### **Usage**:
1. Load the HDA into Houdini.
2. Select a texture from PolyHaven via the HDA interface and PySide GUI.
3. Apply it to your geometry with automated UV and material setup.
4. Customize resolution and format as needed.

#### **Installation**:
1. **Download the HDA** file from this repository.
2. Place the HDA file in Houdini's `OTL` folder or another directory of your choice.
3. In Houdini, go to the **Tab Menu** and select the HDA to load it.
4. Follow the usage instructions to assign textures from PolyHaven to your geometry.

---

### 2. **Prefix Manager (Script)**  
A user-friendly PySide2-based tool for managing node prefixes in Houdini.

**Features**:
- Assign new prefixes to selected nodes.
- Change an existing prefix while keeping the rest of the node name intact.
- Undo recent changes to revert node names.
- Input validation for alphanumeric characters and underscores.
- Real-time status feedback for successful or failed operations.

#### **Usage**:
1. Select the nodes in Houdini.
2. Enter the desired prefix.
3. Choose the action: assign or change prefix.
4. Click "Add Prefix" to apply changes.
5. Use "Undo" to revert changes if needed.

#### **Installation**:
1. Download the script file from the repository.
2. Create a new shelf tool in Houdini.
3. Edit the new tool and add the script in the python module under the script tab.

---

### 3. **Import SOP Assets to Karma (Script)**
A GUI tool designed to simplify scene setup for Karma rendering workflows in Houdini.

#### Features
- Import scene assets into Karma with multiple modes:
  - **All Together**: Imports everything at once.
  - **By Category**: Separates geometry, lights, and cameras.
  - **By Node/Prefix**: Filters imports based on selection or prefix.
- Scene graph path management with duplicate import detection.
- Automates creation of **Scene Import** and **Merge** nodes for Karma.

#### Usage
1. Launch the tool and specify the **Scene Graph Path**.
2. Choose the desired import mode.
3. Click **Create Karma Setup** to generate the nodes in the LOP network.
4. Verify the imported assets in Karma.

#### Installation
1. Download the script file from the repository.
2. 2. Create a new shelf tool in Houdini.
3. Ensure Karma and LOPs are enabled in your Houdini session.
3. Edit the new tool and add the script in the python module under the script tab.

---

## Prerequisites
- **Houdini** (with Karma rendering support for relevant tools).
- **PySide2** (for GUI-based scripts).

---

## Contribution
Contributions are welcome! Feel free to submit pull requests or raise issues for any suggestions or bugs.

---

## Acknowledgments
- **PolyHaven** for their open-access library and public API.
- The Houdini community for inspiring innovative tools and workflows.


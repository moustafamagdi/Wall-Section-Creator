# Introducing the Ultimate Wall Section Creator for Revit

Tired of the repetitive, time-consuming task of creating individual section views for every wall in your project? Need to generate dozens of sections for documentation, detailing, or coordination?

Our new **Wall Section Creator** add-in for Revit is a powerful tool designed to automate this entire workflow. With a rich user interface, it gives you complete control over every aspect of the section, from geometry and naming to advanced handling for linked models and curved walls.



![Addin User Interface](https://raw.githubusercontent.com/moustafamagdi/Wall-Section-Creator/refs/heads/main/UI.png) 


## Key Features at a Glance

- **Batch Creation**: Select multiple walls at once and generate all their sections in a single operation.
- **Full UI Control**: A user-friendly window to pre-configure all your settings.
- **Linked Model Support**: Create sections for walls located in linked Revit models just as easily as those in the host project.
- **Advanced Curved Wall Handling**: Choose to skip, create a single tangent section, or automatically segment curved walls into multiple, manageable sections.
- **Flexible Naming Conventions**: Automatically name sections with a prefix and number, or base the name on the wall's type.
- **Smart Geometry**: Precisely control section depth, width, height, and offsets.
- **Template Integration**: Apply your office's standard view templates automatically upon creation.
- **Persistent Settings**: The add-in remembers your last-used settings, saving you setup time on your next use.

## How to Use the Wall Section Creator: A Step-by-Step Guide

### Step 1: Download and Install the Tool

To get started, download the **Wall Section Creator** add-in for Revit by clicking the link below:

[Download Wall Section Creator](https://github.com/moustafamagdi/Wall-Section-Creator/raw/refs/heads/main/Wall%20Section%20Creator.exe)

After downloading, run the installer and follow the on-screen instructions to install the tool.

### Step 2: Launch the Add-in

1. Navigate to the **MM Tools** tab in the Revit ribbon.
2. In the **Modeling Tools** panel, click the **Wall Sections** button.
3. The **Wall Section Creator** window will appear. You must be in a **Plan View** to run the tool.

### Step 3: Configure Your Sections

The interface is organized into four main groups. Let's go through each option:

#### Section Visual Properties & Dimensions

- **Section Type**: Choose which Revit View Family Type to use for the new sections (e.g., "Building Section," "Wall Section").
- **View Template**: Apply a pre-existing View Template from your project. Select this if you don't want to apply a template.
- **Section Offset (mm)**: The distance the section line will be placed away from the wall's location line.
- **Far Clip Offset (mm)**: The depth of the section view. Note: This can be overridden by the selected View Template.
- **Horizontal Padding (mm)**: Adds extra width to each side of the section view's crop box, beyond the wall's length.
- **Vertical Padding (mm)**: Adds extra height to the top and bottom of the section's crop box.

#### Section Height

This controls which walls you can select and allows you to filter out small segments.

- **Select Walls From**: Choose which walls to generate sections from.
- **Filtering**: Defines how the new section views will be named in the Project Browser:
  - **Prefix + Number**: The standard option.
  - **Based on Wall Type Name**: The section name will be derived from the name of the wall's type.

#### Curved Wall Handling

This provides powerful options for dealing with arc-shaped walls.

- **Skip Curved Walls**: The tool will simply ignore any selected walls that are curved.
- **Create Single Section (Tangent)**: Creates one section view that is tangent to the midpoint of the wall's arc.
- **Create Multiple Sections per Wall**: This is the most advanced option. It divides a single curved wall into multiple straight segments and creates a section for each.

### Step 4: Create the Sections

After configuring all your settings, click the big blue **Create Sections** button.

1. The window will hide, and Revit will prompt you to select walls based on the mode you chose in Step 2.
2. Select the walls you want to process and click **Finish** on the Revit options bar.
3. The add-in will run through your selection, creating a section for each valid wall or segment.

A summary message will appear, telling you how many sections were successfully created and how many were skipped.

# Process Workflow

# Dependencies
- Pegasus v5.0+
- Python 3.6+

![process-workflow](https://github.com/user-attachments/assets/26959fb8-8d17-47d3-85e0-9d93a9c6a547)

# File Description

<b>plan.sh:</b> Consists of all commands to be executed to run the workflow. Takes care of planning the pegasus workflow and initialising where the input files are and where output files should be located after execution of workflow.

<b>workflow_generator.py:</b> Creates the abstract workflow, the replica catalog, the transformation catalog, and the site catalog. It has one job: ls This is used to invoke the executables which are present in bin folder.

<b>Input Folder:</b> Contains all the input files to be used in the workflow.

# How to run the workflow?
```
# Plan and run the workflow generator to create an abstract workflow for the given input files
./workflow_generator.py
./plan.sh workflow.yaml
`````

# Flow2Python Desktop App
Flow2Python is an educational desktop application that helps learners construct algorithms visually using flowcharts, then view the converted results as Python code. Built with React.js and packaged as a desktop application, it allows users to design algorithmic flows on a canvas, eliminating the need to write all the code manually from scratch.

## Download and install on Windows
The release available in this distribution folder is Flow2Python 1.0.0 for 64-bit Windows. Choose one of the following files:

- Flow2Python Setup 1.0.0.exe — recommended installer. This file is roughly 137 MB.
- Flow2Python 1.0.0.exe — portable version; run it directly without an installation process.

## Usage tutorial
### 1. Creating a flowchart
- Open Flow2Python. The canvas is in the center, the symbol palette is on the left, and the code panel is on the right.
- Drag Start onto the canvas to begin the algorithm.
- Add the needed symbols. For example, use Input to receive data, Process for calculations, Decision for branching, Output to display results, and End to finish the flow.
- Click a symbol you want to change, then adjust its value in the Properties panel.
- Connect the connection points between symbols so the flow can be followed. For Decision, connect both branches for true and false conditions, and make sure both lead to the right next step.
- Adjust the view with the zoom controls or minimap if the diagram is large. Check the validation indicator above the canvas and fix the flow if the diagram is not yet valid.

### 2. Viewing and running code
- Watch the Python Code panel. The code updates based on the flowchart you build.
- Click Run to execute the program. View messages or results in the Console panel, and enter values when the program asks for input.
- If the output does not match expectations, recheck symbol values, connections, and decision branch directions, then run again.

### 3. Practice example: checking even or odd numbers
- Select Load Example... and load the sample if it is available.
- Follow the algorithm pattern: Start → Input number n → Decision with condition n % 2 == 0.
- Connect the true branch to the output "Even" (or "Genap" as in the original sample), and the false branch to the output "Odd" (or "Ganjil"). Connect both branches back to End.
- Inspect the generated code. Conceptually, the condition becomes if n % 2 == 0, producing different outputs for the true and false branches.
- Click Run, enter a number, and observe the result in Console.

### 4. Saving or sharing your work
- Click Export JSON to save a diagram so you can reopen or continue it later with Import JSON.
- Click Copy Python to copy the code to the clipboard, or Download .py to save the code as a .py file.
- JSON files store the diagram to reopen in Flow2Python; .py files contain code to study or run in a Python environment.

### 5. Editing a diagram
- New starts a fresh diagram.
- Undo reverts the last change, while Redo reapplies a reverted change.
- Select any symbol on the canvas to edit its properties or rearrange the flow.

### Tips for students and instructors
- Start with simple algorithms: sequential steps, input-output, then branching and loops.
- Make sure every flow has a Start and End, and every decision branch has a clear destination.
- Compare the flowchart against the Python code rather than just copying what is generated. Notice how conditions and execution order translate.
- Test multiple input values—including boundary cases—so different branches are checked.
- Save JSON diagrams for assignments or continued practice. Share .py files when the resulting code is what is needed.

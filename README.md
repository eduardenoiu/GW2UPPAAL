# GW2UPPAAL: Combining Model-Based Testing and Automated Analysis of Behavioural Models using GraphWalker and UPPAAL

![markus-spiske-cjOAigK9xo0-unsplash](https://user-images.githubusercontent.com/7644735/223975735-e3255482-cbb7-49c6-9a89-7495f02a5b83.jpg)

Please follow the below instructions:

1. Use the ToolOutput folder as the folder  where the UPPAAL models will be exported.
2. Navigate to ToolOutput folder and open terminal/comman prompt.
3. type the command: java -jar GW2UPPAAL.jar [path to out-put file folder] [name of the output file that tester wants togive] [path to input GW JSON file] [Name of the JSON filethat the tester wants to transform] .(Remove square brackets and provide the path with //)

GW2UPPAAL: Hybrid Model-Based Testing and Analysis Tool
Overview
GW2UPPAAL bridges the gap between model-based testing (MBT) and model checking by integrating GraphWalker and UPPAAL. It automates the transformation of GraphWalker models into UPPAAL-compatible models for verification and test case generation. This hybrid approach ensures efficient analysis of behavioral models and helps validate requirements early in the development lifecycle.

Key Features
Automated Model Transformation: Converts GraphWalker JSON models into UPPAAL XML models.
Property Verification: Checks reachability, deadlock, and other properties using UPPAAL.
Model Confidence: Facilitates analysis and refinement of test models before test generation.
User-Friendly: Simplifies the verification process with automated query generation for UPPAAL’s verifyta.
Quick Start
1. Clone the Repository
bash
Copy code
git clone https://github.com/your-repo/GW2UPPAAL.git
cd GW2UPPAAL
2. Prepare Your GraphWalker Model
Design your model in GraphWalker Studio.
Export the model as a JSON file.
3. Run GW2UPPAAL
Transform the GraphWalker model into an UPPAAL-compatible XML format:

bash
Copy code
java -jar GW2UPPAAL.jar --input your_model.json --output output_model.xml
4. Analyze in UPPAAL
Import the output_model.xml into UPPAAL.
Use verifyta for automatic property verification:
bash
Copy code
verifyta output_model.xml

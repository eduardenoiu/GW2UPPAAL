# GW2UPPAAL: Combining Model-Based Testing and Automated Analysis of Behavioural Models using GraphWalker and UPPAAL

![markus-spiske-cjOAigK9xo0-unsplash](https://user-images.githubusercontent.com/7644735/223975735-e3255482-cbb7-49c6-9a89-7495f02a5b83.jpg)

GW2UPPAAL integrates GraphWalker and UPPAAL to enable a seamless combination of model-based testing (MBT) and model checking. This tool automates the transformation of GraphWalker models into UPPAAL-compatible formats for efficient verification and test case generation. By bridging the gap between testing and analysis, GW2UPPAAL helps developers validate requirements and improve model accuracy early in the development lifecycle.

Please follow the below instructions:

1. Use the ToolOutput folder as the folder  where the UPPAAL models will be exported.
2. Navigate to ToolOutput folder and open terminal/comman prompt.
3. type the command: java -jar GW2UPPAAL.jar [path to out-put file folder] [name of the output file that tester wants togive] [path to input GW JSON file] [Name of the JSON filethat the tester wants to transform] .(Remove square brackets and provide the path with //)

Commands needed:
git clone https://github.com/your-repo/GW2UPPAAL.git
cd GW2UPPAAL
java -jar GW2UPPAAL.jar --input your_model.json --output output_model.xml
verifyta output_model.xml

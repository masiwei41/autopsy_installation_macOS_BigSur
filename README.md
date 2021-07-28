# autopsy_installation_macOS_BigSur
The problems and solutions

autopsy dependencies:

follow the instructions:
https://slo-sleuth.github.io/tools/InstallingAutopsyOnMacOS.html

Notes:
To uninstall Java completely:
sudo rm -rf /Library/Internet\ Plug-Ins/JavaAppletPlugin.plugin  
sudo rm -rf /Library/PreferencePanes/JavaControlPanel.prefPane  
sudo rm -rf /Library/Application\ Support/Oracle/Java/ 
sudo rm -rf /Library/Java/JavaVirtualMachines 

For MacOS Big Sur, to install the full version of Liberica JDK 8, use
% brew install --cask liberica-jdk8-full

Problem when run bin/autospy: Cannot find java Please use the --jdkhome switch.
Solution: In the bin/autospy file, add  ' jdkhome="$JAVA_HOME" ' in line 83 or earlier.





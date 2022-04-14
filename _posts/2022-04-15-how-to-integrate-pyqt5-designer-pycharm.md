---

layout: post  
title:  "How to Integrate Qt Designer with PyCharm ?"  
author: rahul  
categories: [BLOG]  
image: assets/images/designer.jpg  
tags: [featured]  

---

**PyQt** is one of the most commonly used toolkit for making GUI (Graphical User Interface) based programs in python. You can use Qt Designer tool to easily make GUIs using drag and drop functionality. After you design your GUI using QT Designer , you will get a .ui file which you can convert to .py using pyuic5. It is sometimes a little bit of hassle to do all this. Luckily for us there exists a much easier way to do all this using PyCharm.

PyCharm is one of the most famous python IDEs and it has both free and a paid version. You can get PyCharm from [Get PyCharm](https://www.jetbrains.com/pycharm/download/#section=windows)

First of all, lets start with installing PyQt5 and PyQt5-tools which contains the Qt designer and other necessary things.

To install pyqt5, open command prompt and run **pip install pyqt5 pyqt5-tools** 

After pyqt5 and pyqt5-tools is successfully installed, we can proceed to the next step that is configuring designer and pyuic as external tools in pycharm. For that open pycharm and go to file --> settings --> tools --> external tools.

![pycharm settings window](https://www.rahulvk.com/assets/images/pycharm-settings.jpg)

Click on the plus button to add a new tool.

Fill in the details as follows:

- Name: QTdesigner
- Program: <write the path to your python installation folder here>\Scripts\pyqt5-tools.exe
- Arguments : designer
- Working directory: $ProjectFileDir$

Now click on ok and again press the plus button to add the next tool that is pyuic which we will use to convert our designer ui files to python .py files.

![adding pyuic as external tool](https://www.rahulvk.com/assets/images/pyuic.jpg)

Fill in the details as follows

- Name : PyUIC
- Program: <your python installation folder>\Scripts\pyuic5.exe
- Arguments: -x $FileName$ -o $FileNameWithoutExtension$.py
- Working directory: $ProjectFileDir$

That's it. We have configured pyqt5 designer and pyuic as tools in pycharm.

Now to create a new gui , just go to designer tool

![using designer tool from pycharm](https://www.rahulvk.com/assets/images/designertool.jpg)

And the designer window will open

![designer window](https://www.rahulvk.com/assets/static/images/designer.jpg)

create your UI and then click on save as and save the file with .ui extension.

After that you can see the .ui file you saved on your pycharm project window.

Just right click on the file select external tools --> PyUIC.

![converting .ui to py](https://www.rahulvk.com/assets/images/converttopy.jpg)

You will see a python file with the same name as the .ui file on your pycharm window. 

![python code for gui](https://www.rahulvk.com/assets/images/pythonfile.jpg)

You can modify that python file to add functionality to the GUI just created.

 


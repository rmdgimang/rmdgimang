..projectviwsbot.//
#Selenium Webdriver must be installed for this to work
import time;
from PyQt5 import QtWidgets
from PyQt5 import QtGui
from PyQt5.QtWidgets import QApplication, QMainWindow
import sys
from selenium import webdriver;
#application
def window():
    def runBot():
        #time to refresh page (seconds)
        Timer = 30
        Timer = int(timeInput.text())

        #youtube link
        link = linkInput.text():
@@ -40,6 +40,13 @@ def runBot():
    linkInput./UCGToazTIgmw9GbF_tu8nUzA<>
    linkInput.move(100, 25)

    timeLabel = QtWidgets.QLabel(win)
    timeLabel.setText("WatchTime(seconds)")
    timeLabel.move(15, 45)
    timeInput = QtWidgets.QLineEdit(win)
    timeInput.setGeometry(40, 10, 40, 20)
    timeInput.move(140, 55)

    runBotBtn = QtWidgets.QPushButton(win)
    runBotBtn.setGeometry(60, 270, 180, 40)
    runBotBtn.move(65, 80)       
    runBotBtn.setText("RUN VIEWBOT")
    runBotBtn.clicked.connect(runBot)
    win.show()
    sys.exit(app.exec_())
window()def check_and_log(method, self,

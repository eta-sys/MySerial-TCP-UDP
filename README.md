
# MySerial TCP UDP
=======

   MySerial can help you in develop and test of your devices. It offers to you Serial Port, TCP Client and Server, UDP Client and Server Channels. As Client you may use plain IP or DNS name.
   
   MySerial can be downloaded from http://ftp.eta-sys.net/MyNewSerial where actual version hosts. Using it is very easy. No 'Help' required - just hover the mouse over the box you want and a brief message will appear.
   
   You can send plane text, hex, files and files line by line (after each row waits any response). 
   
   You are in able to set control chars sequence at row end.
   
   You can see all the data in hex, which is very helpful when some extra or missing unprintable chars present in a message. You don't have to type your message 'in hex', but the whole dialogue will be presented 'in hex' in main ListBox.
   
   You can capture your whole session to one text file and explore it when it is convenient to you. Just right-click in main ListBox.
   
   You may use program as a RS protocol recorder, using both channels just Rx wires tied to data-line.
   
   To send a hex value 1A type '0x1a' including '..'. Note that when you put a control char to the end of your message, the delimiter you set (CR or CRLF) will be omitted!
   
      for example: AT'0x1a' will send hex "41541A".
      
   To repeat an already send message, select appropriated TextBox to desired channel then use Up and Down Arrows to find it and press 'ENTER'.
   
Right clicking on channel's text box you have options to send a as whole file or row-by-row. The last one means that after sending a row the program will wait any responce from device to send the next row of the file. This is very useful when sending a sequence of AT commands to initialise a device. You can put them in a text file.
   
      for example, AT commands to initialize a GSM module like SIM800
	    AT
	    ATE0
	    AT+CMEE=0
	    AT+CPBS="SM"
	    AT+CLIP=1
	    AT+CMGF=1
	    AT+CSMS=0
	    AT+VTD=1
	    AT+CLTS=1
	    AT+CHFA=1
	    AT+CLVL=90
	    AT+CMIC=1,11
	    AT+SIDET=1,11
	    AT+CMGDA="DEL ALL"
	    AT+MORING=1
	    AT+DDET=1,250,0,0
  
  Right click on main List box and you are given the options to capture whole dialog or only the received data to a file.
  
   Svetlin
 

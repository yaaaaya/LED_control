# LED_control
**### Overview**
To control the LED using Bolt Cloud

**Things used in this product:**
The Bolt Wifi module

1 x 330 ohm Resistor

1 x LED

**Steps for building the product**
_Hardware connections:_
Step 1: Take one leg of the resistor and wrap it around the longer leg of the LED i.e positive leg.
Step 2: Insert the negative leg of the LED into the ground pin of the Bolt.
Step 3: Insert the other leg of the resistor in digital pin 0 of the Bolt.
Step 4:Connect the device to bolt cloud.

Code in js
singleButton({name:"Led On", action:"digitalWrite", 
              pin:"0", value:"HIGH",bgcolor:"green",
              shape:"rectangle",align:"left","text_color":"white" })

singleButton({name:"Led Off", action:"digitalWrite", 
              pin:"0", value:"LOW", bgcolor:"red",
              shape:"rectangle", align:"left", text_color:"black"})

singleButton({name:"Fan On", action:"analogWrite", 
              pin:"0", value:"230",bgcolor:"#ffa500",
              shape:"circle", align:"right","text_color":"white" })

singleButton({name:"Fan Off", action:"analogWrite", 
              pin:"0", value:"0",bgcolor:"#6a5acd",
              shape:"circle", align:"right", text_color:"white"})

Code in html:
<!--<!DOCTYPE html>-->
<!--<html>-->
<!--    <head>-->
<!--        <title>Bolt IoT Platform</title>-->
<!--        <script type="text/javascript" src="https://cloud.boltiot.com/static/js/boltCommands.js"></script>-->
<!--        <script>-->
<!--        setKey('{{ApiKey}}','{{Name}}');-->
<!--        </script>-->
<!--    </head>-->
<!--    <body>-->
<!--        <center>-->
<!--        <button onclick="digitalWrite(0, 'HIGH');">ON</button>-->
<!--        <button onclick="digitalWrite(0, 'LOW');">OFF</button>-->
<!--        </center>-->
<!--    </body>-->
<!--</html>-->

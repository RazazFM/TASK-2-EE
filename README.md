
### Arduino Auto Switch Off

As we know Arduino have only limited output voltage and current from its pins.

So when we want to control a motor or a bulb we need to first control a relay to control that bulb or motor.

But also the relay coil draws relativily high current from that Arduino can supply.

#### That’s why we use the NPN transistor as a switch !

as we know Arduino cannot control high power devices it only supplies 5 volts with limited current, so we use relays in between to control motors and bulbs with a high voltage.

this relay cannot be directly controlled from Arduino because it throws current from its coil, now we know it only supplies 5 voltage with limited current, so we use that transistor NPN as a switch, this is the emitter base and collector we use it as a switch between the Arduino and the relay base

It is directly controlled by the Arduino output pin so it rings he 5 voltage to the relay terminal to control it’s open and close, let’s see how this circuit work this is the code here we can see that it has the code to control the pin button number 8 to take the action from the pin button.

as we have seen in the previous posts this relay the output pin number 2 it starts with the state relay low and a state button, this uses the bounce to to filter the input from the button and it makes some delay in between>

so let’s start the emulation and see how it’s working, let’s press Start simulation and find that there are three volts coming to the Bulb and controlled by the relay which is controlled by that transistor controlled by the Arduino>

let’s press the button then bulb lights on we can see high current and then pours off let’s see it again it’s powered up then it’s powered down t’s powered up then powered down .

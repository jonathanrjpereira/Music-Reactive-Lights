# Music Reactive LEDs
LED lights that are controlled by music levels.

**Order PCB:** []()

## Electronic Components
| Qty | Component | Buy |
| ------------- | ------------- | ------------- |
| 1 | Electret Condenser Microphone |[AliExpress](http://s.click.aliexpress.com/e/bSOOMYPe) |
| 1 | BC547 PNP Transistor |[AliExpress](http://s.click.aliexpress.com/e/bpL0Irsk) |
| 1 | 10KΩ Potentiometer |[AliExpress](http://s.click.aliexpress.com/e/bR23nRuG) |
| 2 | 1KΩ Resistor |[AliExpress](http://s.click.aliexpress.com/e/bh4eqrQs) |
| 3 | 5mm LED |[AliExpress](http://s.click.aliexpress.com/e/wuFpLXS) |
| 1 | 10uF Capacitor |[AliExpress](http://s.click.aliexpress.com/e/c9FHzl5W) |
| 1 | 0.1uF (100nF) Capacitor |[AliExpress](http://s.click.aliexpress.com/e/byQG0DZW) |
| 1 | 9V Battery Holder |[AliExpress](http://s.click.aliexpress.com/e/c3jbp72Y) |
| 1 | 9V Battery |[AliExpress](http://s.click.aliexpress.com/e/bbDirGHE) |
| 1 | PCB |[AliExpress](http://s.click.aliexpress.com/e/dhgwzKY) |


| Tools | Buy |
|--|--|
|Soldering Iron|[AliExpress](http://s.click.aliexpress.com/e/E83bSJI) |
|Soldering Wire|[AliExpress](http://s.click.aliexpress.com/e/PdhB0nm) |
|Mini PCB Hand Drill + Bits|[AliExpress](http://s.click.aliexpress.com/e/b93tomjI) |

## Working

![Music Reactive LED Block Diagram](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/BD.png)

The input of a Microphone is filtered through a Low Pass Filter. The filter will only allow certain frequencies at the output. The LEDs will only react to these filtered frequencies.

**Low Pass Filter:**

![Music Controlled LED Low Pass Filter](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/LPF.png)

A Low Pass Filter (LPF) will block all signals that are above it's Cutoff Frequency and allow only those signals that are below it's Cutoff Frequency.

The Cutoff Frequency can be set by selecting the passive components as follows: ![LPF](https://latex.codecogs.com/png.latex?f_%7Bc%7D%20%3D%20%5Cfrac%7B1%7D%7B2%5Cpi%20RC%7D)

## Circuit

![Music Controlled Reactive LED Circuit Schematic](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/sch.png)

The Electret Condenser Microphone has a frequency range between 100-10,000 Hz. The 10KΩ potentiometer can be varied to change the Cutoff Frequency of the Low Pass Filter.
For example, if the pot is set to 10KΩ, the Cutoff Frequency will be equal to 159Hz. Similarly if the pot is set to 100Ω the Cutoff Frequency will be equal to 15KHz.
The transistor BC547 acts as a switch which turns the LEDs ON.

![Music Controlled Reactive LED Circuit Board PCB](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/brd.png)

You can **Order the PCB:** []()

![Printable](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/printable.png)

Or you can printout the [PDF file](https://github.com/jonathanrjpereira/Music-Reactive-Lights/blob/master/img/printable.pdf) and make your own PCB using the [Iron-on method]().

## Contributing🛠
Are you an engineer or hobbyist who has a great idea for a new feature in this project? Maybe you have a good idea for a bug fix? Feel free to grab our code & schematics from Github and tinker with it. Don't forget to smash ⭐️ & the Pull Request button.

[![alt text][1.1]][1] [![alt text][2.1]][2] [![alt text][3.1]][3]

[1.1]: https://github.com/jonathanrjpereira/Social-Media-README/blob/master/youtube.png (YouTube)
[2.1]: https://github.com/jonathanrjpereira/Social-Media-README/blob/master/instagram.png (Instagram)
[3.1]: https://github.com/jonathanrjpereira/Social-Media-README/blob/master/github.png (GitHub)

[1]: https://www.youtube.com/channel/UCRW-41O1vy98KKgJRQoYzdg
[2]: https://www.instagram.com/electroguruji/
[3]: https://github.com/jonathanrjpereira

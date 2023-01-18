<b>ESP32-HOMEKIT</b>

Apple HomeKit Accessory Server Library for IDF V5.0. Developing apps and accessories for the home.Let people communicate with and control connected accessories in their home using your app. With the HomeKit or Matter framework, you can provide users the ability to configure accessories and create actions to control them. Group those actions together into powerful automations and trigger them using Siri.
<br>
<br>
<b>WORKS WITH APPLE HOME BADGE</b>

<img  style="float: right;" src="https://github.com/AchimPieters/ESP32-SmartPlug/blob/main/images/works-with-apple-home.svg" width="150">

The Works with Apple Home badge can be used to visually communicate that your accessory is compatible with the Apple Home and Siri on Apple devices. If you plan to develop or manufacture a HomeKit accessory that will be distributed or sold, your company needs to be enrolled in the MFi Program.


See [esp32-homekit-demo](https://github.com/AchimPieters/esp32-homekit-demo) for examples.
<br>
<br>
<sub><sup>-------------------------------------------------------------------------------------------------------------------------------------</sup></sub>
<br>
<br>
<b>QR CODE PAIRING</b>

You can use a QR code to pair with accessories. To enable that feature, you need to configure accessory to use static password and set some setup ID:
```
homekit_server_config_t config = {
    .accessories = accessories,
    .password = "123-45-678",
    .setupId="1QJ8",
};
```
<b>GENERATE QR CODE</b>

Then you need to generate QR code using supplied script:

tools/gen_qrcode `5` `123-45-678` `1QJ8` qrcode.png


| <sup><b>HOMEKIT ACCESSORY CATEGORY</b></sup> | <sup><b>NUMBER</b></sup> |
|----------------------------|--------|
| <sup>Other</sup>                      | <sup>1</sup>      |
| <sup>Bridges</sup>                    | <sup>2</sup>      |
| <sup>Fans</sup>                       | <sup>3</sup>      |
| <sup>Garage door openers</sup>        | <sup>4</sup>      |
| <sup>Lighting</sup>                   | <sup>5</sup>      |
| <sup>Locks</sup>                      | <sup>6</sup>      |
| <sup>Outlets</sup>                    | <sup>7</sup>      |
| <sup>Switches</sup>                   | <sup>8</sup>      |
| <sup>Thermostats</sup>                | <sup>9</sup>      |
| <sup>Sensors</sup>                    | <sup>10</sup>     |
| <sup>Security systems</sup>           | <sup>11</sup>     |
| <sup>Doors</sup>                      | <sup>12</sup>     |
| <sup>Windows</sup>                    | <sup>13</sup>     |
| <sup>Window coverings</sup>           | <sup>14</sup>     |
| <sup>Programmable switches</sup>      | <sup>15</sup>     |
| <sup>Range extenders</sup>            | <sup>16</sup>     |
| <sup>IP cameras</sup>                 | <sup>17</sup>     |
| <sup>Video door bells</sup>           | <sup>18</sup>     |
| <sup>Air purifiers</sup>              | <sup>19</sup>     |
| <sup>Heaters</sup>                    | <sup>20</sup>     |
| <sup>Air conditioners</sup>           | <sup>21</sup>     |
| <sup>Humidifiers</sup>                | <sup>22</sup>     |
| <sup>Dehumidifiers</sup>              | <sup>23</sup>     |
| <sup>Apple tv</sup>                   | <sup>24</sup>     |
| <sup>Speakers</sup>                   | <sup>26</sup>     |
| <sup>Airport</sup>                    | <sup>27</sup>     |
| <sup>Sprinklers</sup>                 | <sup>28</sup>     |
| <sup>Faucets</sup>                    | <sup>29</sup>     |
| <sup>Shower heads</sup>               | <sup>30</sup>     |
| <sup>Televisions</sup>                | <sup>31</sup>     |
| <sup>Target remotes</sup>             | <sup>32</sup>     |



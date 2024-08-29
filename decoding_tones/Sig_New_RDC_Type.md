## SDRSharp_20240702_210156Z_152353000Hz_AF

Sub-second eight-tone transmitter signal.

9 bursts of about 65ms sent back to back but only 8 tones are used maybe?.

Test TX button has 9 bursts with the length of about 32ms then a pause of 252ms then a long 1000Hz TX of about 3345ms.

If you trigger and hold a zone trigger it's about 11 seconds between a signal TX (device can be configured to use release as a trigger)

```
Signal consists of a sub second burst (total TX is just over half a second)

1_____2_____3_____4_____5_____6_____7_____8_____9
|     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |
|     |     |     |     |     |     |     |     |
765   687   1271  765   639   686   725   1548  1128
|     |     |     |     |     |     |     |     |
C     RV    RV    IDC   C     IDC   STV   RV    IDRV

C = Constant Hz

RV = Repeat Variable (changes when the same signal repeats without trigger reset) *not too sure about this

IDC = ID Constant

STV = Signal Type Variable 1553Hz=Test TX, 883Hz=Zone1, 740Hz=Zone2, 824Hz=Zone3, 690Hz=Zone4

IDRV = ID Repeat Variable (stays the same when signal burst repeats without trigger reset)


```

Example of newer signal

|Sig Pos|Tone Value|Time|
| :------------| :------------ | :------------ |
|1.|**765Hz**|*41ms*|
|2.|**687Hz**|*41ms*|
|3.|**1271Hz**|*41ms*|
|4.|**765Hz**|*41ms*|
|5.|**639Hz**|*41ms*|
|6.|**686Hz**|*41ms*|
|7.|**725Hz**|*41ms*|
|8.|**1548Hz**|*41ms*|
|9.|**1128Hz**|*41ms*|

|1.|data|*[asdad](link)*|

```
RAW DATA
1. 765 41ms
2. 687 41ms
3. 1271 41ms
4. 765 41ms
5. 639 41ms
6. 686 41ms
7. 725 41ms
8. 1548 41ms
9. 1128 41ms
```

## Links
- https://www.securitysa.com/regular.aspx?pklregularid=2595
- https://www.securitysa.com/regular.aspx?pklregularid=2680
- https://ludens.cl/Electron/fts8/fts8.html
- https://www.cl.cam.ac.uk/~sps32/mcu_lock.html
- http://sm0vpo.altervista.org/pic/ctcss_01.htm
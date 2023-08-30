- 👋 Hi, I’m @capoty
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
capoty/capoty is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<integervariable value-"g" variable-"iConnect" />
2
<integervariable value-"g" variable-"{Ret" />
3
«integervariable value-"g" variable-"{Size" />
4
«stringvariable value-"" variable="sBuf" /»
5
6
«display line-"0" column="g" message-"HTTP Post test" />
7
8
<! -- The preconnect command attempts to connect the device on Clou
g
«display line-"I" column-"g" message-"Connecting
" /
10
«preconnect variablestatus="$(iConnect)" />
11
12
<1-- Performs the transaction after connecting --»
13- <if variable="$(iConnect)" operator="iqual" value="g" >
14
<display line="1" column="0" message="Connected!" />
15
16
<!-- The content of the variable buffer should be hexadecimal.
17
below, the value 0123456789 is being sent. It is possible to use
18
string. tohex to convert any string to hexadecimal format, and t
19
use the command string. length to get the string size -->
20
21
<!-- In order to send data properly, it is necessary to send
22
at least 7 bytes to CloudWalk
23
24
«display Line-"3" column-"g" message-"Posting .
.." /
25
26
«stringvariable value-"0123456789" variable-"sBufsend" /»
27
<integervariable value-"g" variable-"iSzBufsend" /-
28
29
«string. tohex string-"$(sBufSend)" variablereturn-"$(sBufSend)
30
<string. Length value-"$(sBufSend)" variablereturn-"$(iSzBufsen
31
«network.send buffer="$(sBufSend)" size="$(iSzBufSend)* variat

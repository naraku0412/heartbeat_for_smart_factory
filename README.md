## heartbeat_for_smart_factory
### 0 Paper
### 1 Heartbeat frame struct

<table border="1" width="500px" cellspacing="10">
<tr>
  <th align="center">Byte number</th>
  <th align="center">Byte quantity</th>
  <th align="center">Typical values</th>
  <th align="center">Meanings</th>
</tr>
<tr>
  <td>0-1</td>
  <td>2</td>
  <td>0x57AB</td>
  <td>Lead code</td>
  <td rowspan="2" align="center">Frame Header 3 Bytes</td>
</tr>
<tr>
  <td>2</td>
  <td>1</td>
  <td>0xD5</td>
  <td>Delimiter</td>
</tr>
<tr>
  <td>3-8</td>
  <td>6</td>
  <td>0xFF FF FF FF FF FF</td>
  <td>Destination MAC address</td>
  <td rowspan="4" align="center">E II format 14 Bytes</td>
</tr>
<tr>
  <td>9-14</td>
  <td>6</td>
  <td>0xFF FF FF FF FF FF</td>
  <td>Source MAC address</td>
</tr>
<tr>
  <td>15</td>
  <td>1</td>
  <td>0x08</td>
  <td rowspan="2">Type IP 0x0800</td>
</tr>
<tr>
  <td>16</td>
  <td>1</td>
  <td>0x00</td>
</tr>
<tr>
  <td>17</td>
  <td>1</td>
  <td>0x45</td>
  <td>Protocol version</td>
  <td rowspan="10" align="center">IP header 20 Bytes</td>
</tr>
<tr>
  <td>18</td>
  <td>1</td>
  <td>0x00</td>
  <td>TOS(type of service)</td>
</tr>
</table>

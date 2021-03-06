Bip to Energymech
=================

This is a python script that converts the IRC logs generated by the [Bip IRC bouncer](http://bip.milkypond.org/) to the Energymech format used by [ZNC](http://wiki.znc.in/).

The reason for this converter is to enable logs generated by Bip to be used with [pisg](http://pisg.sourceforge.net/) for stats building.


How to use
----------

- Edit setup.cfg

<table border=1>
  <tbody>
    <tr>
      <th>Option name</th>
      <th>What does it do?</th>
    </tr>
    <tr>
      <td>input =</td>
      <td>contains the full path to the folder holding the <b>bip</b> IRC logs</td>
    </tr>
    <tr>
      <td>output = </td>
      <td>contains the full path of the folder where the <b>energymech</b> logs will be saved to</td>
    </tr>
  </tbody>
</table>

- Run convert.py

Release notes
-------------

1. **Version 1.2** searches for logs recursively; you can now have subfolders in the input folder. 

2. **Version 1.1** now supports bans and unbans.

3. **Version 1.0** doesn't know how to parse bans. If you happen to have a bip IRC log containing a ban and unband please let me know so I can update the script.
## Magic word
![Cover photo](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExanR0eHMyN3lpbjlva3Q4MDc3OHFlOGNnaWgxZmltbmNuZDJhaHVvdyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/5ftsmLIqktHQA/giphy.gif)

### Purpose
The purpose behind is to provide a fully showcasing example of how you can utilize goevil to create what could be a wiper being disguised

<b>Disclaimer: We take no liability of how you use it!</b>
<b>Disclaimer: Don't run this on your own machine! </b>

### What it does
1. Everything in the users Desktop directory is encrypted
2. The user is later prompted to enter a magic word
2a. Upon failure to enter the correct word, the screen is changed and a coundown appears on the screen
2b. Upon success the malware will decrypt all files and exit.

If the countdown in 2a reaches zero, the malware will delete itself and nuke the system.

The key needed to enter is `Isla Nublar`

<b>Note:</b> A SHA256 hash sum of the key can be seen in the source code of the website.

The ransomware will only work on a nix based system but can with ease be changed to work on windows aswell.

### Detection
The best way forward to detect it is to look for files that have the extension '.magic' in the Desktop directory.

As of 2023-07-20, virustotal has not detected the wiper as something malicious.
![Result](https://github.com/s9rA16Bf4/go-evil/blob/main/images/Virus_total_magic_word.png)

[Link to virustotal result](https://www.virustotal.com/gui/file/163dccd0033ba59f9702ae9310cd939e7144af6643470b1299918f1815a6604a?nocache=1)

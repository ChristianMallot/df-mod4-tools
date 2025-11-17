# DF Module 4 – Tools & Evidence Analysis  
Digital Forensics – Autopsy, Hex Editors, Simple Encryption, and Rainbow Tables  
Author: Christian Mallot

---

## ## Exercise 1 – Importing Known-File Hash Database (NSRL)

In this exercise, I downloaded the latest NSRL RDS set and imported it into Autopsy so the tool can automatically identify “known good” operating system files and reduce noise during investigations. This is essential for filtering out standard Microsoft and system binaries so investigators can focus on unknown or suspicious artifacts.

### ✔ Verification Screenshot  
![Exercise 1](A_screenshot_displays_Autopsy_version_4.21.0_runni.png)

---

## ## Exercise 2 – Creating a “Known Bad” Evidence Hash Set

I loaded the *InChap09.dd* disk image into Autopsy, located the suspicious files labeled **Special Project-A** (.jpg and .bmp), tagged them as notable, generated an Excel report, extracted their hashes, and created a new Known Bad hash set. This allows rapid detection of these same incriminating files on other systems.

### ✔ Verification Screenshot  
![Exercise 2](A_screenshot_of_Autopsy,_an_open-source_digital_fo.png)

---

## ## Exercise 3 – Hex Editor File Remnant Matching

To practice matching remnants of deleted files, I used a hex editor to examine the first sector of a document and compute a sector-level SHA-256 hash. This technique is useful when only fragments survive in unallocated space. Investigators can connect offenders to evidence even when full files are deleted.

### ✔ Verification Screenshot  
![Exercise 3](A_screenshot_of_FTK_Imager_software,_version_4.7.1.png)

---

## ## Exercise 4 – Simple Encryption (Vigenère Encode + Decode)

To simulate encryption used to hide evidence, I created an `evidence.txt` message, encoded it using Vigenère Cipher, saved the encrypted output as `nothing.txt`, and then decoded it back to `recovered.txt` using the same key.

This demonstrates how simple bit/character-shift encryption works and how investigators can reverse it to reveal hidden messages.

### ✔ Verification Screenshot  
![Exercise 4](A_screenshot_displays_CyberChef,_a_web-based_tool_.png)

---

## ## Bonus (Optional) – Rainbow Table Exploration

If completed, this section would demonstrate generating SHA-256 hashes for all numeric 6-digit passcodes, storing them in a rainbow table, and performing reverse lookup against the provided challenge hashes.

(If you complete it, add your screenshot here.)

---

## ## Notes & Skills Demonstrated

- Autopsy: hash set import, notable tagging, reporting, known-bad database creation  
- Hex Editor: sector-level hash analysis and remnant matching  
- CyberChef: encoding, decoding, and understanding simple encryption  
- GitHub: repo organization, version control, Markdown documentation  

---

## ## System Info

Evidence collected and all screenshots generated on my Windows workstation per module requirements.



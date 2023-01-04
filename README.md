# CTI Reports using TRAM

Threat Report ATT&CK Mapping (TRAM) is an open-source platform designed to advance 
research into automating the mapping of cyber threat intelligence reports to MITRE ATT&CK®. 
<a href="https://github.com/center-for-threat-informed-defense/tram/">TRAM Project</a>

---

### Catalog

| ID | Source | Topic |
|:--- | :---: |:--- |
| 1 | malwarebytes LABS | Woody RAT malware |
| 2 | | |
| 3 | | |

---

### Reports

- ```Report 1``` <a href="https://www.malwarebytes.com/blog/threat-intelligence/2022/08/woody-rat-a-new-feature-rich-malware-spotted-in-the-wild">ARTICLE</A>
Focuses on a newer RAT called Woody.
  * Final Notes (see TRAM report in *REPORTS* folder) - Given the responsibility, I can analyze more of this report, or similar reports for additional TTPs. Whether its Malware, APTs or some other attack vector, I can apply this workflow proactively to avoid a similar incident on business operations. 
  
---

### Report Details

```Report 1```

<p align="left">
Step 1 - Import an HTML format of article
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210481736-5838cfa3-cf2d-4bfd-9879-a93c5dc9a1e0.PNG" alt="import" style="width:100%">
TRAM queues the report and identifies relevant information to check for TTPs using MITRE ATT&CK. I will be stepping through each item here, mapping any findings
</p>

<p align="left">
Step 2 - Look for relevant TTPs
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210666065-2b264c87-8ea4-41a3-bebb-ed98d0cc74ff.PNG" style="width:100%">
Header and footer information gets imported so I will focus on medium to high confidence scores. If I feel a TTP deserves a higher score, I can use the MITRE ATT&CK navigator tool to investigate further
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210666406-8cb1953e-7e8b-4084-bbcd-8f2c8e2be610.PNG" style="width:100%">
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210666817-42ba835e-f3d5-466a-bb01-0f4214693828.PNG" style="width:100%">
  Adding an additional TTP for a detailed view of the application protocol
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210666434-5e05f4f0-82b6-415b-add6-9b931d2baa95.PNG" style=width="128" height="128">
  <div align="center">Justification for the add using the ATT&CK NAVIGATOR</div>
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210667298-1f79f612-81c2-439b-ad32-2e19bd6b4242.PNG" style="width:100%">
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210667307-53309953-71fc-4b15-ab83-a989f8ba642f.PNG" style="width:100%">
  <div align="center">Looking on the MITRE ATT&CK site for the low confidence TTP</div>
</p>

<p align="left">
Step 3 - Export findings
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210667586-f358db6a-4bf9-4a2c-8d5d-aa40bdb0f6c9.PNG" style="width:auto" height="256">
  <div align="center">TRAM exports either a .DOCX or .json file. It isnt very user friendly but it does identify the TTPs it thinks were in the CTI report. I prefer to use VS Code and the Att&ck extension. That allows for a more thorough check</div>
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210667599-8d63c5cc-5614-4ad5-b5e6-ec1f87c1a5bd.PNG" style="width:100%">
  The Att&ck extension allows me to type the TTP name and VS Code will identify its ID code
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210668257-dfe9cbe6-42c8-4149-86c1-52fd473bbfb7.PNG" style="width:100%">
  CTRL + spacebar turns the name into an ID with a summary
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210668426-2853b9b3-29e7-4eec-8196-987975be1c37.PNG" style="width:100%">
  You can type the ID directly in VS Code and use the CTRL + spacebar cmd to add TTPs. An additional cmd will show the summary prior to adding the ID
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210668619-1b0e035b-9da6-4195-b239-f32a34242bba.PNG" style="width:100%">
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/210668733-c465c95a-58d4-46c2-bfae-749723ff4141.PNG" style="width:auto" height="256">
  <div align="center">Right clicking on the ID will let me link directly to the MITRE ATT&CK site</div>
</p>

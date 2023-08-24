# USV-RWPS485-MetaHuman
This repository highlights my contributions to the University of Silicon Valley's RWPS485 Capstone Project 2 class.

The reason why I wanted to upload and showcase this project was that it challenged me in areas I never knew I would be challenged, certainly not in the academic sense. I was used to coding, as a computer science major would be. Yet, this project required minimal coding from my end and instead understanding implementation, documentation, employing logic, problem-solving, and most importantly teamwork.

## Documentation / Necessary Links
https://docs.metahumansdk.io/metahuman-sdk/reference/metahuman-sdk-unreal-engine-plugin/v1.6.0#audio-to-lipsync

https://metahumansdk.io/

https://www.unrealengine.com/en-US/metahuman?utm_source=BingSearch&utm_medium=Performance&utm_campaign=%7Bcampaigname%7D&utm_id=554356335&sub_campaign=&utm_content=&utm_term=metahuman%20unreal

Most of my progress was uploaded onto YouTrack, but I will summarize what I have uploaded onto Github.

- Converted MP4 recordings to WAV files for animation sequences and created lipsync animations for all metahuman responses.
- Compressed all animations to ensure optimal performance on slower machines.
- Implemented switch statements for all keywords and their respective animations/sounds in the blueprint and connected all those responses to an enum, ensuring they run when a response is selected.
- Organized and removed redundancies in the blueprint for better readability and maintainability.

The original audio files were screen recording mp4s in Zoom. To make them usable for the project and convert them to lipsync animations, I had to convert every file to `.wav` instead of `.mp4`.

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/7.png" alt="Image Description" width="700"/>

After converting the files, it was time to make lipsync animations from the said files. These were the settings used to make the animations and they remained consistent throughout the project.

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/1.png" width="700"/>
<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/3.png" width="900"/>

The animations were also compressed, even though there was little size difference, every bit of data counted to make this usable on lower-end machines

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/2.png" alt="Image Description" width="500"/>

After these animations were made, we now needed a way to output every single one. The solution was to use switch statements by using an enumerator to process keywords.

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/8.png" alt="Image Description" width="500"/>

This shows the enum being used in the level blueprint where the output is to play the metahuman animation and recording at the same time when a keyword is inputted into the switch statement.

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/4.png" alt="Image Description" width="900"/>

This can be an arduous process and can look something like this:

<img src="https://raw.githubusercontent.com/imjbassi/USV-RWPS485-MetaHuman/main/Images/6.png" alt="Image Description" width="900"/>

After that, we have working output and are free to designate any output we so choose!

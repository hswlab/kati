> **Warning**
> This app is based on the unofficial API BingChat. Unfortunately, sometimes BING updates can cause a broken communication with the AI. I will try to fix broken communication, if it can be fixed on my side, as soon as possible. :)

> **Info**
> If Bing does not respond, try starting a new conversation, removing the default behavior text from the settings or saving a new token.


# KATI-AI (bing Chat-GPT 4)
[![GitHub](https://img.shields.io/github/license/hswlab/kati)](https://github.com/hswlab/kati/blob/main/LICENSE) 
![GitHub issues](https://img.shields.io/github/issues/hswlab/kati)
[![Downloads](https://img.shields.io/github/v/release/hswlab/kati)](https://github.com/hswlab/kati/releases/latest) 
<!--
https://www.rarst.net/code/link-latest-github-release-binary
![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/hswlab/kati)
[![Downloads](https://img.shields.io/github/downloads/hswlab/kati/total)](https://github.com/hswlab/kati/releases/latest) 

<img src="https://img.shields.io/badge/dynamic/json.svg?label=download&url=https://api.github.com/repos/hswlab/kati/releases/latest&query=$.assets[0].name&style=for-the-badge" alt="download partial file" loading="lazy"> 
-->

KATI is an AI desktop chat application with bing Chat-GPT 4. It supports voice and visual emotion feedback of the AI. The goal of the development goes in the direction of J.A.R.V.I.S or HAL 9000. I imagine an application that is uncomplicated to set up and does not cost anything. Just download, launch and use. 

KATI is programmed with Electron and .NET6 and is therefore operating system independent. Currently only a download for Windows is offered, but there will probably also be an executable for Linux. The heart for the communication with the AI is the C# library [BingChat](https://github.com/bsdayo/BingChat). A detailed description of all features in KATI can be found in the user manual.
<a href="https://github.com/hswlab/KATI/blob/main/about-de.pdf">`User manual: German`</a> <a href="https://github.com/hswlab/KATI/blob/main/about-en.pdf">`User manual: English`</a>


[![GitHub release (with filter)](https://img.shields.io/github/downloads/hswlab/kati/total?style=for-the-badge&logo=ChatBot&label=download%20KATI
)](https://github.com/hswlab/kati/releases/latest)


*Key features of KATI:*
- [X] Conversation with the AI in the chat modes: Creative, Balanced or Direct
- [X] Optional voice output with a voice pre-installed in the operating system or a naturalsounding TikTok voice.
- [X] Optional speech input (System Speech & Whisper)
- [X] Dynamic avatar images to represent AI emotions.
- [X] Chat history with filter function, read-aloud function and the possibility to resume a previous conversation.
- [X] Rating option for the AI answers and filter history by rating
- [X] Storage option for a behavioral description of the AI and a salutation name. This information is automatically transferred to the AI when a new topic is created.
- [X] Short waiting times due to direct streaming of answers. Text and code are formatted for readability.
- [X] Multilingual user interface (DE, EN, FR, ES, PT, JA, KO)

![preview](https://github.com/hswlab/kati/blob/main/Screenshot.png)

![preview2](https://github.com/hswlab/kati/blob/main/Screenshot2.png)

![preview3](https://github.com/hswlab/kati/blob/main/Screenshot3.png)

# Nuget packages and associated licenses used in KATI
- BingChat <a href="https://github.com/bsdayo/BingChat/blob/main/LICENSE">`MIT License`</a>
- ElectronNET.API <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- Esprima <a href="https://licenses.nuget.org/BSD-3-Clause">`BSD 3-Clause License`</a>
- LiteDB <a href="https://www.nuget.org/packages/LiteDB/5.0.16/license">`MIT License`</a>
- Microsoft.AspNetCore.SignalR.Client <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- NAudio <a href="https://www.nuget.org/packages/NAudio/2.2.1/license">`License Info`</a>
- Newtonsoft.Json <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- System.Data.SQLite <a href="https://www.sqlite.org/copyright.html">`Public Domain`</a>
- System.Linq.Async <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- System.Speech  <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- SoundTouch <a href="https://www.surina.net/soundtouch/license.html">`License Info`</a>
- WhisperNet <a href="https://licenses.nuget.org/MPL-2.0">`MPL-2.0 License`</a>


# Next milestone (research)
- [ ] I want to try out a local AI, because I don't really like the user to handle with a bing token to get the chat running. Probably I try LLama or something which don't need an authentikation, can be used on weak PC's, don't need a complicated installation and is still for free. I'm not sure if I will be sattisfied with my resarch results, but if I am, there will be a new project similar to KATI but with an alternative AI. Maybe there is a solution to use the Bing chat outside of the Edge browser without a token. This has already worked from time to time, I do not give up hope :)

# Ideas for upcoming milestones
- [ ] Feature to convert text to audiofile (suno-ai/bark => PABannier/bark.cpp is a nice candidate. TikTok voice is also nice to use)
- [ ] Test OpenNlp for better recognition of sentence endings.
- [ ] Export/Import function for chat history
- [ ] Setting your own avatar image
- [ ] Management for alternative AI avatar packages
- [ ] More AI avatar packages
- [ ] Using emojis in own messages
- [ ] ...

# Known bugs that will be fixed soon
- [ ] Can't find any bugs yet :)

# Known issues
- Captcha message instead of a response. In this case, a link with a redirect to the Edge browser will be displayed, which will redirect you to the actual Bing Chat. From time to time, a captcha query is displayed there, which is intended to ensure that the chat is used by people and not by machines. Make sure that you solve the captcha with the same account for which you use the cookie token in the KATI app.
- The AI does not send a response: I have noticed that this sometimes happens with the VPN enabled. Disable VPN if it is enabled and restart the application.
- The AI sends an incomplete response: In the case of links, code, special characters, or if the AI's response is too long, the response sometimes does not arrive in full. Explain to the AI that its last response is incomplete, it will then try to send its response in a different way. If the answer takes longer, such as 5 minutes, it will also be canceled. There will be a setting option for this in a later version.


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

KATI is programmed with Electron and .NET6 and is therefore operating system independent. Currently only a download for Windows is offered, but there will probably also be an executable for Linux. The heart for the communication with the AI is the C# library [BingChat](https://github.com/bsdayo/BingChat).


[![GitHub release (with filter)](https://img.shields.io/github/downloads/hswlab/kati/total?style=for-the-badge&logo=ChatBot&label=download%20KATI
)](https://github.com/hswlab/kati/releases/latest)


*Key features in KATI v2.0.0:*
- [X] Conversation with the AI in the 3 usual chat modes: creative, balanced or direct
- [X] Formatted code and text output as a running text stream
- [X] Optional voice output with the default voice pre-installed in the OS
- [X] Visual emotions Feedback from the AI by means of a dynamic avatar image
- [X] Multilingual user interface (DE, EN, other languages on request)

![preview](https://github.com/hswlab/kati/blob/main/Screenshot.png)

![preview2](https://github.com/hswlab/kati/blob/main/Screenshot2.png)

# Nuget packages and associated licenses used in KATI
- Newtonsoft.Json <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- Esprima <a href="https://licenses.nuget.org/BSD-3-Clause">`BSD 3-Clause License`</a>
- ElectronNET.API <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- LiteDB <a href="https://www.nuget.org/packages/LiteDB/5.0.16/license">`MIT License`</a>
- BingChat <a href="https://github.com/bsdayo/BingChat/blob/main/LICENSE">`MIT License`</a>
- System.Speech  <a href="https://licenses.nuget.org/MIT">`MIT License`</a>

# More details
- English: [user manual](https://github.com/hswlab/kati/blob/main/about-en.pdf)
- German: [user manual](https://github.com/hswlab/kati/blob/main/about-de.pdf)

# Known issues
- Captcha message instead of a response. In this case, a link with a redirect to the Edge browser will be displayed, which will redirect you to the actual Bing Chat. From time to time, a captcha query is displayed there, which is intended to ensure that the chat is used by people and not by machines. Make sure that you solve the captcha with the same account for which you use the cookie token in the KATI app.
- The AI does not send a response: I have noticed that this sometimes happens with the VPN enabled. Disable VPN if it is enabled and restart the application.
- The AI sends an incomplete response: In the case of links, code, special characters, or if the AI's response is too long, the response sometimes does not arrive in full. Explain to the AI that its last response is incomplete, it will then try to send its response in a different way. If the answer takes longer, such as 5 minutes, it will also be canceled. There will be a setting option for this in a later version.

# Next milestone v3.0.0
- [ ] Use of Markdown interpreter for the Bing responses and better handling/representation of references used in the text.
- [ ] Setting option for automatic chat request timeot
- [ ] Manually cancel a running chat request
- [ ] Chat history
- [ ] Chat history search

# Ideas for upcoming milestones
- [ ] Minimization of problems listed in Known Issues
- [ ] Support for AI generated images
- [ ] Better voice output by using AI voices (only if realizable for free)
- [ ] Chat input with voice recognition (only if realizable free of charge)
- [ ] Setting your own avatar image
- [ ] Management for alternative AI avatar packages
- [ ] More AI avatar packages
- [ ] Initialization of the AI with basic information about the user and a desired behavior of the AI.
- [ ] Better text formatting for the AI answers
- [ ] Selection of emoji for own chat messages
- [ ] Emoji suggestions for your own messages
- [ ] Dynamic avatar images for your own messages (similar function to AI avatars)
- [ ] ...


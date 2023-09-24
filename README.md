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
- [X] Conversation with the AI in the 3 usual chat modes: creative, balanced or direct
- [X] Chat history with filter
- [X] Chat initialization with custom AI behaviour
- [X] Formatted code and text output as a running text stream
- [X] TTS: Optional voice output with the default voices in Windows
- [X] STT: Optional voice to text input with the default voice recognition of Windows
- [X] Visual emotions Feedback from the AI by means of a dynamic avatar image
- [X] Multilingual user interface (DE, EN, other languages on request)
- [X] Minimize to tray function

![preview](https://github.com/hswlab/kati/blob/main/Screenshot.png)

![preview2](https://github.com/hswlab/kati/blob/main/Screenshot2.png)

![preview3](https://github.com/hswlab/kati/blob/main/Screenshot3.png)

# Nuget packages and associated licenses used in KATI
- Newtonsoft.Json <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- Esprima <a href="https://licenses.nuget.org/BSD-3-Clause">`BSD 3-Clause License`</a>
- ElectronNET.API <a href="https://licenses.nuget.org/MIT">`MIT License`</a>
- LiteDB <a href="https://www.nuget.org/packages/LiteDB/5.0.16/license">`MIT License`</a>
- BingChat <a href="https://github.com/bsdayo/BingChat/blob/main/LICENSE">`MIT License`</a>
- System.Speech  <a href="https://licenses.nuget.org/MIT">`MIT License`</a>


# Next milestone v6.0.0
- [X] Better voice output by using AI TTS voices (I decided to use TikTok voices. I will also keep System.Speech as a fallback solution)
- [X] Multilangual TTS and UI (DE, EN, FR, ES, PT, JA, KO)
- [X] Simplify settings for TTS (Just choice TTS Voice and Speech speed)
- [X] Replacing BING API with own implementation (BING API is no longer supported so I decided to implement a custom solution)
- [X] Bing Token is not required anymore to make a conversation. (You simply can make even more requests, when a BING Token is added)
- [X] Automatically update BING token from Edge browser via button click.
- [X] Embedded BING Chat (If you like, you can also use the actual BING Chat directly in the KATI APP)
- [X] Show current/max conversation count in active conversation
- [ ] Advanced history view (Read aloud and continue conversation feature)
- [ ] Update Documentation/Manual. (For privacy reasons, the documentation must be supplemented with a note that EDGE cookies are processed!)
 

# Ideas for upcoming milestones
- [ ] Better voice input by using AI STT models (Maybe Whisper or a restricted free to use API. I will also keep System.Speech as a fallback solution)
- [ ] Feature to convert text to audiofile (suno-ai/bark => PABannier/bark.cpp is a nice candidate. TikTok voice is also nice to use)
- [ ] Test OpenNlp for better recognition of sentence endings.
- [ ] Categorize and fovorize selected conversations in the history.
- [ ] Export/Import function for chat history
- [ ] Support for AI generated images
- [ ] Setting your own avatar image
- [ ] Management for alternative AI avatar packages
- [ ] More AI avatar packages
- [ ] Selection of emoji for own chat messages
- [ ] Emoji suggestions for your own messages
- [ ] Dynamic avatar images for your own messages (similar function to AI avatars)
- [ ] UI Translations for Frensh, Chinese, Japanese, Russian, Spanish,...
- [ ] Using chat GPT in the APP without having to copy tokens from the edge browser or solving captcha questions outside the app.
- [ ] ...

# Known bugs that will be fixed soon
- [ ] Can't find any bugs yet :)

# Known issues
- Captcha message instead of a response. In this case, a link with a redirect to the Edge browser will be displayed, which will redirect you to the actual Bing Chat. From time to time, a captcha query is displayed there, which is intended to ensure that the chat is used by people and not by machines. Make sure that you solve the captcha with the same account for which you use the cookie token in the KATI app.
- The AI does not send a response: I have noticed that this sometimes happens with the VPN enabled. Disable VPN if it is enabled and restart the application.
- The AI sends an incomplete response: In the case of links, code, special characters, or if the AI's response is too long, the response sometimes does not arrive in full. Explain to the AI that its last response is incomplete, it will then try to send its response in a different way. If the answer takes longer, such as 5 minutes, it will also be canceled. There will be a setting option for this in a later version.


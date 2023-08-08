# KATI-AI (bing Chat-GPT 4)
[![GitHub](https://img.shields.io/github/license/hswlab/kati)](https://github.com/hswlab/kati/blob/main/LICENSE) 
[![Downloads](https://img.shields.io/github/downloads/hswlab/kati/total)](https://github.com/hswlab/kati/releases/latest) 
[![Downloads](https://img.shields.io/github/v/release/hswlab/kati)](https://github.com/hswlab/kati/releases/latest) 

KATI is an AI desktop chat application with bing Chat-GPT 4. It supports voice and visual emotion feedback of the AI. The goal of the development goes in the direction of J.A.R.V.I.S or HAL 9000. I imagine an application that is uncomplicated to set up and does not cost anything. Just download, launch and use. The heart for the communication with the AI is the C# library [BingChat](https://github.com/bsdayo/BingChat). 

*Key features in KATI v2.0.0:*
- Conversation with the AI in the 3 usual chat modes: creative, balanced or direct
- Formatted code and text output as a running text stream
- Optional voice output with the default voice pre-installed in the OS
- Visual emotions Feedback from the AI by means of a dynamic avatar image
- Multilingual user interface (DE, EN, other languages on request)

![preview](https://github.com/hswlab/kati/blob/main/Screenshot.png)

![preview2](https://github.com/hswlab/kati/blob/main/Screenshot2.png)

# Nuget packages and associated licenses used in kati
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
- Di AI does not send a response: I have noticed that this sometimes happens with the VPN enabled. Disable VPN if it is enabled and restart the application. 
- The AI sends an incomplete response: In the case of links, code, special characters, or if the AI's response is too long, the response sometimes does not arrive in full. Explain to the AI that its last response is incomplete, it will then try to send its response in a different way. If the answer takes longer, such as 5 minutes, it will also be canceled. There will be a setting option for this in a later version.


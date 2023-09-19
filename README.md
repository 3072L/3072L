### Hi there 👋

<!--
**3072L/3072L** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->


### I'm a sercurity researcher and coder 🔭 [my blog](https://github.com/3072L/3072l.github.io)


CNVD = Chinese National Vulnerability Database ID

I don't like CVE ID, because nowadays you can apply for a CVE ID even without providing any POC, and even the provided code snippet doesn't contain any vulnerabilities

###  vulnerabilities I found


#### IOT platform

| id             | company |   model    | vul type |  method   |
| -------------- | ------- | ---------- | ---- | ------------------ |
| X              | tenda    | Ac6        | RCE  | reverse  |
| x              | vigorfly | 200      | RCE    | reverse |
| x              | vigorfly | 2960     | RCE    | reverse |
| CNVD-2023-52338 | dlink    | 615      | overflow  | reverse + rcall |
| CNVD-2023-52238	 | dlink    | 615      | overflow  | reverse + rcall |
| CNVD-2023-56319 | dlink    | 615      | overflow  | reverse + rcall |
| CNVD-2023-53593 | dlink    | 615      | overflow  | reverse + rcall |
| CNVD-2023-53542 | dlink    | 615      | overflow  | reverse + rcall |
| CNVD-2023-53541 | dlink    | 615      | overflow  | reverse + rcall |

.... hundreds of overflow



#### Windows platform

| id             | company |   model    | vul type |  method   |
| -------------- | ------- | ---------- | ---- | ------------------ |
| CNVD-2021-21860 | Valve  | steam        | Dll Hijacking | dllfuzzer |
| CNVD-2021-18307 | tencent | yehu        | Dll Hijacking | dllfuzzer |
| x               | sangfor| edr          | Dll Hijacking | dllfuzzer |
| x               |  tencent | wechat     |  null pointer derefer | jackalope + tinyInst |
| x               |  microsoft | win32cacl |  null pointer derefer |   rust +  Mesos     |

.... hundreds of Dll Hijacking found by dllfuzzer 





#### Linux platform

| id             | company |   model      | vul type            |  method   |
| -------------- | ------- | ----------   |  ------------------ |---------- |
| X              | GIMP    | libbabl      |  SEGV               | AFL++     |



SEGV found by AFL++ in libbabl


#### Web

| id             | company |   model      | vul type            |  method   |
| -------------- | ------- | ----------   |  ------------------ |---------- |
| CVE-2020-16610 |Hoosk CMS|     x        |  CSRF               | code audit|


### Tools I developed


#### dllfuzzer

A very simple tool that can find hundreds of dll Hijacking vulnerabilities, which is developed in rust

to be public ....

#### rcall

A tool that can help researcher find  lots of potential  vulnerabilities in IOT firmware inspired by @alexjplaskett

to be public ....

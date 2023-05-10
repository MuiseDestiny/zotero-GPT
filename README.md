<div align="center">
  <img src="imgs/background.svg" width="50%" />


# Zotero GPT


👋

Share the tag command you made in [here](https://github.com/MuiseDestiny/zotero-gpt/discussions/3) using [Meet API](src/modules/Meet/api.ts).

[![Using Zotero Plugin Template](https://img.shields.io/badge/Using-Zotero%20Plugin%20Template-blue?style=flat-round&logo=github)](https://github.com/windingwind/zotero-plugin-template)
[![Latest release](https://img.shields.io/github/v/release/MuiseDestiny/zotero-gpt)](https://github.com/MuiseDestiny/zotero-gpt/releases)
![Release Date](https://img.shields.io/github/release-date/MuiseDestiny/zotero-gpt?color=9cf)
[![License](https://img.shields.io/github/license/MuiseDestiny/zotero-gpt)](https://github.com/MuiseDestiny/zotero-gpt/blob/master/LICENSE)
![Downloads latest release](https://img.shields.io/github/downloads/MuiseDestiny/zotero-gpt/latest/total?color=yellow)


  <img src="https://user-images.githubusercontent.com/51939531/228763331-90baa9aa-8bef-4b32-9d6f-35538b58b158.png" width="80%" />

</div>




---


## 🚀 Main Features
Features about GPT:  
- [x] 🔗 **Integrate with Zotero**: You can use the plugin to search and ask items in the library based on the selected text or the PDF file.
- [x] 🧠 Use GPT to generate reply text: support `gpt-3.5-turbo` and `gpt-4`
- [x] 🏷️ [Command tags](https://github.com/MuiseDestiny/zotero-gpt#command-tags): **Click once** to accelerate your research.  
  - [x] 💬 Ask questions about current **PDF file** (full-text or selected text).
  - [x] 💬 Ask questions about **selected paper** (Abstract).
  - [x] 📝 **Summarize the selected paper** into several highly condensed sentences.
  - [x] 🔍 **Search items** in the library based on the selected text.
  - [x] ... ...
- [x] ⚙️ **Advanced settings for GPT**: You can set the [api key](https://platform.openai.com/account/api-keys), [model name](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model), [api url](https://platform.openai.com/docs/api-reference/chat/create), [temperature](https://platform.openai.com/docs/api-reference/chat/create#chat/create-temperature).
- [x] 📚 **Integrate with Better Notes**: You can directly open this plugin when using [Better Notes](https://github.com/windingwind/zotero-better-notes).

Features about UI:
- [x] 🎨 **Real-time markdown rendering** for reply text: Latex and mathjax are supported.
- [x] 🔍 **Zoom in and out** of the reply text or the size of the plugin window.
- [x] 🖱️ **Move the plugin window to any position** on the screen.
- [x] 📋 **Copy the reply text** to the clipboard.
- [x] ⚠️ Detailed **error message** will be displayed when the request fails.
- [x] 🔧 Compatible with **Zotero 6** and **Zotero 7**.
- [x] 🎉 Discover more exciting features that are not listed here.

## How to Use
### For User

| Step | Desp | Screenshot |
| -- | -- | -- |
|1| Download the latest [xpi file](https://github.com/muisedestiny/zotero-gpt/releases/latest/download/zotero-gpt.xpi). | ![image](https://user-images.githubusercontent.com/51939531/236629181-0514d0b8-6f2f-46d3-9387-0bdbdea8245b.png)|
|2|Open Zotero, click `Tools`-`Add-ons`, and drag xpi file to `Add-ons` window. |![image](https://user-images.githubusercontent.com/51939531/236629000-f2d0e027-70e0-4f5c-84a5-60cff5d1246f.png)|
|3| Press `Ctrl + /` or `Shift + /` to wake up Zotero GPT window. | https://github.com/MuiseDestiny/zotero-gpt/issues/102 |

### For Developer

|Step|Desp|
|--|--|
|1|`git clone https://github.com/MuiseDestiny/zotero-gpt.git`|
|2|`cd zotero-gpt`|
|3|`npm i -s`|
|4|`npm run build` to generate xpi file. |

### Set up the API secret key

Enter `/secretKey sk-xxxx` and press `Enter`.
![image](https://user-images.githubusercontent.com/51939531/236629699-f4cc70f0-7bb7-46ac-a528-df555643ff80.png)

## Command Tags

The plug-in design concept is to configure command tabs according to different application scenarios, and directly click on the tabs to complete the interaction with GPT.

Type `#label_name[color=#eee][position=1]` and Enter to edit a lable. Save with `Ctrl + S`. Save and Run with `Ctrl + R`.

`color` can be abbreviated to `c`, `position` can be reviated to `pos` and the values can be quoted.

For example, `#test[c=#eee][pos=9]` is a legit input.

Of course `color` and `position` are optional parameters and will have default values if not entered.

In the next step, you can declare an executable code fragment for the current environment like this:

![image](imgs/prompt.png)

It will be executed and the returned result will replace the code snippet here.

You can command GPT to output a code fragment and the plugin can execute it.

Click the left mouse button and hold to enter the edit mode of a label.

**Hold with the right mouse button is to delete the label**.

Single click on a label is to execute it.

You can click and hold on each label after installing the plugin to see the internal statements of the sample tags, and I'm sure you'll be up and running writing a new one in no time.


## Ask PDF [build-in tag]

<div align="center">

https://user-images.githubusercontent.com/51939531/232497591-9f78e65e-3c4b-4519-987c-f1c3a277a209.mp4

</div>

Implementation method:

Make sure the plugin version is up-to-date.

## Search Items [build-in tag]

![image](https://user-images.githubusercontent.com/51939531/231054213-427056c2-35dd-48d4-8e0d-e334bb85a46f.png)

Implementation method: 
Same as `Ask PDF`

## Ask Annotations [Under development]

![image](https://user-images.githubusercontent.com/51939531/232672386-8f0b929c-13de-4f34-9d75-d3d889ceb316.png)


## Demonstration

![image](imgs/demo.png)


![image](imgs/demo2.png)

## Support the project

[Here](https://github.com/MuiseDestiny/zotero-reference#%E8%B5%9E%E5%8A%A9)


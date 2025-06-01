<h4 align="left">
  <b href="readme.md">中文</b> |
  <a >English</a>
</h4>

# Disclaimer  

> 1. This is machine-translated, so the quality may not be ideal. Please don’t expect perfection!  
>  
> 2. My personal setup: Videos without embedded subtitles + external ASS subtitles + online translation. I recommend this approach because hardcoded subtitles (burned into the video frames) cannot be translated. Try testing with this format first!  
>  
> 3. I am only the open-source contributor, providing this for technical discussion. I decline any responsibility for issues that may arise.  
>  
> 4. Parts of this document and some code are adapted from prior works.  
>  
> 5. Special thanks to the original authors! Grateful for their contributions!  
>  
> 6. Original project address: [https://github.com/fjqingyou/PotPlayer_Subtitle_Translate_Baidu](https://github.com/fjqingyou/PotPlayer_Subtitle_Translate_Baidu)  

---  

# Cost  

> 1. First, this plugin is completely free!  
>  
> 2. As far as I know, Youdao Translate is not entirely free, but new accounts get 50 free credits (trial quota).  

---  

# Installation & Usage  

## Step 1: Register an application on Youdao Zhiyun  

> 1. Visit: [https://ai.youdao.com/product-fanyi-text.s](https://ai.youdao.com/product-fanyi-text.s)  
>  
> 2. Register and log in or sign in to your existing Youdao Zhiyun account.  
>  
> 3. On the page from Step 1, click "Start Using Now."  
>  
> 4. In the dashboard, find "Natural Language Translation Service" on the left, then select "Text Translation" and click "Create Application."  
>  
> 5. Fill in:  
> - "Application Name" → Custom  
> - "Select Service" → Check "Text Translation" under "Natural Language Translation Service"  
> - "Access Method" → Select "API"  
> Then click "Confirm" to complete.  

---  

## Step 2: Install the translation plugin  

> 1. Select `SubtitleTranslate - Youdao.as` and `SubtitleTranslate - Youdao.ico`, then press **Ctrl+C** to copy.  
>  
> 2. Navigate to PotPlayer’s installation directory (search online if unsure how).  
>  
> 3. Go into the **Extention** folder → **Subtitle** → **Translate**.  
>  
> 4. Press **Ctrl+V** to paste the two files here.  

---  

## Step 3: Configure the App ID and Secret Key  

> 1. Return to the URL in Step 1, click your username in the top-right corner, and enter the "Dashboard."  
>  
> 2. Under "My Applications" in "Business Overview," you’ll see the app you created. Note the **Application ID** and **Application Secret**.  
>  
> 3. Open a video with external subtitles (e.g., an ASS file).  
>  
> 4. Right-click the video → **Subtitles** → **Online Subtitle Translation** → **Real-time Translation Settings** → Select **Youdao Translate** → Click **"Account Settings"** on the right.  
>  
> 5. Enter the **Application ID** and **Application Secret** from Step 2 into "App ID" and "Secret Key," respectively. Click **OK**, then close the dialog.  

---  

## Step 4: Testing  

> 1. Open any video with subtitles (or reuse the previous one).  
>  
> 2. Right-click → **Subtitles** → **Online Subtitle Translation** → **Youdao Translate**.  
>  
> 3. Optional:  
> - Enable **Always Use** (if preferred).  
> - Enable **Show Translation Below** (if preferred).  
> - Set **Target Language** (e.g., English, Japanese, Chinese, etc.).  
>  
> 4. Enjoy!  

---  

## Optional Configuration – Translation Request Frequency  

> 1. This step is optional and usually unnecessary.  
>  
> 2. Reason: Youdao Translate has a default cooldown period. Frequent requests may trigger errors (e.g., `errorCode: xxxx`). Adjust only if issues occur. Refer to the **Cost** section for details.  
>  
> 3. Open `SubtitleTranslate - Youdao.as` (the installed file, not the local copy) in a text editor.  
>  
> 4. Locate `int coolTime = 1000;` (around line 23). Increase the value (e.g., 2000 for 2 seconds) to reduce request frequency.  
> - `1000` = 1 second delay between translations.  
> - Lower values = faster requests; higher values = slower requests.  
> - Do not delete the semicolon (`;`).  
>  
> 5. Save the file and restart PotPlayer.  

---  

# Contribute  

> Contributions are welcome! Feel free to submit improvements via pull requests.  
>  
> GitHub: [https://github.com/lp20010415/PotPlayer_Subtitle_Translate_Youdao](https://github.com/lp20010415/PotPlayer_Subtitle_Translate_Youdao)  
>  
> Gitee: [https://gitee.com/lp20010415/PotPlayer_Subtitle_Translate_Youdao](https://gitee.com/lp20010415/PotPlayer_Subtitle_Translate_Youdao)  

---  
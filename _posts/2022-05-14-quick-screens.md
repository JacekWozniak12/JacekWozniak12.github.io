---
layout: post
title: Creating quick screenshots using Unity. 
categories: [Unity, Programming, C#]
imageLink: "/assets/images/posts/blog-miniatures/5to1.png"
--- 

Recently I was working on my simple logic game called __5 To 1__. As I wanted to make my job quicker with levels I created tool, that would easily help me with achieving multiple screenshots at the same time. 

I wrote simple code below.

```
    IEnumerator ScreenshotTask()
    {
        for (int i = 0; i < Container.Length; i++)
        {
            // Additive is very important here, as this coroutine is scene dependant.
            // And unloading it would break entire process of gathering screens

            SceneManager.LoadSceneAsync(Container[i].SceneName, LoadSceneMode.Additive);
            yield return new WaitForSecondsRealtime(0.33f);
            // here can come other things before capture
            ScreenCapture.CaptureScreenshot(
                    Application.dataPath + "/Images/" + 
                    Container[i].SceneName + ".png" 
                    );
            // after capture
            yield return new WaitForSecondsRealtime(0.33f);
            yield return SceneManager.UnloadSceneAsync(Container[i].SceneName);
        }
    }
```

It is both scene dependant (as I'm running it on other scene, that handles loading all of levels) and display dependant (so I have to set my display before I start gathering screenshots).

![](/assets/images/posts/five-to-one/unity-view.png)


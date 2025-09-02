# Setup Additional Features

Some features of Sequentior needs some specific packages are imported to your project. After you import a specific package, you can setup its related functions by opening __Tools -> KerimKaynakci Games -> Sequentior Setup__ from the main menu of Unity Editor.

![Setup](img/setupadditional.jpg)

!!! warning
    You need to setup again if you switch the target platform of your project!

## TextMeshPro

Although TextMeshPro UPM package is already included in a project, TextMesh Pro TMP package needs to be installed manually. So Sequentior cannot assume it's included in your project. So you need to tell Sequentior that you've the TextMeshPro package in your project.

To make this happen, click the "TextMeshPro Setup" button in this Setup window.

!!! note
    This setup procedure will simply add __"SEQUENTIOR_TMP"__ to the _Scripting Define Symbols_ of your project. And in the sequential scripts, TextMeshPro related codes are defined in the scope of this symbol.


## Post Processing for URP

Normally, when you create a URP project from Unity templates, the packages for post processing effects are included by default. But for some reason it might be removed (manually). Also, you need to tell Sequentior that you're using URP specifically. 

To make this happen, click the "Post Processing for URP Setup" button in this Setup window.

!!! note
    This setup procedure will simply add __"SEQUENTIOR_POSTPROCESSING_URP"__ to the _Scripting Define Sybmols_ of your project. And in the sequential scripts, URP Post Processing related codes are defined in the scope of this symbol.


## Post Processing for Built-in Render Pipeline

Built-in RP projects don't have a post processing library included by default. So you need to import Post Processing (Stack) library from package manager manually and then you need to tell Sequentior that you've imported this post processing package. 

To make this happen, click the "Post Processing for Built-in RP Setup" button in this Setup window.

!!! note
    This setup procedure will simply add __"SEQUENTIOR_POSTPROCESSING_BUILTIN"__ to the _Scripting Define Sybmols_ of your project. And in the sequential scripts, Built-in RP Post Processing related codes are defined in the scope of this symbol.



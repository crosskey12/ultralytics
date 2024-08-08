---
comments: true
description:
keywords: Visual Studio Code, VS Code, deep learning, convolutional neural networks, computer vision, Python, code snippets, Ultralytics, developer productivity, machine learning, YOLO, developers, productivity, efficiency, learning, programming, IDE, code editor, developer utilities, programming tools
---

# Accelerate Your Computer Vision Projects with Ultralytics Code Snippets

<p align="center">
  <br>
    <img src="https://github.com/Burhan-Q/ultralytics-snippets/assets/62214284/42ad0b17-e752-479c-9c6c-e451fffbe8b3" alt="Snippet Prediction Preview">
  <br>
  <strong>NOTE: </strong>Tab-completion used to complete snippet and quickly hop between fields.
</p>

✅ Are you a data scientist or machine learning engineer building computer vision applications with Ultralytics?

✅ Do you despise writing repetitive code for common tasks?

✅ Are you always forgetting the arguments or default values for the [predict], [train], [track], or [val] methods?

✅ Looking to get started with Ultralytics and wish you had an _easier_ way to reference or run code examples?

✅ Want to speed up your development cycle when working with Ultralytics?

If you use Visual Studio Code and answered 'yes' to any of the above, then the `Ultralytics-Snippets` extension for VS Code is her to help! It was the Ultralytics Community that inspired the creation of this extension. Read on to learn more about the extension, how to install it, and how to use it.

## Why VS Code?

[Visual Studio Code](https://code.visualstudio.com/) is extremely popular with developers worldwide and has ranked most popular by the Stack Overflow Developer Survey in [2021], [2022], [2023], and [2024]. Given VS Code's high level of customization, built-in features, compatibility, and extensibility, it's no surprise that so many developers are using it. Given the popularity in the larger developer community and within the Ultralytics [Discord], [Discourse], [Reddit], and [GitHub] Communities, it made sense to build a VS Code extension to help streamline your workflow and boost your productivity.

Want to let us know what you use for developing code? Head over to our Discourse [community poll] and let us know! While you're there, maybe check out some of our favorite computer vision, machine learning, AI, and developer [memes], or even post your favorite!

## Installing the Extension

!!! Note
Any code environment that will allow for installing VS Code extensions _should be_ compatible with the `Ultralytics-snippets` extension. After publishing the extension, it was discovered that [neovim](https://neovim.io/) can be made compatible with VS Code extensions. To learn more see the [`neovim` install section of the Readme][neovim install] in the [Ultralytics-Snippets repository][repo].

### Installing in VS Code

1. Navigate to the Extensions menu in VS Code, and search for `Ultralytics-Snippets`.

2. Click the ++"Install"++ button.

<p align="center">
  <br>
    <img src="https://github.com/user-attachments/assets/9de46d22-ef7b-4765-ba2c-d0459cafa4dc" alt="VS Code extension menu">
  <br>
</p>

### Installing from the VS Code Extension Marketplace

1. Visit the VS Code Extension Marketplace by going to https://marketplace.visualstudio.com/VSCode and search for `Ultralytics-Snippets` or go straight to the [extension page on the VS Code marketplace].

2. Click the ++"Install"++ button and allow your browser to launch a VS Code session.

<p align="center">
  <br>
    <img src="https://github.com/user-attachments/assets/b40cc8e2-2353-4165-859a-c84eec070db6" alt="VS Code marketplace extension install">
  <br>
</p>

3. Follow any prompts to install the extension.

## Using the Ultralytics-Snippets Extension

- **Intelligent Code Completion:** Write code faster and more accurately with advanced code completion suggestions tailored to the Ultralytics API.

- **Increased Development Speed:** Save time by eliminating repetitive coding tasks and leveraging pre-built code block snippets.

- **Improved Code Quality:** Write cleaner, more consistent, and error-free code with intelligent code completion.

- **Streamlined Workflow:** Stay focused on the core logic of your project by automating common tasks.

### Overview

The extension will only operate when the [Language Mode](https://code.visualstudio.com/docs/getstarted/tips-and-tricks#_change-language-mode) is configured for Python. This is to avoid snippets from being inserted when working on any other file type, as all code snippets are for Python. All snippets start with a prefix of `ultra`, and simply typing `ultra` in your editor after installing the extension, will display a list of possible snippets to use. You can also open the VS Code [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) using ++ctrl+shift+p++ and running the command `Snippets: Insert Snippet`.

### Code Snippet Fields

Many snippets have "fields" with default placeholder values or names. For instance, output from the [predict] method could be saved to a Python variable named `result`, `results`, `detections`, `preds` or whatever else a developer chooses, which is why the "fields" are important. Using ++tab++ on your keyboard after a snippet is inserted, your cursor will move between fields quickly. Once a field is selected, typing a new variable name will change that instance, but also every other instance in the snippet code for that variable!

<p align="center">
  <br>
    <img src="https://github.com/user-attachments/assets/661c1b85-39a5-48ec-9faa-89d44e49aa37" alt="Multi-update field and options">
  <br>
  After inserting snippet, renaming <code>model</code> as <code>world_model</code> updates all instances. Pressing <kbd class="key-tab">Tab</kbd> moves to the next field, which opens a dropdown menu and allows for selection of a model scale, and moving to the next field provides another dropdown to choose either <code>world</code> or <code>worldv2</code> model variant.
</p>

### Code Snippet Completions

It's not required to type the full name of the snippet, or even from the start of the snippet. The snippets are named in the most descriptive way possible, but this means there could be a lot to type and that could be counterproductive if the aim is to move _faster_. VS Code let's users type `ultra.example-yolo-predict`, `example-yolo-predict`, `yolo-predict`, or even `ex-yolo-p` and still reach the intended snippet option! If the intended snippet was _actually_ `ultra.example-yolo-predict-kwords`, then just using your keyboard arrows ++up++ or ++down++ to highlight the desired snippet and pressing ++enter++ or ++tab++ will insert the correct block of code.

<p align="center">
  <br>
    <img src="https://github.com/user-attachments/assets/bdd9aada-de8a-4d73-b714-04f8a48c0436" alt="Incomplete Snippet Example">
  <br>
  Typing <code>ex-yolo-p</code> will <em>still</em> arrive at the correct snippet.
</p>

## Categories

These are the current snippet categories available to the `Ultralytics-Snippets` extension. More will be added in the future, so make sure to check for updates or enable auto-updating. You can also request additional snippets to be added if you feel there's any missing.

| Category  | Description                                                                                                                                   |
| :-------- | :-------------------------------------------------------------------------------------------------------------------------------------------- |
| Examples  | Example code to help learn or for getting started with Ultralytics. Examples are copies of or similar to code from documentation pages.       |
| Kwargs    | Speed up development by adding snippets for [train], [track], [predict], and [val] methods with all keyword arguments and default values.     |
| Imports   | Snippets to quickly import common Ultralytics objects.                                                                                        |
| Models    | Insert code blocks for initializing various models, including dropdown configuration options.                                                 |
| Results   | Code blocks for common operations when [working with inference results].                                                                      |
| Utilities | Provides quick access to common utilities that are built into the Ultralytics package, learn more about these on the [Simple Utilities page]. |

### Learning with Examples

The examples snippets are to useful for anyone looking to learn how to get started with the basics of working with Ultralytics YOLO. Example snippets are intended to run once inserted (some have dropdown options as well), an example of this is shown at the animation at the [top] of this page, where after the snippet is inserted, all code is selected and run interactively using ++shift+enter++.

!!! Example

    Just like the animation shows at the [top] of this page, you can use the snippet `ultra.example-yolo-predict` to insert the following code example. Once inserted, the only configurable option is for the model scale which can be any one of: `n`, `s`, `m`, `l`, or `x`.

    ```python
    from ultralytics import ASSETS, YOLO

    model = YOLO("yolov8n.pt", task="detect")
    results = model(source=ASSETS / "bus.jpg")

    for result in results:
        print(result.boxes.data)
        # result.show()  # uncomment to view each result image
    ```

### Accelerating Development

The aim for snippets outside of the `examples` are for making development easier and quicker when working with Ultralytics. A common code block to be used in many projects, is to iterate the Results returned from using the model [predict] method. The `ultra.result-loop` snippet can help with this.

!!! Example

    Using the `ultra.result-loop` will insert the following default code (including comments).

    ```python
    # reference https://docs.ultralytics.com/modes/predict/#working-with-results

    for result in results:
        result.boxes.data  # torch.Tensor array
    ```

However, since Ultralytics supports numerous [tasks], when [working with inference results] there are other `Results` attributes that you may wish to access, which is where the [snippet fields](#code-snippet-fields) are helpful.

<p align="center">
  <br>
    <img src="https://github.com/user-attachments/assets/16cc72eb-4390-4380-bfaa-a0e84e5251db" alt="Results Loop Options">
  <br>
  Once tabbed to the <code>boxes</code> field, a dropdown menu appears to allow for selection of other methods available.
</p>

### Keywords Arguments

There are over 💯 keyword arguments for the various Ultralytics [tasks] and [modes]! That's a lot to remember and it can be easy to forget if the argument is `save_frame` or `save_frames` (it's definitely `save_frames` by the way). This is where the `kwargs` snippets can help out!

!!! Example

    To insert the [predict] method, including all [inference arguments], use `ultra.kwargs-predict`, which will insert the following code (including comments).

    ```python
    model.predict(
        source=src,  # (str, optional) source directory for images or videos
        imgsz=640,  # (int | list) input images size as int or list[w,h] for predict
        conf=0.25,  # (float) minimum confidence threshold
        iou=0.7,  # (float) intersection over union (IoU) threshold for NMS
        vid_stride=1,  # (int) video frame-rate stride
        stream_buffer=False,  # (bool) buffer all streaming frames (True) or return the most recent frame (False)
        visualize=False,  # (bool) visualize model features
        augment=False,  # (bool) apply image augmentation to prediction sources
        agnostic_nms=False,  # (bool) class-agnostic NMS
        classes=None,  # (int | list[int], optional) filter results by class, i.e. classes=0, or classes=[0,2,3]
        retina_masks=False,  # (bool) use high-resolution segmentation masks
        embed=None,  # (list[int], optional) return feature vectors/embeddings from given layers
        show=False,  # (bool) show predicted images and videos if environment allows
        save=True,  # (bool) save prediction results
        save_frames=False,  # (bool) save predicted individual video frames
        save_txt=False,  # (bool) save results as .txt file
        save_conf=False,  # (bool) save results with confidence scores
        save_crop=False,  # (bool) save cropped images with results
        stream=False,  # (bool) for processing long videos or numerous images with reduced memory usage by returning a generator
        verbose=True,  # (bool) enable/disable verbose inference logging in the terminal
    )
    ```

    This snippet has fields for all arguments, but also for `model` and `src` in case you've used a different variable in your code. On each line containing a keyword argument, a brief description is included for reference.

### All Code Snippets

The best way to find out what snippets are available is to download and install the extension! If you're curious and want to take a look at the list beforehand, you can visit the [repo] or [extension page on the VS Code marketplace] to view the tables for all available snippets.

## FAQ

### How do I request a new snippet?

New snippets can be requested using the Issues on the Ultralytics-Snippets [repo].

### How much does the Ultralytics-Extension Cost?

It's 100% free!

### Why don't I see a code snippet preview?

VS Code uses the key combination ++ctrl+space++ to show more/less information in the preview window. If you're not seeing a snippet preview when you type in a code snippet prefix, using this key combination should restore the preview.

### How do I disable the extension recommendation in Ultralytics?

If you use VS Code and have started to see a message prompting you to install the `Ultralytics-Snippets` extension, and don't want to see the message any more, there are two ways to disable this message.

1. Install `Ultralytics-Snippets` and the message will no longer be shown 😆!

2. You can using `yolo settings vscode_msg False` to disable the message from showing without having to install the extension. You can learn more about the [Ultralytics Settings] on the [quickstart] page if you're unfamiliar.

### I have an idea for a new Ultralytics code snippet, how can I get one added?

Visit the `Ultralytics-Snippets` [repo] and open an Issue or Pull Request!

<!-- Article Links -->

[top]: #accelerate-your-computer-vision-projects-with-ultralytics-code-snippets
[export]: ../modes/export.md
[predict]: ../modes/predict.md
[track]: ../modes/track.md
[train]: ../modes/train.md
[val]: ../modes/val.md
[tasks]: ../tasks/index.md
[modes]: ../modes/index.md
[working with inference results]: ../modes/predict.md#working-with-results
[inference arguments]: ../modes/predict.md#inference-arguments
[Simple Utilities page]: ../usage/simple-utilities.md
[Ultralytics Settings]: ../quickstart.md/#ultralytics-settings
[quickstart]: ../quickstart.md
[Discord]: https://ultralytics.com/discord
[Discourse]: https://community.ultralytics.com
[Reddit]: https://reddit.com/r/Ultralytics
[GitHub]: https://github.com/ultralytics
[community poll]: https://community.ultralytics.com/t/what-do-you-use-to-write-code/89/1
[memes]: https://community.ultralytics.com/c/off-topic/memes-jokes/11
[repo]: https://github.com/Burhan-Q/ultralytics-snippets
[extension page on the VS Code marketplace]: https://marketplace.visualstudio.com/items?itemName=Ultralytics.ultralytics-snippets
[neovim install]: https://github.com/Burhan-Q/ultralytics-snippets?tab=readme-ov-file#use-with-neovim
[2021]: https://survey.stackoverflow.co/2021#section-most-popular-technologies-integrated-development-environment
[2022]: https://survey.stackoverflow.co/2022/#section-most-popular-technologies-integrated-development-environment
[2023]: https://survey.stackoverflow.co/2023/#section-most-popular-technologies-integrated-development-environment
[2024]: https://survey.stackoverflow.co/2024/technology/#1-integrated-development-environment
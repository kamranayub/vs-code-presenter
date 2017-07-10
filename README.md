# presenter README

See my [series of tweets](https://twitter.com/kamranayub/status/884236601945206785).

Highly experimental. Probably crazy.

## Features

- Capture audio from a recording device
- Captures UI events including keystrokes
- Exports to a file that can be shared
- Plays back recordings with "virtual" workspace

## TODO

Gotta figure out:

- How to playback virtually without requiring exact machine/workspace configuration?
- Does it just snapshot the state of VS Code? If so how does it restore?
- What about other parts of the UI (terminal, etc.)?
- What about different VS code versions over time? Does it matter (i.e. this thing just TAKES OVER and the UI is what it was when it was recorded)?

Ideas:

- Similar "mode" to debugging where status bar and UI changes to "record" mode
- In playback mode, I think the only way for this to work is to take control over the entire IDE
- Users could edit in playback mode, but it probably wouldn't do anything--without actual physical files/configuration, nothing would work
- Could it allow tying into Git commits? Would that be a way to distribute the workspace? It would have to have preparation steps or automation (npm, etc.).
- If VS code exposes eventing model and actions, that could be a standard API surface to record/playback as long as underlying workspace and configuration was the same. Or if something like Redux was used to allow for time traveling over state.
- THIS IS CRAZY.

## Requirements

<!--
If you have any requirements or dependencies, add a section describing those and how to install and configure them.
-->

## Extension Settings

<!--
Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something
-->

## Known Issues

- It doesn't work yet

## Release Notes
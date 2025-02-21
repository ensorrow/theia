# Change Log

## v0.11.0

- [task] added `tasks.fetchTasks()` and `tasks.executeTask()` to plugins API [#6058](https://github.com/theia-ide/theia/pull/6058)

Breaking changes:

- [core][plugin] support alternative commands in context menus [6069](https://github.com/theia-ide/theia/pull/6069)
- [workspace] switched `workspace.supportMultiRootWorkspace` to enabled by default [#6089](https://github.com/theia-ide/theia/pull/6089)

## v0.10.0

- [core] added ability to execute tasks via keybindings [#5913](https://github.com/theia-ide/theia/pull/5913)
- [core] added better handling for the `SingleTextInputDialog` `onEnter` [#5868](https://github.com/theia-ide/theia/pull/5868)
- [core] added handling for command handler errors [#5894](https://github.com/theia-ide/theia/pull/5894)
- [core] added propagation of phosphor events to view container widgets [#5817](https://github.com/theia-ide/theia/pull/5817)
- [core] added support for HTML titles for widgets in the sidebar [#5948](https://github.com/theia-ide/theia/pull/5948)
- [core] added support for path normalization [#5918](https://github.com/theia-ide/theia/pull/5918)
- [core] added the optional flag `runIfSingle` for `QuickPickOptions` [#6059](https://github.com/theia-ide/theia/pull/6059)
- [core] fixed issue where the last visible view container was not preserved [#5817](https://github.com/theia-ide/theia/pull/5817)
- [core] fixed menu bar color [#6014](https://github.com/theia-ide/theia/pull/6014)
- [core] improved `QuickInput` and `QuickInputBox` APIs [#5187](https://github.com/theia-ide/theia/pull/5187)
- [core] supported diagnostic marker in the tab bar [#5845](https://github.com/theia-ide/theia/pull/5845)
- [cpp] added support for multiple root cpp build configurations [#4603](https://github.com/theia-ide/theia/pull/4603)
- [cpp] enabled better semantic highlighting support [#5850](https://github.com/theia-ide/theia/pull/5850)
- [cpp] moved cpp grammars from the `@theia/cpp` extension to the `@theia/textmate-grammars` extension [#5803](https://github.com/theia-ide/theia/pull/5803)
- [debug] added progress indicator for the debug widget [#6009](https://github.com/theia-ide/theia/pull/6009)
- [debug] ensured that terminate flags are properly restarted [#5954](https://github.com/theia-ide/theia/pull/5954)
- [debug] fixed issue where the debug icons remain opaque after a debug session has terminated [#5933](https://github.com/theia-ide/theia/pull/5933)
- [debug] removed superfluous scrollbars [#5879](https://github.com/theia-ide/theia/pull/5879)
- [editor] added support for tab details to disambiguate identical tabs [#5775](https://github.com/theia-ide/theia/pull/5775)
- [editor] added support to re-open files with different encodings [#5371](https://github.com/theia-ide/theia/pull/5371)
- [editor] added support to set default file encoding [#5371](https://github.com/theia-ide/theia/pull/5371)
- [editor] updated editor tabbar captions for better multi-root support [#5924](https://github.com/theia-ide/theia/pull/5924)
- [file-search] improved Windows support [#6029](https://github.com/theia-ide/theia/pull/6029)
- [git] added progress indicators for scm/git operations [#5830](https://github.com/theia-ide/theia/pull/5830)
- [git] added support to initialize a workspace as a git repository [#6008](https://github.com/theia-ide/theia/pull/6008)
- [git] fixed the git-diff widget header details alignment [#5998](https://github.com/theia-ide/theia/pull/5998)
- [git] updated ls-files so it works with Git >= 2.16 [#5851](https://github.com/theia-ide/theia/pull/5851)
- [keymaps] fixed clumsy auto-suggestion dropdown [#5990](https://github.com/theia-ide/theia/pull/5990)
- [markers] added problem markers to editor tabs [#5845](https://github.com/theia-ide/theia/pull/5845)
- [markers] added the preference `problems.decorations.enabled` to control the display of problem markers in tree widgets [#6021](https://github.com/theia-ide/theia/pull/6021)
- [messages] reworked messages and added a notification center [#5830](https://github.com/theia-ide/theia/pull/5830)
- [mini-browser] added support for editor/title context menus for webviews [#6030](https://github.com/theia-ide/theia/pull/6030)
- [monaco] aligned snippet completion logic with VSCode [#5931](https://github.com/theia-ide/theia/pull/5931)
- [navigator] added support for multi-file copy [#5864](https://github.com/theia-ide/theia/pull/5864)
- [navigator] added the toolbar item `more actions...` for the explorer [#5953](https://github.com/theia-ide/theia/pull/5953)
- [navigator] added the toolbar item `refresh` to force a refresh of the explorer [#5940](https://github.com/theia-ide/theia/pull/5940)
- [outline] added `OutlineViewTreeModel` for the outline view tree widget [#5687](https://github.com/theia-ide/theia/pull/5687)
- [outline] added the toolbar item `collapse-all` for the outline widget [#5687](https://github.com/theia-ide/theia/pull/5687)
- [outline] updated the keybinding for `toggle outline view` to avoid conflict [#5707](https://github.com/theia-ide/theia/pull/5707)
- [plugin-ext] added `ignoreFocusOut` parameter support for the `QuickPick` [#5900](https://github.com/theia-ide/theia/pull/5900)
- [plugin-ext] added automatic downloading of `extensionDependencies` [#5379](https://github.com/theia-ide/theia/pull/5379)
- [plugin-ext] added support for theming webview content [#5981](https://github.com/theia-ide/theia/pull/5981)
- [plugin-ext] fixed leaking java debug process [#5281](https://github.com/theia-ide/theia/pull/5281)
- [plugin-ext] fixed plugin-ext file path error [#5929](https://github.com/theia-ide/theia/pull/5929)
- [plugin] added additional support for `QuickPick` API [#5766](https://github.com/theia-ide/theia/pull/5766)
- [plugin] added better error handling for plugins that cannot find files [#6002](https://github.com/theia-ide/theia/pull/6002)
- [plugin] added cache for command arguments to safely pass them over JSON-RPC [#5961](https://github.com/theia-ide/theia/pull/5961)
- [plugin] added view containers support [#5665](https://github.com/theia-ide/theia/pull/5665)
- [search-in-workspace] added display of leading and trailing whitespaces in the search-in-workspace results [#5989](https://github.com/theia-ide/theia/pull/5989)
- [search-in-workspace] added progress indicator for search-in-workspace [#5980](https://github.com/theia-ide/theia/pull/5980)
- [search-in-workspace] fixed clumsy auto-suggestion dropdown [#5990](https://github.com/theia-ide/theia/pull/5990)
- [search-in-workspace] fixed the alignment in the search-in-workspace result note [#5802](https://github.com/theia-ide/theia/pull/5802)
- [search-in-workspace] modified `replace-all` functionality to save changes to editors without opening them [#5600](https://github.com/theia-ide/theia/pull/5600)
- [task] added display of process tasks in the terminal [#5895](https://github.com/theia-ide/theia/pull/5895)
- [task] added multi-root support to "configure task" and customizing tasks in `tasks.json` [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] added support for VSCode task contribution points: `taskDefinitions`, `problemMatchers`, and `problemPatterns` [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] added the display of configured tasks when executing `configure tasks...` [#5472](https://github.com/theia-ide/theia/pull/5472)
- [task] allowed users to override any task properties other than the ones used in the task definition [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] changed the way that "configure task" copies the entire task config, to only writing properties that define the detected task plus [#5777](https://github.com/theia-ide/theia/pull/5777)`problemMatcher`, into `tasks.json`
- [task] displayed the customized tasks as "configured tasks" in the task quick open [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] fixed the problem where a detected task can be customized more than once [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] notified clients of TaskDefinitionRegistry on change [#5915](https://github.com/theia-ide/theia/pull/5915)
- [task] updated `isVisible` and `isEnabled` handling for `Run Selected Text` [#6018](https://github.com/theia-ide/theia/pull/6018)
- [task] added support for removing all data from tasks.json [#6033](https://github.com/theia-ide/theia/pull/6033)
- [task] updated compare task to use task definitions [#5975](https://github.com/theia-ide/theia/pull/5975)
- [terminal] added a preference `terminal.integrated.scrollback` to control the terminal scrollback [#5783](https://github.com/theia-ide/theia/pull/5783)
- [vscode] added support for `command` variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] added support for `config` variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] added support for `execPath` variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] added support for `inputs` variable substitution for debug [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] added support for `selectedText` variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] added support for `when` closure for views [#5855](https://github.com/theia-ide/theia/pull/5855)
- [vscode] added support for environment variable substitution [#5811](https://github.com/theia-ide/theia/pull/5811)
- [vscode] added support for workspace scoped variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
- [vscode] fixed resolution of environment variables [#5835](https://github.com/theia-ide/theia/pull/5835)

Breaking changes:

- [core] refactored `TreeDecoration` to `WidgetDecoration` and moved it to shell, since it is a generic decoration that can be used by different types of widgets (currently by tree nodes and tabs) [#5845](https://github.com/theia-ide/theia/pull/5845)
- [plugin]refactored  files from 'plugin-ext/src/api' moved to 'plugin-ext/src/common', renamed 'model.ts' to 'plugin-api-rpc-model.ts', 'plugin-api.ts' to 'plugin-api-rpc.ts'
- [shell][plugin] integrated view containers and views [#5665](https://github.com/theia-ide/theia/pull/5665)
  - `Source Control` and `Explorer` are view containers now and previous layout data cannot be loaded for them. Because of it the layout is completely reset.
- [task] `TaskService.getConfiguredTasks()` returns `Promise<TaskConfiguration[]>` instead of `TaskConfiguration[]` [#5777](https://github.com/theia-ide/theia/pull/5777)
- [task] ensured that plugin tasks are registered before accessing them [5869](https://github.com/theia-ide/theia/pull/5869)
  - `TaskProviderRegistry` and `TaskResolverRegistry` are promisified
- [task] removed `filterDuplicates()` from `TaskConfigurations` class [#5915](https://github.com/theia-ide/theia/pull/5915)
- [vscode] completed support of variable substitution [#5835](https://github.com/theia-ide/theia/pull/5835)
  - inline `VariableQuickOpenItem`

## v0.9.0

- [core] added `theia-widget-noInfo` css class to be used by widgets when displaying no information messages [#5717](https://github.com/theia-ide/theia/pull/5717)
- [core] added additional options to the tree search input [#5566](https://github.com/theia-ide/theia/pull/5566)
- [core] added fix to prevent the IDE from scrolling along with the text on mobile (e.g. on iPad) [#5742](https://github.com/theia-ide/theia/pull/5742)
- [core] added view container layout changes [#5536](https://github.com/theia-ide/theia/pull/5536)
- [core] fixed the alignment of the expansion icon [#5677](https://github.com/theia-ide/theia/pull/5677)
- [core] fixed the toolbar item comparator [#5624](https://github.com/theia-ide/theia/pull/5624)
- [core] updated quick-open UI [#5733](https://github.com/theia-ide/theia/pull/5733)
- [cpp] added the ability to run `clang-tidy` as a task [#5533](https://github.com/theia-ide/theia/pull/5533)
- [debug] fixed behavior of creating launch configurations always under the '.theia' folder [#5678](https://github.com/theia-ide/theia/pull/5678)
- [debug] updated to ensure that node-based debug adapters spawn the same node executable as Theia [#5508](https://github.com/theia-ide/theia/pull/5508)
- [doc] updated `node.js` prerequisites [#5643](https://github.com/theia-ide/theia/pull/5643)
- [editor] added `Toggle Minimap` command [#5633](https://github.com/theia-ide/theia/pull/5633)
- [filesystem] disposed the clipboard copy listener [#5709](https://github.com/theia-ide/theia/pull/5709)
- [filesystem] fixed file dialog opening folder [#4868](https://github.com/theia-ide/theia/pull/4868)
- [filesystem] fixed scaling issues of save and file dialogs in small viewports [#5688](https://github.com/theia-ide/theia/pull/5688)
- [filesystem] improved the download of large files [#5466](https://github.com/theia-ide/theia/pull/5466)
- [git] improved the support for empty Git repositories in the `Git` and `Git History` view [#5484](https://github.com/theia-ide/theia/pull/5484)
- [keymaps] added the `Reset` button directly when attempting to update a command's keybinding [#5603](https://github.com/theia-ide/theia/pull/5603)
- [keymaps] aligned the keybindings widget with VSCode [#5545](https://github.com/theia-ide/theia/pull/5545)
- [markers] added support for `Information` diagnostic severity [#5763](https://github.com/theia-ide/theia/pull/5763)
- [markers] enabled single-click and keyboard arrow selection to navigate problem markers [#5646](https://github.com/theia-ide/theia/pull/5646)
- [messages] fixed the button positioning when displaying messages with a multiple lines of text [#5657](https://github.com/theia-ide/theia/pull/5657)
- [monaco] added re-detect languages on new grammar [#5754](https://github.com/theia-ide/theia/pull/5754)
- [monaco] fixed textmate highlighting when changing themes [#5728](https://github.com/theia-ide/theia/pull/5728)
- [monaco] fixed the alignment of the file icon in the quick-open menus [#5725](https://github.com/theia-ide/theia/pull/5725)
- [plugin-dev] added the path in the PluginFolder notification [#5731](https://github.com/theia-ide/theia/pull/5731)
- [plugin-dev] fixed the run/debug flow on Windows [#5608](https://github.com/theia-ide/theia/pull/5608)
- [plugin-ext] fixed the display of webview icons in the sidepanel [#5723](https://github.com/theia-ide/theia/pull/5723)
- [plugin-ext] fixed workspace name getter when no folders are opened [#5588](https://github.com/theia-ide/theia/pull/5588)
- [plugin] added support of debug activation events [#5645](https://github.com/theia-ide/theia/pull/5645)
- [plugin] fixed `converting circular structure to JSON` error [#5661](https://github.com/theia-ide/theia/pull/5661)
- [plugin] fixed auto detection of new languages [#5753](https://github.com/theia-ide/theia/issues/5753)
- [plugin] fixed plugin loading to better support modules that have immutable exports [#5520](https://github.com/theia-ide/theia/pull/5520)
- [plugin] improved `node.js` error handling [#5695](https://github.com/theia-ide/theia/pull/5695)
- [scm] fixed the alignment of the status item [#5729](https://github.com/theia-ide/theia/pull/5729)
- [search-in-workspace] added 'title' to search result nodes [#5628](https://github.com/theia-ide/theia/pull/5628)
- [search-in-workspace] added the `search.collapseResults` preference to the search-in-workspace widget [#5686](https://github.com/theia-ide/theia/pull/5686)
- [search-in-workspace] fixed issue which displayed 'No results found' while a user types their search [#5701](https://github.com/theia-ide/theia/pull/5701)
- [search-in-workspace] improved the ordering of the search results [#5669](https://github.com/theia-ide/theia/pull/5669)
- [search-in-workspace] updated the `Replace All` disabled state [#5611](https://github.com/theia-ide/theia/pull/5611)
- [security] updated the version of `lodash.mergewith` from 4.6.1 to 4.6.2 [#5700](https://github.com/theia-ide/theia/pull/5700)
- [task] added support for Linux and OSX specific command properties [#5579](https://github.com/theia-ide/theia/pull/5579)
- [task] added support for VSCode task contribution points: `taskDefinitions`, `problemMatchers`, and `problemPatterns` [#5024](https://github.com/theia-ide/theia/pull/5024)
- [task] disposed task listeners and emitters when necessary [#5024](https://github.com/theia-ide/theia/pull/5024)
- [terminal] implemented `Show All Opened Terminals` quick-open menu [#5577](https://github.com/theia-ide/theia/pull/5577)
- [terminal] updated `processId` and `cwd` to return a rejected promise instead of throwing an error [#5553](https://github.com/theia-ide/theia/pull/5553)
- [vscode] added unzipping of node_modules for built-in extensions [#5756](https://github.com/theia-ide/theia/pull/5756)
- [workspace] added handling to not re-open a workspace that is currently opened [#5632](https://github.com/theia-ide/theia/pull/5632)
- [workspace] fixed path variables on Windows [#5741](https://github.com/theia-ide/theia/pull/5741)

Breaking changes:

- [plugin] activate dependencies before activating a plugin [#5661](https://github.com/theia-ide/theia/pull/5661)
- [plugin] added basic support of activation events [#5622](https://github.com/theia-ide/theia/pull/5622)
  - `HostedPluginSupport` is refactored to support multiple `PluginManagerExt` properly
  - Theia plugins should declare the `"activationEvents": ["*"]` entry in the root of the `package.json`. Otherwise, they won't start at app startup. See [#5743](https://github.com/theia-ide/theia/issues/5743) for more details.
- [plugin] added support of `workspaceContains` activation events [#5649](https://github.com/theia-ide/theia/pull/5649)
- [plugin] fixed typo in 'HostedInstanceState' enum from RUNNNING to RUNNING in `plugin-dev` extension [#5608](https://github.com/theia-ide/theia/pull/5608)
- [plugin] removed member `processOptions` from `AbstractHostedInstanceManager` as it is not initialized or used [#5608](https://github.com/theia-ide/theia/pull/5608)


## v0.8.0

- [core] added bépo keyboard layout
- [core] added sorting to the extension names in the about dialog
- [core] added sorting to the prefixed quick-open commands
- [core] added support for octicon icons in the statusbar
- [core] allowed passing of command args to context menus
- [core] added the ability to rebind the `BrowserMenuBarContribution`
- [core] fixed issue with webview resizing
- [core] fixed label encoding for diff uris
- [cored] added `TextareaAutosize` for textarea resizing
- [debug] added throttling to the debug console output
- [debug] fixed breakpoint resizing error in the debug-widget
- [editor] added the ability to rebind the `EditorWidgetFactory`
- [editor] implemented `Show All Opened Editor` command and quick-open menu
- [editor] removed the 'dirty' state of an editor if changes are reverted
- [electron] fixed issue when exiting Electron based applications
- [electron] improved startup performance
- [filesystem] improved animation when dragging and dropping multiple files
- [keymaps] added a toolbar item to open the keymaps.json
- [keymaps] added command to `Open Keyboard Shortcuts (JSON)`
- [keymaps] added toolbar item to clear keybindings-widget search
- [keymaps] enhanced the keybindings-widget search to support different key orders
- [keymaps] fixed the display of key chords in the keybindings-widget
- [keymaps] updated the UI of the keybindings-widget when resizing
- [monaco] fixed overflow with editor hints
- [navigator] added VSCode-like compare for files
- [navigator] added ability to select for compare
- [plugin] added VSCode API to register `DebugAdapterTrackerFactory`
- [plugin] added `setTextDocumentLanguage` Plug-in API
- [preview] added scrolling synchronization between editor and preview
- [preview] fixed issue where preview images were broken
- [problems] added `copy` and `copy message` features to the problems-widget
- [problems] fixed the problem-widget markers from wrapping when resizing
- [task] added the ability to add comments in tasks.json
- [task] added the display of the source folder name for detected tasks in the quick-open
- [task] added the task label in the terminal title when executing tasks
- [task] implemented `Show Running Tasks...` command and quick-open menu
- [terminal] implemented `Terminate Task...` command and quick-open menu

Breaking changes:

- [core] `scheme` is mandatory for URI
  - `URI.withoutScheme` is removed, in order to get a path use `URI.path`
- [core] `SelectionCommandHandler.getMulitSelection()` is renamed into `SelectionCommandHandler.getMultiSelection()`
- [debug] align commands with VS Code [#5102](https://github.com/theia-ide/theia/issues/5102)
    - `debug.restart` renamed to `workbench.action.debug.restart`
- [plugin] 'Hosted mode' extracted in `plugin-dev` extension
- [preferences] removed constructor from the `FolderPreferenceProvider` class
- [preferences] renamed overridenPreferenceName to overriddenPreferenceName
- [task] `cwd`, which used to be defined directly under `Task`, is moved into `Task.options` object
- [workspace] `isMultiRootWorkspaceOpened()` is renamed into `isMultiRootWorkspaceEnabled()`
- [filesystem] Changed `FileDownloadService` API to support streaming download of huge files.

## v0.7.0

- [console] added `Clear Console` command and toolbar item
- [console] fixed issue where the debug console auto-scrolls when is it located at the bottom
- [core] added command to manually choose a keyboard layout
- [core] added functionality for the toolbar to respond to mouse events
- [core] added launch preferences support
- [core] added preference to control the number of recently used items to display
- [core] added support for recently used commands
- [core] added support for several international keyboard layouts
- [core] added the command `Clear Command History`
- [core] fixed issue allowing the load of Theia in an iframe over a protected connection
- [core] implemented auto-detection of keyboard layout based on pressed keys
- [core] updated monaco configurations on default preference changes
- [cpp] added support for OpenCL file types
- [debug] added support for debug configuration prefixed quick-open menu
- [electron] added the command `Close Window`
- [file-upload] fixed reporting uploaded URIs
- [filesystem] added support for multiple files drag and drop
- [java] added new preference to add command line arguments when starting language server
- [markers] added `Collapse All` toolbar item to the problems-widget
- [mini-browser] fixed issue where the mini-browser resizes unnecessarily
- [monaco] removed overriding dark-plus theming
- [navigator] added the command `Collapse Folders in Explorer`
- [navigator] fixed the commands `Remove Folder` and `Add Folder`
- [outline] added informative tooltips to outline view items
- [plugin-ext] added `onDidEndTaskProcess` Plug-in API
- [plugin-ext] added `onDidStartTaskProcess` Plug-in API
- [plugin-ext] added ability to match browser displayed nodes with the plugin created node
- [plugin-ext] added additional command to install VSCode extensions
- [plugin-ext] added support for inline actions
- [plugin-ext] aligned views with Theia styles
- [plugin-ext] fixed he loading of icons
- [plugin-ext] fixed issue of overriding preferences
- [plugin-ext] fixed issue to support single source deployment state
- [plugin-ext] fixed issue where the hosted plugin instance did not properly stop
- [plugin-ext] fixed plugin folder path in Windows
- [plugin-ext] fixed the rendering of png icons
- [plugin-ext] implemented command `workbench.action.reloadWindow`
- [plugin] added file management vscode commands
- [plugin] fixed plugin export
- [preferences] added additional information to the preference tooltips
- [process] added link matcher for local files
- [process] normalized task types and processes
- [tabbar] fixed widget leaking via phosphor VDOM
- [terminal] added ability to activate links with `cmd + click`
- [terminal] added support for basic link matching
- [terminal] fixed random 1px white border in Firefox
- [typescript] fixed broken code actions
- [workspace] allowed `WorkspaceCommandContribution` to be re-bindable by extensions
- [xterm] upgraded xterm to fix terminal dragging between areas

Breaking changes:

- [filesystem] extracted `FileUploadService` and refactored `FileTreeWidget` to use it [#5086](https://github.com/theia-ide/theia/pull/5086)
  - moved `FileDownloadCommands.UPLOAD` to `FileSystemCommands.UPLOAD`
- [git] bind Git UI to SCM
- [output] moved the channel selection and clear icons to the toolbar.
  - The CLEAR_BUTTON and OVERLAY constants are no longer available. Furthermore OutputChannelManager API has changed.
- [preferences] refactored to integrate launch configurations as preferences
- [scm] added Source Control Model
- [core] renamed the `src/electron-main` folder to `src/electron-node` in `@theia/core`. Removed `preventStop` from the `FrontendApplication` API. Move the `DefaultWindowService` class into its own module.

## v0.6.0

- Allowed the creation of sub-files and/or sub-folders if name has `/`
- [core] added `files.enableTrash` preference
- [core] added support for custom React toolbar widgets
- [core] added support for tail decorators
- [core] aligned the statusbar styles with VSCode
- [core] updated the prefix quick-open service to support `actionProviders`
- [cpp] added support for block comment auto-closing pairs
- [editor-preview] fixed error at application startup if no preview editors are opened
- [editor-preview] fixed the `goToDefinition` failure when in editor preview mode
- [electron] added the ability to run plugins by binding the components on the backend
- [electron] added the configure Plug-ins option to the start script
- [electron] updated Electron to include a `minWidth` and `minHeight`
- [electron] upgraded version of Electron used to version 3
- [filesystem] added the menu item `Upload Files...` to easily upload files into a workspace
- [filesystem] implemented `Save As` including a save dialog, and new command
- [filesystem] updated the handling when attempting to perform copying when the source and target are the same
- [git] added ability to toggle `Git History` widget
- [git] fixed `Discard All` alignment when the `Git` widget is too narrow
- [git] fixed `Git History` widget alignment and behavior issues
- [git] updated the ahead/behind icons on the statusbar
- [keyboard] aligned the file and event naming conventions
- [languages] updated error type for backwards compatibility
- [plugin-ext] fixed the Plug-in path selection dialog for the hosted instance
- [plugin] added `CodeActionKind` `intersects` Plug-in API
- [plugin] added necessary Webview Plug-in APIs
- [plugin] added propagation of `thisArg` on `registerCommand`
- [plugin] added support for Gulp, Jake, Grunt Plug-in extensions
- [plugin] added support for extensions without activation functions
- [plugin] added the ability to choose through the CLI which VSCode API version to use
- [plugin] aligned `window.setStatusBarMessage` with VSCode
- [plugin] fixed `vscode.open` command by adding checks on arguments
- [plugin] fixed implementation of `vscode.diff` command
- [plugin] fixed issue where webviews were not focused or revealed properly
- [plugin] fixed memory leak on Plug-ins reload
- [plugin] fixed serialization of `Range` object
- [plugin] fixed the registration of text decoration keys
- [plugin] updated Plug-in language services to hook in monaco cancellation tokens
- [preferences] added ability to override default application preference values
- [search-in-workspace] added the ability to pass the currently selected editor text when searching
- [security] fixed XSS vulnerability
- [task] added command to clear task history
- [task] added support to configure tasks
- [task] added the ability to configure tasks
- [task] added the ability to display recently used tasks
- [task] updated the tasks quick-open menu including alignment, category labels and borders
- [terminal] updated terminal preference's minimum value for `lineHeight` and `fontSize`
- [textmate-grammars] added php grammar
- [textmate-grammars] added rust grammar
- [textmate-grammars] fixed incorrect jsx scope
- [tree] added support for icons in node tail decorators
- [workspace] allowed the creation of files and folders using recursive paths
- [workspace] fixed incorrect file-icon when displaying recent workspaces

Breaking changes:

- [core] added support native keyboard layouts [#4724](https://github.com/theia-ide/theia/pull/4724)
- [dialog] updated `validate` and `accept` methods so they are now Promisified [#4764](https://github.com/theia-ide/theia/pull/4764)
- [editor] turned off autoSave by default to align with VSCode [#4777](https://github.com/theia-ide/theia/pull/4777)
  - default settings can be overridden in application package.json:
  ```json
  {
    "private": true,
    "name": "myapp",
    "theia": {
      "frontend": {
        "config": {
          "preferences": {
            "editor.autoSave": "on"
          }
        }
      }
    }
  }
  ```
- [electron] removed cluster mode and startup timeout setting
- [electron] updated Electron to make runtime dependencies optional [#4873](https://github.com/theia-ide/theia/pull/4873)
- [extension-manager] deprecated [#4876](https://github.com/theia-ide/theia/pull/4876)
- [node] moved to using Node.js version 10, dropping support for Node.js version 8

## v0.5.0

- Added `scope` to task configurations to differentiate 3 things: task type, task source, and where to run tasks
- [core] added implementation for toolbar support for sidepanels and changed sidepanel tabs
- [core] added new keybinding <kbd>alt</kbd>+<kbd>shift</kbd>+<kbd>w</kbd> to close all main area tabs
- [core] added the ability to make sidebar widgets closable
- [core] fixed `ToolbarAwareTabBar` detachment errors
- [core] fixed broken wheel listener
- [core] improved scrollbar styling
- [core] updated tabbar toolbar to use VSCode icons
- [core] updated the UI with numerous improvements including sidepanel icons, better alignment, tabbar and menu size
- [cpp] added new `cpp.clangTidy `and `cpp.clangTidyChecks` preferences to lint cpp program when clangd v9+ is used
- [cpp] fixed properly restarting clangd language server when changing cpp build configurations
- [debug] added new debug preferences to control `view`, `console`, and `location` appearance
- [editorconfig] added support to apply properties to monaco editor when opening/switching editors
- [file-search] improved ordering and consistency of file search results
- [filesystem] added `files.associations` property
- [filesystem] improved the performance when deleting large directories
- [filesystem] upgraded `nsfw` file-watching dependency from `vscode-nsfw` to `Axosoft/nsfw` which fixes memory leaks as well as fixes issues where files are not being properly watched outside the main watched directory
- [git] fixed issue where Theia did not refresh the git view after deleting the only repository
- [git] improved the git diff navigation header to be static
- [java] improved handling of incomplete classpath commands
- [keybindings] improved the keybindings widget search and table header to be static
- [mini-browser] improved error handling of iframe errors
- [navigator] added `Collapse All` toolbar item
- [navigator] updated the navigator to handle multi-root workspaces better
- [plugin-ext] added `workspace.onDidRenameFile ` Plug-in API
- [plugin-ext] added `workspace.onWillRenameFile ` Plug-in API
- [plugin-ext] added `workspace.registerFileSystemProvider` Plug-in API
- [plugin-ext] added `workspace.saveAll` Plug-in API
- [plugin-ext] added `workspace.updateWorkspaceFolders` Plug-in API
- [plugin-ext] added ability to proceed `runInTerminal` requests in sidecar containers
- [plugin-ext] added the ability to get selection context after executing a command
- [plugin-ext] fixed VSCode Plug-in API incompatibilities for the `onDidChangeActiveTextEditor` event
- [plugin-ext] fixed firing the `onWillSaveTextDocument` event
- [plugin-ext] fixed issue of re-deploying already initialized plugins
- [plugin] `workspace.openTextDocument` API now respects the contributed `FileSystemProviders`
- [plugin] added support for multiple windows per backend
- [plugin] fixed progress creation
- [plugin] improved the view container to use the native toolbar
- [preferences] fixed content assist when editing `settings.json`
- [preferences] fixed parsing of settings from workspace files
- [preferences] improved overriding of default configurations
- [preview] fixed issue when opening images
- [search-in-workspace] added a new preference `search.lineNumbers` to control whether to show line numbers for search results
- [task] added ability to `Run Selected Text`
- [task] added new command to re-run the last task
- [task] added schema support for `tasks.json`
- [typehierarchy] added the new type hierarchy extension
- [typehierarchy] improved `typehierarchy` to use all levels the language server sends if available
- [workspace] added new `package.json` properties `newFIleName` and `newFileExtension` to specify default file name and extension when creating a new file
- [workspace] improved performance of the file rename action for large directories

Breaking changes:

- [editor] computation of resource context keys moved to core [#4531](https://github.com/theia-ide/theia/pull/4531)
- [plugin] support multiple windows per a backend [#4509](https://github.com/theia-ide/theia/issues/4509)
  - Some plugin bindings are scoped per a connection now. Clients, who contribute/rebind these bindings, will need to scope them per a connection as well.
- [quick-open] disable separate fuzzy matching by default [#4549](https://github.com/theia-ide/theia/pull/4549)
- [shell] support toolbars in side bars [#4600](https://github.com/theia-ide/theia/pull/4600)
  - In side bars a widget title is rendered as an icon.

## v0.4.0

- [application-manager] added support for pre-load HTML templates
- [console] added support for console `when` contexts
- [core] added support for os `when` contexts
- [core] added support for shell `when` contexts
- [core] added support for vscode closure contexts
- [core] fixed bad vertical resizing behavior
- [core] improved scrollbar visibility for the command palette
- [core] improved tab-bar display (display 'X' (close) on dirty editors when hovering over dirty icon)
- [core] improved tab-bar display (display 'X' (close) only when current editor is active, or has hover)
- [cpp] fixed `CPP_CLANGD_COMMAND` and `CPP_CLANGD_ARGS` environment variables
- [cpp] fixed the update of the active build config statusbar when preferences are updated
- [cpp] implemented the command `Create New Build Configuration`
- [cpp] implemented the command `Reset Build Configuration`
- [cpp] removed duplicate json config entry generated by the command `New Build Config`
- [debug] added support for debug mode `when` contexts
- [editor] added `Clear Editor History` command
- [editor] added support for editor `when` contexts
- [editor] added support for resource `when` contexts
- [editor] registered editor to navigation location stack when `onCurrentEditorChange` event is fired
- [electron] improved opening markdown links by opening them in the OS' default browser
- [electron] stored the last state of window geometry
- [file-search] added separator between recently opened items, and file results when executing the quick file open
- [file-search] added support for ignored globs and limit in file search
- [file-search] improved quick open file sort order
- [file-search] removed git diff editors from displaying the quick file open
- [file-search] added support for `glob` file searches
- [file-search][plugin-ext] updated `exclude` of file search
- [git] added the following git commands: `Stash`, `Apply Stash`, `Apply Latest Stash`, `Pop Stash`, `Pop Latest Stash` and `Drop Stash`
- [git] enhanced `Git Remote` command to obtain complete data
- [git] fixed refreshing the `GitView` when git repo changes
- [git] fixed the command `Git Reset`
- [git] removed bundled git from `dugite`
- [languages] fixed clash in language server session ids
- [messages] added support for notification `when` contexts
- [mini-browser] added ability to pass argument for `openUrl` command
- [monaco] added support for quick open `when` contexts
- [monaco] added support for snipped mode `when` contexts
- [navigator] added support for explorer `when` contexts
- [navigator] fixed updating the navigator context menu on `supportMultiRootWorkspace` preference change
- [plugin-ext-vscode] added ability to handle `vscode.diff` and open diff editor commands
- [plugin-ext-vscode] added vscode `setContext` command
- [plugin-ext-vscode] fixed local resource loading in webviews
- [plugin-ext] fixed `TreeView` widget registration
- [plugin-ext] fixed `onDidSelectItem` behavior for the quick pick widget
- [plugin-ext] fixed command conversions for code lens
- [plugin-ext] fixed issue of `OutputChanel.show` not displaying
- [plugin-ext] fixed miscellaneous issues in golang plugin
- [plugin-ext] implemented `onWillSaveTextDocument` event handler
- [plugin-ext][markers] added support to use problem manager to handle plugin markers
- [plugin] added `tasks.onDidEndTask` Plug-in API
- [plugin] added `tasks.taskExecutions` Plug-in API
- [plugin] added ability to display webview panel in 'left', 'right' and 'bottom' area
- [plugin] added support for `menus.commandPalette` contribution point
- [plugin] added support for `vscode.previewHtml` command
- [plugin] added support for read-only configuration index access
- [plugin] fixed issue of ensuring statusbar entry uniqueness
- [plugin] implemented inspect configuration command
- [plugin] refactored the `Command` interface by splitting into two: `CommandDescription` and `Command`
- [plugin][debug] added ability to connect to a remote debug server
- [preferences] added support for language specific preferences
- [preferences] aligned preference default values by type with vscode
- [search-in-workspace] added support for search `when` contexts
- [search-in-workspace] fixed keybinding for `Search in Workspace` widget
- [terminal] added support for font preferences
- [terminal] added support for terminal `when` contexts
- [vscode] added support for OS specific keybindings
- [vscode] implemented `commands.getCommands`
- [vscode] implemented `commands.registerTextEditorCommand`
- [vscode] implemented `workspace.rootPath`
- [workspace] added support for easier overriding of the `DefaultWorkspaceServer`
- [workspace] added support for workspace `when` contexts
- [workspace] fixed displaying the `Open With...` context menu only when more than one open handler is present
- [mini-browser] improved handling of iframe errors and time-outs

Breaking changes:

- menus aligned with built-in VS Code menus [#4173](https://github.com/theia-ide/theia/pull/4173)
  - navigator context menu group changes:
    - `1_open` and `4_new` replaced by `navigation` group
    - `6_workspace` renamed to `2_workspace` group
    - `5_diff` renamed to `3_compare` group
    - `6_find` renamed to `4_search` group
    - `2_clipboard` renamed to `5_cutcopypaste` group
    - `3_move` and `7_actions` replaced by `navigation` group
  - editor context menu group changes:
    - `2_cut_copy_paste` renamed to `9_cutcopypaste` group
- [debug] align commands with VS Code [#4204](https://github.com/theia-ide/theia/issues/4204)
    - `debug.breakpoint.toggle` renamed to `editor.debug.action.toggleBreakpoint`
    - `debug.start` renamed to `workbench.action.debug.start`
    - `debug.thread.continue` renamed to `workbench.action.debug.continue`
    - `debug.start.noDebug` renamed to `workbench.action.debug.run`
    - `debug.thread.pause` renamed to `workbench.action.debug.pause`
    - `debug.thread.stepin` renamed to `workbench.action.debug.stepInto`
    - `debug.thread.stepout` renamed to `workbench.action.debug.stepOut`
    - `debug.thread.next` renamed to `workbench.action.debug.stepOver`
    - `debug.stop` renamed to `workbench.action.debug.stop`
    - `debug.editor.showHover` renamed to `editor.debug.action.showDebugHover`
- multi-root workspace support for preferences [#3247](https://github.com/theia-ide/theia/pull/3247)
  - `PreferenceProvider`
    - is changed from a regular class to an abstract class
    - the `fireOnDidPreferencesChanged` function is deprecated. `emitPreferencesChangedEvent` function should be used instead. `fireOnDidPreferencesChanged` will be removed with the next major release.
  - `PreferenceServiceImpl`
    - `preferences` is deprecated. `getPreferences` function should be used instead. `preferences` will be removed with the next major release
  - having `properties` property defined in the `PreferenceSchema` object is now mandatory
  - `PreferenceProperty` is renamed to `PreferenceDataProperty`
  - `PreferenceSchemaProvider`
    - the type of `combinedSchema` property is changed from `PreferenceSchema` to `PreferenceDataSchema`
    - the return type of `getCombinedSchema` function is changed from `PreferenceSchema` to `PreferenceDataSchema`
  - `affects` function is added to `PreferenceChangeEvent` and `PreferenceChange` interface
- `navigator.exclude` preference is renamed to `files.exclude` [#4274](https://github.com/theia-ide/theia/pull/4274)

## v0.3.19

- [core] added `hostname` alias
- [core] added new `editor.formatOnSave` preference, to format documents on manual save
- [core] added support for setting end of line character
- [cpp] added new `cpp.clangdExecutable` and `cpp.clangdArgs` to customize language server start command
- [debug] added node debugger as a Plug-in
- [debug] added support for source breakpoints
- [git] added `discardAll` command
- [git] added `stageAll` command
- [git] added `unstageAll` command
- [git] added new `git pull` command, to pull from default configured remote
- [git] added new `git push` command, to push from default configured remote
- [git] added the ability to refresh git repositories when a change is detected within a workspace
- [java] allow the ability to rebind `JavaContribution`
- [languages] enabled INI syntax highlighting for `.properties` and `.toml` files
- [monaco] fixed cross editor navigation
- [monaco] fixed document-saving that took too long
- [monaco] improved `MonacoWorkspace.fireWillSave` performance
- [plugin] added `globalState` and `workspaceState` Plug-in API
- [plugin] added `registerColorProvider` Plug-in API
- [plugin] added `registerRenameProvider` Plug-in API
- [plugin] added `tasks.onDidStartTask` Plug-in API
- [plugin] added basic support of snippets
- [plugin] added common service to handle `when` expressions
- [plugin] added debug Plug-in API
- [plugin] added support for terminal APIs on window
- [plugin] added the ability to debug VS Code extensions
- [plugin] added the ability to get operating system connected to Plug-in
- [plugin] added the ability to provide a way to initialize workspace folders when Theia is started
- [plugin] added the ability to set the visibility of menu items through `when` expressions
- [plugin] added workspace symbols Plug-in API
- [plugin] fixed spreading of command arguments
- [preferences] added the ability to update settings schema resource on schema changes
- [search-in-workspace] fixed issue regarding child root in `search-in-workspace` when there is a multiple-root workspace
- [search-in-workspace] removed duplicates from `search-in-workspace` tree
- [security] updated xterm.js to 3.9.2
- [task] added support to run tasks from multiple-roots
- [task] fixed cwd path
- [workspace] added multiple-root support for `WorkspaceService.getWorkspaceRootUri()`

## v0.3.18

- [core] added a preference to define how to handle application exit
- [core] added a way to prevent application exit from extensions
- [core] added functionality to prevent application exit if some editors are dirty
- [core] allowed the ability to scope bindings per connection
- [core] fixed `@theia/core/lib/node/debug#DEBUG_MODE` flag to correctly detect when the runtime is inspected/debugged
- [cpp] fixed clangd being prematurely started when a build config is active
- [electron] implemented HTTP-based authentication for Git
- [electron] updated Electron to `^2.0.14`
- [electron] updated Git for Electron to fall back to embedded Git if no Git is found on the `PATH`
- [file-search] added ability to search files from multiple-root workspaces
- [file-search] improved handling when attempting to open non-existent files from the `quick-open-file`
- [filesystem] added the ability to convert URIs to platform specific paths
- [git] updated Git view to display short hash when on detached state
- [java-debug] added major enhancements to `java-debug`
- [keybinding] normalized key sequences to US layout
- [languages] added a preference for every language contribution to be able to trace the communication client <-> server
- [languages] allowed the ability to provide Language Server start options
- [languages] fixed leaking language clients
- [languages][java] reuse `jdt.ls` workspace
- [monaco] fixed keybindings on OSX
- [plug-in] added Plug-in API for language server contributions
- [plug-in] added `storagePath` Plug-in API
- [plug-in] added `tasks.registerTaskProvider` Plug-in API
- [plug-in] added `window.withProgress` Plug-in API
- [plug-in] added ability to register keybindings from a Plug-in's `package.json`
- [plug-in] added open link command
- [plug-in] added support for context menus in contributed views
- [plug-in] implemented API to get workspace folder by a given file URI
- [plug-in][languages] added ability to register a document highlight provider
- [search-in-workspace] added ability to perform 'Find in Folder...' with multiple folders simultaneously
- [search-in-workspace] added match and file count to search-in-workspace
- [search-in-workspace] added support for multiple-root workspaces
- [search-in-workspace] fixed path issues by instead using URIs
- [terminal] added ability to choose terminal root location when a workspace contains multiple roots
- [workspace] fixed long label computations for multiple-root workspaces
- [xterm] updated Xterm to `3.9.1`

## v0.3.17

- Added better widget error handling for different use cases (ex: no workspace present, no repository present, ...)
- Addressed multiple backend memory leaks
- Prefixed quick-open commands for easier categorization and searching
- Refactored `Task` menu items into the new `Terminal` menu
- [core] added `theia.applicationName` to application `package.json` and improved window title
- [core] added graceful handling of init and re-connection errors
- [core] added the keybinding `ctrl+alt+a` and `ctrl+alt+d` to switch tabs left/right
- [core] added the menu item `Find Command...` to easily trigger quick-open commands
- [core] added toolbar support for tab-bars
- [core] updated the status-bar display when offline
- [cpp] updated the keybinding for `Switch Header/Source` from `Option+o` to `Option+Command+o` when on macOS
- [debug] added the ability to fork a debug adapter
- [debug] added the ability to trace the debug adapter communication
- [debug] implemented major frontend and backend debug improvements
- [electron] miscellaneous stability and usability improvements on Electron
- [getting-started] added `Getting Started Widget` - used to view common commands, recent workspaces, and helpful links
- [lsp] added new symbol types and increased existing workspace symbol resilience
- [lsp] registered 'Restart' commands for each language server started for miscellaneous purposes
- [markers] added the context menu item `Collapse All` for problem markers
- [mini-browser] miscellaneous mini-browser improvements
- [plug-in] added Plug-in API to communicate between Theia and plugins
- [plug-in] added `languages.registerCodeLensProvider` Plug-in API
- [plug-in] added `languages.registerDocumentSymbolProvider` Plug-in API
- [plug-in] added `window.showTextDocument` Plug-in API
- [plug-in] added ability to provide custom namespaces for the Plug-in API
- [plug-in] registered a type definition provider
- [plug-in] added `tasks.registerTaskProvider` Plug-in API
- [preview-editor] added the ability to open editors in preview mode
- [process] added the ability to create new node processes through forking
- [search-in-workspace] prompted users when performing `Replace All...` to limit accidental triggering
- [search-in-workspace] fixed issue when selecting a file, the command `Find in Folder...` searches from the node's closest parent
- [terminal] added the menu item and command `Split Terminal`
- [workspace] added the ability to open multiple files simultaneously from the file navigator
- [workspace] added the context menu item `Collapse All` for the file navigator
- [workspace] included workspace path as part of the URL fragment

## v0.3.16

- Reverted [cpp] Add debugging for C/C++ programs. This feature will come back in its own cpp-specific repo
- [callhierarchy][typescript] adapt to hierarchical document symbols
- [core] added methods to un-register menus, commands and keybindings
- [debug] decoupled debug model from UI + clean up
- [markers] added ability to remove markers
- [output] added a button to clear output view
- [plug-in] Terminal.sendText API adds a new line to the text being sent to the terminal if `addNewLine` parameter wasn't specified
- [plug-in] added `DocumentLinkProvider` Plug-in API
- [terminal] added 'open in terminal' to navigator
- [windows] implemented drives selector for the file dialog

## v0.3.15

- [cpp] added debugging for C/C++ programs
- [debug] added debug toolbar
- [debug] resolved variables in configurations
- [debug] updated debug session views to act like panels
- [keymaps] added new `View Keybindings Widget` - used to view search and edit keybindings
- [languages] added TCL grammar file
- [plug-in] added `menus` contribution point
- [workspace] added multi-root workspace support with vscode compatibility

## v0.3.13

- Re-implemented additional widgets using React
- Re-implemented miscellaneous components using React
- [cpp] added a status bar button to select an active cpp build configuration
- [cpp] implemented watch changes to compile_commands.json
- [git/blame] added support for convert to toggle command
- [markers] fixed #2315: fine grain marker tree computation
- [markers] improved performance by no longer storing markers in browser local storage by default
- [terminal] updated to xterm.js 3.5.0
- [textmate] added C/C++, Java, Python, CSS, html, less, markdown, shell, xml, yaml
- [tree] improved performance by not rendering collapsed nodes
- [ts] added support for one ls for all JavaScript related languages
- [workspace] added support for recently opened workspaces history

## v0.3.12

- New Plugin system !
  - See [design](https://github.com/theia-ide/theia/issues/1482) and [documentation](https://github.com/theia-ide/theia/blob/master/packages/plugin/API.md) for more details.
- Introducing [Task API](https://github.com/theia-ide/theia/pull/2086).
  - Note, the format of tasks.json has been changed. For details, see the Task extension's [README.md](https://github.com/theia-ide/theia/blob/master/packages/task/README.md).
- Added an UI when developing plugins
- Migrated widgets to `react`
- Theia alerts you when the opening of a new tab is denied by the browser
- [core] added quick option to toggle the autosave feature
- [filesystem] added `File Download` feature
- [git] `git commit` now alerts the user if no files are staged
- [git] fixed `git` unstaging feature
- [languages] added textmate syntax coloring support (works on `.ts` files for now until more grammars are registered)
- [search-in-workspace] added new command `Search In Folder...`
- [search-in-workspace] added the missing `Search` menu item
- [workspace] fixed issue to prevent workspace root from being be deleted
- `.md` files that are edited in `diff` mode now correctly open with the editor
- `HTML` files now open in the editor by default

## v0.3.11

- Added search and replace widget
- Added the ability to delete files on OSX with cmd+backspace
- Added the ability to set more finely grained logger levels
- Fixed several memory leaks.
- [editor] changed the font in the editor
- [editor] fixed the capital `R` key (<kbd>shift + r</kbd>) not working in the editor
- [file-search] added support for search in hidden files
- [git] added `git sync` and `git publish` actions
- [navigator] added the ability to toggle hidden files in the navigator
- `jdt.ls` download on postinstall

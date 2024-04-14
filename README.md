# VS Code Settings Boilerplate

This project provides a set of common VS Code settings, tasks, and recommended extensions to supercharge your next project. It includes a `.vscode` folder with `settings.json`, `tasks.json`, and `extensions.json` files.

## The .vscode Folder

The `.vscode` folder is a special folder that VS Code recognizes. It contains configuration files that VS Code reads whenever you open your workspace. These files can be used to override user and workspace settings, define tasks, recommend extensions, and more.

### settings.json

The `settings.json` file is used to override VS Code's default and user settings for the workspace. This can include editor settings, formatting settings, linting settings, and more. It's a great way to ensure consistent editor behavior across your team.

### tasks.json

The `tasks.json` file is used to define tasks that can be run in your workspace. These tasks can be used to build, test, or launch your application among other things. Tasks can be run manually from the Command Palette (`Ctrl+Shift+P` -> `Tasks: Run Task`), or they can be associated with specific events in your workspace (like a file save or a build command).

### extensions.json

The `extensions.json` file is used to recommend extensions to the user. When a user opens your workspace, they will be prompted to install any recommended extensions that they don't already have. This is a great way to ensure that everyone on your team has the same set of tools.

## More Details

In the following sections, we'll dive deeper into each of these files and explain the specific settings, tasks, and extensions that we've included in this boilerplate.

### Settings

The `settings.json` file in the `.vscode` directory configures the behavior of Visual Studio Code. Here are the settings defined in this project:

- `"debug.javascript.autoAttachFilter": "smart"`: This setting controls the automatic attachment of the debugger for Node.js scripts. When set to "smart", the debugger will automatically attach when launching scripts via `npm`, `yarn`, `nodemon`, etc.

- `"editor.cursorBlinking": "smooth"`: This setting controls the cursor animation style. When set to "smooth", the cursor will have a smooth blinking animation.

- `"editor.cursorSmoothCaretAnimation": "on"`: This setting enables smooth caret animation, making the cursor move smoothly as you type.

- `"editor.cursorStyle": "line"`: This setting controls the cursor style. When set to "line", the cursor will be a vertical line.

- `"editor.fontFamily": "Fira Code"`: This setting controls the font family of the editor. In this case, it's set to "Fira Code".

- `"editor.fontLigatures": true`: This setting enables font ligatures, which combine multiple characters into a single typographic unit.

- `"editor.rulers": [...]`: This setting renders vertical rulers after a certain number of monospace characters. It's useful for enforcing line length limits.

- `"editor.stickyScroll.enabled": true`: This setting enables sticky scrolling, which keeps the last line of your file in the middle of the screen when scrolling past the end of the file.

- `"editor.tabSize": 2`: This setting controls the number of spaces a tab is equal to. In this case, it's set to 2.

- `"editor.codeActionsOnSave": {...}`: This setting controls the code action kinds to be run on save. In this case, it's set to organize imports and fix all eslint problems.

These settings can be customized to suit your project's needs. For more information on configuring settings in VS Code, see the [official documentation](https://code.visualstudio.com/docs/getstarted/settings).

### Tasks

The `tasks.json` file in the `.vscode` directory defines tasks that can be run in your workspace. These tasks can be used to build, test, or launch your application among other things. Tasks can be run manually from the Command Palette (`Ctrl+Shift+P` -> `Tasks: Run Task`), or they can be associated with specific events in your workspace (like a file save or a build command).

Here are the tasks defined in this project:

- `build`: This task runs the `npm run build` command. It's grouped under the `build` kind and is the default build task.

- `test`: This task runs the `npm run test` command. It's grouped under the `test` kind and is the default test task. The `detail` property provides a description of the task, and the `icon` property specifies an icon to represent the task in the UI.

- `start`: This task runs the `npm run start` command. It's grouped under the `test` kind and is the default task of this kind.

- `lint`: This task runs the `npm run lint` command. It's not associated with a specific group.

- `clean`: This task runs the `rm -rf ./dist ./node_modules ./build ./coverage` command, which removes the `dist`, `node_modules`, `build`, and `coverage` directories. This can be useful for doing a clean build or install.

- `dev`: This task runs the `npm run dev` command. It's not associated with a specific group.

These tasks can be customized to suit your project's needs. For more information on configuring tasks in VS Code, see the [official documentation](https://go.microsoft.com/fwlink/?LinkId=733558).

### Extensions

The `extensions.json` file in the `.vscode` directory recommends extensions to the user. When a user opens your workspace, they will be prompted to install any recommended extensions that they don't already have. This is a great way to ensure that everyone on your team has the same set of tools.

Here are the extensions recommended in this project:

- `ms-vscode.vscode-typescript-tslint-plugin`: Integrates the TypeScript TSLint language service into VS Code.

- `esbenp.prettier-vscode`: Integrates Prettier, a code formatter, into VS Code.

- `msjsdiag.debugger-for-chrome`: Adds support for debugging JavaScript in Google Chrome to VS Code.

- `editorconfig.editorconfig`: Integrates EditorConfig, a tool for maintaining consistent coding styles, into VS Code.

- `ms-azuretools.vscode-docker`: Adds Docker integration to VS Code.

- `ms-vscode.vscode-jest`: Adds Jest support to VS Code.

- `redhat.vscode-yaml`: Provides comprehensive YAML language support to VS Code.

- `ms-vscode-remote.remote-ssh`: Allows you to use any remote machine with a SSH server as your development environment.

- `ms-vscode-remote.remote-containers`: Develop inside a Docker container.

- `ms-vscode-remote.remote-wsl`: Use the Windows Subsystem for Linux as your full-time development environment.

- `ms-vscode.gitlens`: Supercharge the Git capabilities built into Visual Studio Code.

- `eamodio.gitlens`: Supercharge the Git capabilities built into Visual Studio Code.

- `formulahendry.auto-rename-tag`: Automatically rename paired HTML/XML tag.

- `kamikillerto.vscode-colorize`: A vscode extension to colorize css/web colors in your editor.

- `mikestead.dotenv`: Support for dotenv file syntax.

- `dbaeumer.vscode-eslint`: Integrates ESLint JavaScript into VS Code.

- `github.vscode-github-actions`: View and manage GitHub Actions workflows in Visual Studio Code.

- `github.copilot`: GitHub Copilot is your AI pair programmer.

- `github.copilot-chat`: Chat with GitHub Copilot.

- `ecmel.vscode-html-css`: Support for HTML CSS class and id name completion.

- `yzhang.markdown-all-in-one`: All you need to write Markdown (keyboard shortcuts, table of contents, auto preview and more).

- `christian-kohler.npm-intellisense`: Visual Studio Code plugin that autocompletes npm modules in import statements.

- `johnpapa.vscode-peacock`: Subtly change the workspace color of your workspace. Ideal when you have multiple VS Code instances and you want to quickly identify which is which.

- `yoavbls.pretty-ts-errors`: Make TypeScript errors more readable.

- `mechatroner.rainbow-csv`: Highlight CSV and TSV files in different colors, Run SQL-like queries.

- `ms-vscode-remote.remote-ssh-edit`: Edit files on any remote machine over SSH.

- `ms-vscode.remote-server`: Run VS Code on any server over SSH or Docker and connect to it from anywhere.

- `ms-vscode-remote.vscode-remote-extensionpack`: An extension pack that lets you open any folder in a container, on a remote machine, or in WSL and take advantage of VS Code's full feature set.

- `ms-vscode.remote-explorer`: A UI to manage remote connections.

- `simonsiefke.svg-preview`: View SVG files in a webview panel.

- `bradlc.vscode-tailwindcss`: Adds Tailwind CSS support to VS Code.

- `meganrogge.template-string-converter`: Convert JavaScript and TypeScript strings to template strings and back again.

- `wayou.vscode-todo-highlight`: Highlight TODO, FIXME and other annotations within your code.

- `gruntfuggly.todo-tree`: Show TODO, FIXME, etc. comment tags in a tree view.

- `pflannery.vscode-versionlens`: Shows the latest version for each package using code lens.

These extensions can be customized to suit your project's needs. For more information on configuring extensions in VS Code, see the [official documentation](https://code.visualstudio.com/docs/editor/extension-marketplace).

```json
{
	"editor.codeActionsOnSave": {
		"source.fixAll.eslint": true
	},
	"editor.defaultFormatter": "esbenp.prettier-vscode",
	"editor.detectIndentation": false,
	"editor.tabSize": 2,
	"editor.fontFamily": "Jetbrains Mono",
	"editor.fontLigatures": true,
	"editor.fontSize": 16,
	"editor.formatOnType": false,
	"editor.insertSpaces": true,
	"editor.minimap.enabled": false,
	"editor.renderWhitespace": "none",
	"editor.snippetSuggestions": "top",
	"editor.wordWrapColumn": 80,
	"emmet.triggerExpansionOnTab": true,
	"emmet.showSuggestionsAsSnippets": true,
	"emmet.showAbbreviationSuggestions": true,
	"emmet.showExpandedAbbreviation": "never",
	"emmet.syntaxProfiles": {
		"javascript": "jsx",
		"javascriptreact": "jsx",
		"xml": {
			"attr_quotes": "single"
		}
	},
	"emmet.includeLanguages": {
		"javascript": "javascriptreact",
		"vue-html": "html",
		"vue": "html"
	},
	"extensions.autoUpdate": true,
	"files.eol": "\n",
	"files.associations": {
		"*.js": "javascript",
		"*.jsx": "javascriptreact",
		"*.vue": "vue",
		"*.ejs": "html"
	},
	"files.exclude": {
		"**/.DS_Store": true,
		"**/.idea": true,
		"**/.svn": true,
		"**/.vscode": false,
		"**/tmp": true,
		"*/node_modules": false
	},
	"files.watcherExclude": {
		"**/.git/objects/**": true,
		"**/node_modules/**": true,
		"**/tmp": true,
		"**/build": true,
		"**/defaultsettings/**": true
	},
	"search.exclude": {
		"**/node_modules": true,
		"**/bower_components": true,
		"**/.git": true,
		"**/.DS_Store": true,
		"**/tmp": true,
		"**/coverage": true,
		"**/build": true,
		"**/Pods": true,
		"**/*.xcodeproj": true,
		"**/*.xcworkspace": true,
		"**/.meteor": true
	},
	"html.format.indentInnerHtml": true,
	"npm-intellisense.scanDevDependencies": false,
	"javascript.validate.enable": false,
	"javascript.format.insertSpaceAfterFunctionKeywordForAnonymousFunctions": false,
	"code-runner.defaultLanguage": "javascript",
	"code-runner.executorMapByFileExtension": {
		".js": "javascript",
		".jsx": "javascript",
		".ts": "echo .ts & npm run ts-node"
	},
	"code-runner.runInTerminal": true,
	"code-runner.terminalRoot": "/Applications/iTerm.app",
	"code-runner.clearPreviousOutput": true,
	"code-runner.saveAllFilesBeforeRun": true,
	"material-icon-theme.showUpdateMessage": false,
	"terminal.integrated.fontSize": 14,
	"terminal.integrated.lineHeight": 1.4,
	"terminal.integrated.shell.osx": "/bin/zsh",
	"terminal.integrated.shell.linux": "/bin/zsh",
	"terminal.integrated.fontFamily": "Jetbrains Mono",
	"markdown.preview.linkify": false,
	"git.confirmSync": false,
	"git.enableSmartCommit": true,
	"git.autofetch": true,
	"gitlens.showWhatsNewAfterUpgrades": false,
	"gitlens.keymap": "alternate",
	"gitlens.advanced.messages": {
		"suppressFileNotUnderSourceControlWarning": true,
		"suppressLineUncommittedWarning": true,
		"suppressNoRepositoryWarning": true,
		"suppressShowKeyBindingsNotice": true,
		"suppressUpdateNotice": true,
		"suppressWelcomeNotice": true
	},
	"javascript.updateImportsOnFileMove.enabled": "always",
	"terminal.explorerKind": "external",
	"terminal.external.osxExec": "iTerm.app",
	"prettier.arrowParens": "always",
	"prettier.semi": true,
	"prettier.trailingComma": "all",
	"prettier.disableLanguages": ["markdown", "md"],
	"prettier.useTabs": true,
	"window.openFoldersInNewWindow": "on",
	"workbench.iconTheme": "material-icon-theme",
	"workbench.startupEditor": "newUntitledFile",
	"liveServer.settings.donotShowInfoMsg": true,
	"typescript.updateImportsOnFileMove.enabled": "always",
	"npm.packageManager": "yarn",
	"eslint.alwaysShowStatus": true,
	"eslint.format.enable": true,
	"eslint.lintTask.enable": true,
	"eslint.packageManager": "yarn",
	"eslint.workingDirectories": ["./eslintrc.json"],
	"eslint.run": "onSave",
	"cSpell.userWords": ["Vuex"],
	"editor.suggestSelection": "first",
	"vscode-pets.petSize": "large",
	"vscode-pets.petType": "dog",
	"vscodeGitCommit.variables": {
		"prefix": "aliases...keke",
		"aliases": [
			{
				"label": "🔨 refactor",
				"detail": "새로운 기능이나 버그 수정이 없는 코드 변경 (ex: 중복 코드 제거, 코드 단순화, 네이밍 변경)"
			},
			{
				"label": "🐛 fix",
				"detail": "이전 버전과 호환되는 버그 수정 및 기타 오류 그외에 오타 수정 (SEM/Patch)"
			},
			{
				"label": "✨ feat",
				"detail": "새로운 기능 추가 (SEM/Minor)"
			},
			{
				"label": "📦 build",
				"detail": "빌드 혹은 외부 의존성에 영향을 주는 변경 사항"
			},
			{
				"label": "🚧 ci",
				"detail": "CI 및 설정 관련 스크립트 변경 (ex: Github actions, npm scripts)"
			},
			{
				"label": "👷 chore",
				"detail": "코드 수정 없이 설정 변경"
			},
			{
				"label": "🎨 style",
				"detail": "코드에 영향을 미치지 않는 변경 (ex: 공백, 포맷팅, 세미콜론, 쉼표 등)"
			},
			{
				"label": "✅ test",
				"detail": "테스트 추가 및 수정"
			},
			{
				"label": "📝 docs",
				"detail": "오로지 문서 변경건만 발생"
			},
			{
				"label": "⚡️ perf",
				"detail": "이전 버전과 호환되는 성능 향상 개선건 (SEM/Minor)"
			},
			{
				"label": "⏪ revert",
				"detail": "커밋을 되돌릴때하며 본문에 커밋 hash 추가 (ex: revert: a 개발건 추가 <hash>)"
			}
		]
	},
	"vscodeGitCommit.template": ["{prefix}({scope}): {message}"],
	"todo-tree.general.tags": [
		"BUG",
		"HACK",
		"FIXME",
		"TODO",
		"XXX",
		"[ ]",
		"[x]"
	],
	"todo-tree.regex.regex": "(//|#|<!--|;|/\\*|^|^\\s*(-|\\d+.))\\s*($TAGS)",
	"vscode-pets.position": "explorer",
	"workbench.editor.untitled.hint": "hidden",
	"editor.bracketPairColorization.enabled": true,
	"quokka.compactMessageOutput": false,
	"wallaby.compactMessageOutput": true,
	"quokka.suppressExpirationNotifications": true,
	"wallaby.codeLensFeature.runTest": true,
	"prettier.singleQuote": true,
	"quokka.showOutputOnStart": false,
	"editor.formatOnSave": true,
	"terminal.integrated.autoReplies": {
		"[Oh My Zsh] Would you like to check for updates? [Y/n]": "Y\r"
	},
	"javascript.inlayHints.functionLikeReturnTypes.enabled": true,
	"terminal.integrated.defaultProfile.osx": "zsh",
	"terminal.integrated.enableBell": true,
	"workbench.colorTheme": "Default High Contrast",
	"window.zoomLevel": 2,
	"liveServer.settings.donotVerifyTags": true
}
```
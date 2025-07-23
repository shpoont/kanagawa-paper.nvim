# Changelog

## [3.0.0](https://github.com/shpoont/kanagawa-paper.nvim/compare/v2.1.0...v3.0.0) (2025-07-23)


### ⚠ BREAKING CHANGES

* **wezterm_tabline:** use theme instead of overrides ([#55](https://github.com/shpoont/kanagawa-paper.nvim/issues/55))
* **config:** rename config options for consistency
* **pywal:** remove pywal extra
* **fish:** remove fish extra
* add ability to choose plugin themes to apply
* **treesitter/lsp:** update to latest TS capture names
* **config:** remove check_config logic, but keep it for the future
* **overhaul:** new features and improvements
* **theme:** theme -> background; add theme option to be used when bg is not specified
* **config:** remove lesser options. + remove punct2; + special constructor for lua
* **themes:** rename themes, allow default (wave) to be set explicitly via :colo
* **overhaul:** WIP deep refactor of theme colors
* several improvements.

### improvement

* several improvements. ([0206f40](https://github.com/shpoont/kanagawa-paper.nvim/commit/0206f4083a50849b77f59b80948454c8a2410445))


### Features

* add ability to choose plugin themes to apply ([72a85ab](https://github.com/shpoont/kanagawa-paper.nvim/commit/72a85abca725111b33d916abce5400e567493062))
* add barbar styling ([6ac72d3](https://github.com/shpoont/kanagawa-paper.nvim/commit/6ac72d35bfda017ff545f4c9863959618c38917b))
* add colors for popular plugins ([a769176](https://github.com/shpoont/kanagawa-paper.nvim/commit/a7691769a771355937d8c8f49e5f984d3c8dd025))
* add colours for UI and builtin highlight groups ([1e0984b](https://github.com/shpoont/kanagawa-paper.nvim/commit/1e0984b4415b146fe78194b38b6716bbb5675ec2))
* add empty highlight group ([057b732](https://github.com/shpoont/kanagawa-paper.nvim/commit/057b732a62ab200402d90a4355c4b525a86094d3))
* add extras for integration with other applications ([16e6a4b](https://github.com/shpoont/kanagawa-paper.nvim/commit/16e6a4b1e44669876c9e91e543cab93e5d7f37f6))
* add groups for the mini ecosystem ([1b719a1](https://github.com/shpoont/kanagawa-paper.nvim/commit/1b719a1d7a62a4985ac7e32132af665389032b0f))
* add highlights for noice and satellite ([36e5293](https://github.com/shpoont/kanagawa-paper.nvim/commit/36e52937df10eec3c91cec575b8f3cccfb08750c))
* add hl for markdown.nvim headers ([c1fac34](https://github.com/shpoont/kanagawa-paper.nvim/commit/c1fac349097dab206f1bf8481976bdb89bba995c))
* add hl for new which key preset ([367be8f](https://github.com/shpoont/kanagawa-paper.nvim/commit/367be8f2d08ee00c5603cdc3f6e24beb2999bd85))
* add hl for which key default icon ([2457ccf](https://github.com/shpoont/kanagawa-paper.nvim/commit/2457ccfa4671a8a5c9136a62f8ec4206248c05d5))
* add in support for Note ([66f00dd](https://github.com/shpoont/kanagawa-paper.nvim/commit/66f00dd38fd7de738068942295c78acd9ce67ba7))
* add option to remove gutter background ([475d017](https://github.com/shpoont/kanagawa-paper.nvim/commit/475d017380a7d0d9c1ffd809d8470d771d07a45c))
* add syntax colours ([bc165b4](https://github.com/shpoont/kanagawa-paper.nvim/commit/bc165b4bb16a3fd9f7818f1ac2b2397e95b3451d))
* add wezterm extra ([0a0d567](https://github.com/shpoont/kanagawa-paper.nvim/commit/0a0d567a6ae90189e9054d904f6a00b4feb27c1f))
* advertize themes to vim as separate colorschemes ([bca5195](https://github.com/shpoont/kanagawa-paper.nvim/commit/bca5195db85c6f1b0a89eeca575eb61bfa151b41))
* **alacritty:** add template for alacritty extra ([a8d59a1](https://github.com/shpoont/kanagawa-paper.nvim/commit/a8d59a1e8081a064e60bc58d3caa2eb53f713fab))
* Alfred theme ([a4e99f0](https://github.com/shpoont/kanagawa-paper.nvim/commit/a4e99f089110c6d00bc33f5497709200e914e763))
* Alfred theme ([b4df5ad](https://github.com/shpoont/kanagawa-paper.nvim/commit/b4df5ad19388b1709f87986aadae781ae3563f0a))
* **barbar:** fix background when using transparent theme ([e264574](https://github.com/shpoont/kanagawa-paper.nvim/commit/e2645741fd9f6ec7da149135e181a70bc3725ad6))
* **blink:** add additional blink highlights ([a38356b](https://github.com/shpoont/kanagawa-paper.nvim/commit/a38356b6520fadd710116352e9e98406c9e171c1))
* **blink:** add highlights for blink completion ([79bdc98](https://github.com/shpoont/kanagawa-paper.nvim/commit/79bdc98ffdadaf5a9536a6fa108d3fcb235228ed))
* **canvas:** add canvas palette ([524683a](https://github.com/shpoont/kanagawa-paper.nvim/commit/524683ad8d13069a0b484e13dec3cfb9bc12625d))
* **cmdheight:** improve MsgSeparator on cmdheight=0 ([899f2c9](https://github.com/shpoont/kanagawa-paper.nvim/commit/899f2c9311b35d9d05ca856411815a92407618fd))
* **compile:** add compilation support ([4bd81cd](https://github.com/shpoont/kanagawa-paper.nvim/commit/4bd81cd210c7a6cd7b6ccd8f471099d2d3d181f1))
* **compile:** compile all themes at once; refactor: add golbal _CURRENT_THEME ([ffb2feb](https://github.com/shpoont/kanagawa-paper.nvim/commit/ffb2feb4ca5e117a0f0183b595f51d2e88245e36))
* **compile:** make compile opt-in instead of opt-out ([9025e02](https://github.com/shpoont/kanagawa-paper.nvim/commit/9025e022a9491bdf7f2c6485d431b03f9c1d0cc3))
* **compile:** opt-out of compilation; fix [#106](https://github.com/shpoont/kanagawa-paper.nvim/issues/106) ([faeef98](https://github.com/shpoont/kanagawa-paper.nvim/commit/faeef985abd6f32cdc2e3c2cce89469060b9c74a))
* **config:** add brightness offset option ([0429b5f](https://github.com/shpoont/kanagawa-paper.nvim/commit/0429b5fae555bf4bee497193f96657a1cd6982b6))
* **config:** add option to enable/disable background for virtual text ([71206ee](https://github.com/shpoont/kanagawa-paper.nvim/commit/71206ee3f4e9b5ba7913f3574628ce5202821dc7))
* **config:** add saturation offset option ([10075f0](https://github.com/shpoont/kanagawa-paper.nvim/commit/10075f02e2c5315503614aa211a4871325c2594c))
* **config:** add theme caching option ([bd5b271](https://github.com/shpoont/kanagawa-paper.nvim/commit/bd5b2714852c6c6113ba3f63dc8622b9d38eece3))
* **config:** auto plugin loading option for lazy.nvim ([c19ce6f](https://github.com/shpoont/kanagawa-paper.nvim/commit/c19ce6f475252eeb9a87ab84b48208f068941b7d))
* **config:** choose the theme for override colors ([6d611cf](https://github.com/shpoont/kanagawa-paper.nvim/commit/6d611cfe97361843b46382367be0f699985a813e))
* **config:** remove lesser options. + remove punct2; + special constructor for lua ([f785b97](https://github.com/shpoont/kanagawa-paper.nvim/commit/f785b972320eeb14ef249db965a8924e7012a411))
* **editor:** add group for marks ([a038398](https://github.com/shpoont/kanagawa-paper.nvim/commit/a038398036be89002094a40dea656537be64db55))
* **editor:** add highlight for examples in help files ([ff004f1](https://github.com/shpoont/kanagawa-paper.nvim/commit/ff004f192dd15631981b7ab595aa8084fea787e6))
* **editor:** highlight MsgArea depending on value of 'cmdheight' ([7cede0a](https://github.com/shpoont/kanagawa-paper.nvim/commit/7cede0a885616bf5bd609e092f8ae0cc50cc7d25))
* **extras:** add build process for extras ([ed1119a](https://github.com/shpoont/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **extras:** add color overrides for wezterm tabline ([66053e5](https://github.com/shpoont/kanagawa-paper.nvim/commit/66053e59a7e28cb9e8df542c41f588acebec223e))
* **extras:** add extras/nushell ([#51](https://github.com/shpoont/kanagawa-paper.nvim/issues/51)) ([e8ca337](https://github.com/shpoont/kanagawa-paper.nvim/commit/e8ca337d906542cae45cfae14d8103eb70631029))
* **extras:** add ghostty ([0aee289](https://github.com/shpoont/kanagawa-paper.nvim/commit/0aee2893f0178fb7078b4c6e51fd780d64b046d4))
* **extras:** add kanagawa.tmTheme ([b5c6142](https://github.com/shpoont/kanagawa-paper.nvim/commit/b5c614216faccedb51b071bbeeabb34d089add8f))
* **extras:** add kanagawa.tmTheme ([7b411f9](https://github.com/shpoont/kanagawa-paper.nvim/commit/7b411f9e66c6f4f6bd9771f3e5affdc468bcbbd2))
* **extras:** improve tab foreground in kitty theme ([c8af52c](https://github.com/shpoont/kanagawa-paper.nvim/commit/c8af52c95022f80931b8c042538db6c10e0245ec))
* **fish:** remove fish extra ([3e465db](https://github.com/shpoont/kanagawa-paper.nvim/commit/3e465db0f33bee501135e03bdcb745f1b592d0f1))
* **foot:** add extra theme for foot ([be6dcc4](https://github.com/shpoont/kanagawa-paper.nvim/commit/be6dcc4ed8da2e6b0f567f1dc0661ff3daea821e))
* **fzf:** add color scheme for fzf ([c510f4c](https://github.com/shpoont/kanagawa-paper.nvim/commit/c510f4c6461f00753ff0c03e68e368eb6ba217e1)), closes [#17](https://github.com/shpoont/kanagawa-paper.nvim/issues/17)
* **fzf:** add template for fzf extra ([f1a86cf](https://github.com/shpoont/kanagawa-paper.nvim/commit/f1a86cff532e89c3a8c79f37c44828fb39a28b6d))
* **ghostty:** add template for ghostty theme ([8306edb](https://github.com/shpoont/kanagawa-paper.nvim/commit/8306edbee319320de020300eb6f634239c0cb89b))
* **gitgutter:** add hl for gitgutter ([5c8095c](https://github.com/shpoont/kanagawa-paper.nvim/commit/5c8095c1fba5f133810e70926ede58620474c879))
* **grug-far:** add hl for grug-far ([197f0e8](https://github.com/shpoont/kanagawa-paper.nvim/commit/197f0e83876997be12aaedf20d7c608c3a469daa))
* **highlights-plugins:** add Neogit; fix [#139](https://github.com/shpoont/kanagawa-paper.nvim/issues/139) ([89d5ec4](https://github.com/shpoont/kanagawa-paper.nvim/commit/89d5ec496d371bfda5722612d33fd61d6b858279))
* **highlights:** add FloatFooter hl ([0a24e50](https://github.com/shpoont/kanagawa-paper.nvim/commit/0a24e504a3a278849ad0aef31cd6dd24c73ca3db))
* **HSLuvColor:** improvements to color manipulation ([bf13f1b](https://github.com/shpoont/kanagawa-paper.nvim/commit/bf13f1bb92f80dd3774d943ef43fd80520c1098b))
* **indent:** add hl for indent line character ([06bc994](https://github.com/shpoont/kanagawa-paper.nvim/commit/06bc994416ea2a503a3a171f2fff929f9b12c623))
* **ink:** set scrollbar to shade of the bg ([4c34918](https://github.com/shpoont/kanagawa-paper.nvim/commit/4c349188c0876b020c08753ee2d9ab38a83a9327))
* **ink:** use brightened colors for bright ansi colors ([b2a8360](https://github.com/shpoont/kanagawa-paper.nvim/commit/b2a8360b73d913f8a1c008e78b0ce9c6fee55591))
* **kitty:** add template for kitty extra ([191a5dc](https://github.com/shpoont/kanagawa-paper.nvim/commit/191a5dc9f3d3eefc13f315ebdd977d7dde2503b3))
* **lazygit:** add template for lazygit extra ([c8b7cdf](https://github.com/shpoont/kanagawa-paper.nvim/commit/c8b7cdf0b488bed83e24cb664c7d5120e55fd7af))
* **leap:** add groups for jump motion plugins ([4f41353](https://github.com/shpoont/kanagawa-paper.nvim/commit/4f41353f6a2bf9f25b2466a0f1eb6883d8fd09c1))
* **lsp:** add additional lsp types ([ec651cb](https://github.com/shpoont/kanagawa-paper.nvim/commit/ec651cb118a2e5671b1f148a9e432f09e7bda7c3))
* **lsp:** add typemod.function.readonly.javascript; fix [#144](https://github.com/shpoont/kanagawa-paper.nvim/issues/144) ([6e89801](https://github.com/shpoont/kanagawa-paper.nvim/commit/6e898011e90e7c62a78889c0b3dfe6df54cc5c2d))
* **lsp:** using bg highlight for lspreferences ([89f65b7](https://github.com/shpoont/kanagawa-paper.nvim/commit/89f65b7b9c0b8751318d7e98d58a9a7218afe3ce))
* **luap:** regex highlights for lua patterns ([d0613a6](https://github.com/shpoont/kanagawa-paper.nvim/commit/d0613a6e6df5fa379e6e443755e292b6d89465a4))
* **mcphub:** add colors for mcphub ([#57](https://github.com/shpoont/kanagawa-paper.nvim/issues/57)) ([b0df20c](https://github.com/shpoont/kanagawa-paper.nvim/commit/b0df20cca3b7087c06f241983b488190cc8e23af))
* **neotest:** add hl for neotest ([3407e75](https://github.com/shpoont/kanagawa-paper.nvim/commit/3407e75ab67131dcd0045a9a3854e429de9fff19))
* **octo:** add hl for octo ([94954b6](https://github.com/shpoont/kanagawa-paper.nvim/commit/94954b6e6771e381ba85a8f21597eaa8d6403d8e))
* **overhaul:** new features and improvements ([d146b7e](https://github.com/shpoont/kanagawa-paper.nvim/commit/d146b7e32fa6049025cb808ff8f7c4718b0d4fcd))
* **overseer:** add hl for overseer ([8a40bf2](https://github.com/shpoont/kanagawa-paper.nvim/commit/8a40bf2cb9d81af1c036de378beb04417280e3e2))
* **palette:** add all colors ([72775d9](https://github.com/shpoont/kanagawa-paper.nvim/commit/72775d9d1c55f57ae1cd06a397923a5f35041e94))
* **palette:** add darker sumiInk color ([dca5578](https://github.com/shpoont/kanagawa-paper.nvim/commit/dca55783f2e4b847ba064370c61d877fd0a62cde))
* **plugins-Telescope:** better selection and caret highlights ([66aeaf7](https://github.com/shpoont/kanagawa-paper.nvim/commit/66aeaf7573253a847a02d56218b0d7f6cea7609e))
* **plugins:** add Aerial%KIND%Icon colors; consistent LSP kind colors for Cmp, Navic and Aerial ([23ae977](https://github.com/shpoont/kanagawa-paper.nvim/commit/23ae977e5a46dbf976d051ad2b57f5ed789871d8))
* **plugins:** add explicit background for nvim-notify ([545c9a6](https://github.com/shpoont/kanagawa-paper.nvim/commit/545c9a6e8c34680c9d376d025e9c5afeeefa7d20))
* **plugins:** add Indent blankline v3 ([c19b902](https://github.com/shpoont/kanagawa-paper.nvim/commit/c19b9023842697ec92caf72cd3599f7dd7be4456))
* **plugins:** add Indent blankline v3 ([d8552ee](https://github.com/shpoont/kanagawa-paper.nvim/commit/d8552ee27c777055ed38ea49277aa271214d45e9))
* **plugins:** add NeoTreeIndentMarker ([9cc07c5](https://github.com/shpoont/kanagawa-paper.nvim/commit/9cc07c5a98b2f14dc80a9f464334107cc4b6b497))
* **plugins:** add NeoTreeTabSeparator ([6059509](https://github.com/shpoont/kanagawa-paper.nvim/commit/6059509ca8467dd2068a04bb0b286887e236685e))
* **plugins:** add TreesitterContextLineNumber ([129e817](https://github.com/shpoont/kanagawa-paper.nvim/commit/129e817c65a63b6d1f328670355b6780a2d4f36a))
* **plugins:** better dashboard support ([17a084f](https://github.com/shpoont/kanagawa-paper.nvim/commit/17a084fc27d7a908fef779dea6890fe9a8d0510d))
* **plugins:** hl for NvimTree window picker ([00f4307](https://github.com/shpoont/kanagawa-paper.nvim/commit/00f4307d9eda1393cd32fc033fa720b0843eea87))
* **plugins:** improve telescope and lazy ([5ae029a](https://github.com/shpoont/kanagawa-paper.nvim/commit/5ae029a2aa291a757332897b75df27c26aa38241))
* **plugins:** initial support for NeoTree ([423370a](https://github.com/shpoont/kanagawa-paper.nvim/commit/423370ab6f94df48bcfb9090a6733b6e82b9beb0))
* **plugins:** Trouble v3 ([860e4f8](https://github.com/shpoont/kanagawa-paper.nvim/commit/860e4f80df71221d18bf2cd9ef1deb4d364274d2))
* **pywal:** remove pywal extra ([4c98a06](https://github.com/shpoont/kanagawa-paper.nvim/commit/4c98a06c10962ede0f64c483c80c7fcb1702d38a))
* **rainbow:** add hl for rainbow ([8858669](https://github.com/shpoont/kanagawa-paper.nvim/commit/8858669f93a9b66c44d5734e0b7283bfa747cc0a))
* remove vscode extra in favor of separate extension ([61ce2ed](https://github.com/shpoont/kanagawa-paper.nvim/commit/61ce2edc34048cdcbb315850b62dd3ea822efe2b))
* **semantic_highlights:** add "injected" groups ([554a63e](https://github.com/shpoont/kanagawa-paper.nvim/commit/554a63e9649af5d1cbedcf5e81d912d4612e466b))
* **semantic_highlights:** add "injected" highlights ([0133b85](https://github.com/shpoont/kanagawa-paper.nvim/commit/0133b85255d476afda403f3e9cd0310fe5af3f57))
* **semantic_highlights:** add initial support for semantic tokens highlights ([5781565](https://github.com/shpoont/kanagawa-paper.nvim/commit/57815655d7f7bc0b78c8a5b45de38db28aabfd58))
* set default styling ([bf9acc8](https://github.com/shpoont/kanagawa-paper.nvim/commit/bf9acc88ceda3c6ff720c5451ee66193dc627957))
* **sway:** add config for Sway WM colors ([0041c7e](https://github.com/shpoont/kanagawa-paper.nvim/commit/0041c7ea4e6dd0f39562a4902d93c864b44d4120))
* **sway:** tidy up formatting ([c200345](https://github.com/shpoont/kanagawa-paper.nvim/commit/c2003451a72d95f8a0f8a6addbc04d61219f9d44))
* **tabline:** better TabLineSel background ([cff7a76](https://github.com/shpoont/kanagawa-paper.nvim/commit/cff7a762dbaf9bc6aa5f9c1350362fe49f4263c4))
* **terminal:** add kanagawa dragon alacritty theme ([7fecf21](https://github.com/shpoont/kanagawa-paper.nvim/commit/7fecf215ae44d11dae45d9aff61a294762b60347))
* **terminal:** add kanagawa dragon alacritty theme ([0e8ac7e](https://github.com/shpoont/kanagawa-paper.nvim/commit/0e8ac7ea8c4a8a4b1191b629f04c754fb356ff33))
* **terminal:** add template for windows terminal extra ([1524591](https://github.com/shpoont/kanagawa-paper.nvim/commit/15245916aabae33ff060c66275eca1f17979f5d1))
* **terminal:** improve terminal colors, add kanagawa_dragon kitty theme ([181e322](https://github.com/shpoont/kanagawa-paper.nvim/commit/181e3223512799d7248c70fa7249ab58a33d9906))
* **terminator:** add template for terminator extra ([2f191bf](https://github.com/shpoont/kanagawa-paper.nvim/commit/2f191bf69dafbf3f5100ad9ffbea631ca4147218))
* **termux:** add template for termux extra ([e9761e1](https://github.com/shpoont/kanagawa-paper.nvim/commit/e9761e1dd31efca8fd82bb1713f9a9ba1099e1c3))
* **theme:** add default lotus colors ([aa96c99](https://github.com/shpoont/kanagawa-paper.nvim/commit/aa96c99b85201505311d3d56c043c3b8f4b5a597))
* **theme:** add theme switching ([2220c56](https://github.com/shpoont/kanagawa-paper.nvim/commit/2220c56a61093e51fe22be0ccfaeac3e25bf4824))
* **theme:** create new accent color ([651acd8](https://github.com/shpoont/kanagawa-paper.nvim/commit/651acd83e524d9d8bcdddfce77c6c80a18e2e546))
* **themes:** rename themes, allow default (wave) to be set explicitly via :colo ([1928e9c](https://github.com/shpoont/kanagawa-paper.nvim/commit/1928e9cbca28d9d6342c52a24d1242af8dd3cf2d))
* **tilix:** add template for tilix extra ([b246761](https://github.com/shpoont/kanagawa-paper.nvim/commit/b24676178ccbd3470daca2543f5c272c56277e67))
* **todo-comments:** better TS highlights for todo/warning/danger comments ([6668ad6](https://github.com/shpoont/kanagawa-paper.nvim/commit/6668ad6e092e03e8d3f8b3a3184e05413df02247))
* **treesitter/lsp:** update to latest TS capture names ([75be2b9](https://github.com/shpoont/kanagawa-paper.nvim/commit/75be2b90c135a6cdacf05826aeb44dcf0c95df3c))
* **treesitter:** better support for markup (latex) ([497a5ea](https://github.com/shpoont/kanagawa-paper.nvim/commit/497a5eadf76bc57ab0d80d50a87ecc0e7535d72d))
* **treesitter:** enable strikethrough and underline in markup ([bfa818c](https://github.com/shpoont/kanagawa-paper.nvim/commit/bfa818c7bf6259152f1d89cf9fbfba3554c93695))
* **TS:** add [@text](https://github.com/text).diff.{add,delete} groups; fix [#135](https://github.com/shpoont/kanagawa-paper.nvim/issues/135) ([a0c9e7c](https://github.com/shpoont/kanagawa-paper.nvim/commit/a0c9e7c7aab4a139196ec00e77787b0c8c3e2be4))
* update mode colors for lualine ([0d8ec61](https://github.com/shpoont/kanagawa-paper.nvim/commit/0d8ec61c0490ac0fef2cec544dc02606c77314f1))
* upstream updates ([d21f0f9](https://github.com/shpoont/kanagawa-paper.nvim/commit/d21f0f96e3c3a898891e110c9179765c1f9f7fb8))
* **utils:** add utils lib and hot reload for palette ([ed1119a](https://github.com/shpoont/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **vscode_terminal:** add template for vscode terminal extra ([d8942ed](https://github.com/shpoont/kanagawa-paper.nvim/commit/d8942eddd628e3da7c833b78fa79240e73b00bc4))
* **wezterm_tabline:** add template for wezterm tabline plugin ([bdd93df](https://github.com/shpoont/kanagawa-paper.nvim/commit/bdd93df0f430f938cd62f740e283d41e71f25591))
* **wezterm_tabline:** use theme instead of overrides ([#55](https://github.com/shpoont/kanagawa-paper.nvim/issues/55)) ([c44f951](https://github.com/shpoont/kanagawa-paper.nvim/commit/c44f951ec55dbc2451d3ce75f0cef6dfa66ba51a))
* **wezterm:** add wezterm integration to auto switch the theme ([bd51421](https://github.com/shpoont/kanagawa-paper.nvim/commit/bd514210dcfef8af4629fb02561420212e7923db))
* **wezterm:** add wezterm template ([66bae38](https://github.com/shpoont/kanagawa-paper.nvim/commit/66bae38175261db0df9a0e5e6be397346e72f7b8))
* **which-key:** add hl for the title ([05c0e0b](https://github.com/shpoont/kanagawa-paper.nvim/commit/05c0e0b02d75254dc7ccadb06caff48ae6b67177))
* **windowpicker:** add hl for window picker letter ([bbf1a7b](https://github.com/shpoont/kanagawa-paper.nvim/commit/bbf1a7b1d3a0b7eb61d69c371401e59062f31f55))


### Bug Fixes

* add more consistency to member and property colors ([5e28672](https://github.com/shpoont/kanagawa-paper.nvim/commit/5e2867285a6614ada73200d6d5bb594662efc61f))
* add transparency to NC windows ([b300277](https://github.com/shpoont/kanagawa-paper.nvim/commit/b300277a077c7f97b041f82b5ea59f9cc8a95983))
* adjust default theme colors ([f877d58](https://github.com/shpoont/kanagawa-paper.nvim/commit/f877d58ba4f9413953d7ec62929abbbaa4f79acd))
* **annotations:** fix background option annotation ([a7db9f1](https://github.com/shpoont/kanagawa-paper.nvim/commit/a7db9f1794635332f2e74e85f0403953fc567efb))
* **barbar:** fix bolding of a few elements ([07d9685](https://github.com/shpoont/kanagawa-paper.nvim/commit/07d9685e9e1724bb30d543959c8ccf2432e4f2bc))
* better colours for search highlights ([e65f728](https://github.com/shpoont/kanagawa-paper.nvim/commit/e65f728ecacae0a17f1fb55ef7ad2f3240ea3513))
* **blink:** make source text more readable ([502cd71](https://github.com/shpoont/kanagawa-paper.nvim/commit/502cd718eec01bb9fd6cbbd12bc6508f07ce1312))
* **blink:** re-enable icon colors ([04b5985](https://github.com/shpoont/kanagawa-paper.nvim/commit/04b59856dcab6a0569ec88568ae1ccdb46dcbe7b))
* bold buffer numbers ([9720afb](https://github.com/shpoont/kanagawa-paper.nvim/commit/9720afbf6ca60c65051d0fc81ee974b86096c1be))
* bufferline buffer separators ([48b1ec2](https://github.com/shpoont/kanagawa-paper.nvim/commit/48b1ec21c5edfb99322f7dde18825f718eec219c))
* **cache:** correct scope for encapsulation pattern ([#29](https://github.com/shpoont/kanagawa-paper.nvim/issues/29)) ([76633c3](https://github.com/shpoont/kanagawa-paper.nvim/commit/76633c3035aa4c626b00b4487048077786c271d8))
* **canvas:** bolder colors ([e7c9255](https://github.com/shpoont/kanagawa-paper.nvim/commit/e7c92555efe43521add43da0975784e14e0707ca))
* **canvas:** improve indent colors ([e7c9255](https://github.com/shpoont/kanagawa-paper.nvim/commit/e7c92555efe43521add43da0975784e14e0707ca))
* **canvas:** make fzf highlights more readable ([1947ab5](https://github.com/shpoont/kanagawa-paper.nvim/commit/1947ab58e37f412119248e87a30450ea9f3ab567))
* **canvas:** reduce saturation of canvas colors ([0449f68](https://github.com/shpoont/kanagawa-paper.nvim/commit/0449f68a7963cb82571bb042a3f6e4d9fba2632c))
* **command:** call load directly ([246ac28](https://github.com/shpoont/kanagawa-paper.nvim/commit/246ac283e9cc90fa49bd4736144c1977ac0a9ee6))
* **compile-command:** trigger ColorScheme autocmd on compilation ([ef1882b](https://github.com/shpoont/kanagawa-paper.nvim/commit/ef1882b21c84b4ccb1bd55cad7a38b7362ef2d18))
* **compile:** also compile terminal colors ([10527da](https://github.com/shpoont/kanagawa-paper.nvim/commit/10527dafc57c412a75a13d45325bc1ec6d5d0970))
* **compile:** compile to own directory ([bd157a1](https://github.com/shpoont/kanagawa-paper.nvim/commit/bd157a17172b21f4292405e33583b32569962584))
* **config:** fix theme overrides for multiple themes ([ad35e0e](https://github.com/shpoont/kanagawa-paper.nvim/commit/ad35e0ec1a8a85eacb4f48384011fee4fc8113e2))
* **config:** fix wrong error thrown if `theme` is set ([d12d8fd](https://github.com/shpoont/kanagawa-paper.nvim/commit/d12d8fd5202ea69ec4e80b387439a59ae042e921))
* **config:** remove unused option ([3b40289](https://github.com/shpoont/kanagawa-paper.nvim/commit/3b4028972651a156fa5b1c5daf608ba25c7e8aad))
* **config:** rename config options for consistency ([908f6a9](https://github.com/shpoont/kanagawa-paper.nvim/commit/908f6a905cd103cb77f76f5c2e2e4b733b03e81a))
* **dap:** make breakpoints and UI buttons more readable ([bf4a8a9](https://github.com/shpoont/kanagawa-paper.nvim/commit/bf4a8a986cbc8f5c193adb2ed0cd2970f672040f))
* **dev:** fix colour indicators during dev mode ([ed1119a](https://github.com/shpoont/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **diff:** make changed diff text more readable ([a3a6320](https://github.com/shpoont/kanagawa-paper.nvim/commit/a3a6320997a022b3546f62335b6442853fc76191))
* **editor:** add fg color to visual selections so they're easier to read ([03969da](https://github.com/shpoont/kanagawa-paper.nvim/commit/03969da8b17a1d47b1c630a96c0654c54e033322))
* **editor:** differentiate cursorline and visual selection colors ([1a4909c](https://github.com/shpoont/kanagawa-paper.nvim/commit/1a4909caf86013280226a8391391e44ff3fe35e4)), closes [#14](https://github.com/shpoont/kanagawa-paper.nvim/issues/14)
* **editor:** keep syntax colors on visual selections ([1afb15d](https://github.com/shpoont/kanagawa-paper.nvim/commit/1afb15de43b6c25930f56eda948c7b4d15906037))
* **editor:** winbar typo ([5067fa5](https://github.com/shpoont/kanagawa-paper.nvim/commit/5067fa5a27c57bfee29cb2c4099933da3bb12707))
* **extras:** building with the wrong theme field ([52e7781](https://github.com/shpoont/kanagawa-paper.nvim/commit/52e7781985f1c3ca82a6a69336e7b16bddd670e6))
* **extras:** fix bg of dragon kitty theme ([bd27c98](https://github.com/shpoont/kanagawa-paper.nvim/commit/bd27c9835dad727f77c80f5c035f3b297b4f1e6a))
* **extras:** make wezterm highlights more readable ([ca32d10](https://github.com/shpoont/kanagawa-paper.nvim/commit/ca32d10d59d73f5fee728b9e03bb88e966e5ca18))
* **extras:** revert broken suckless extension ([002b624](https://github.com/shpoont/kanagawa-paper.nvim/commit/002b624d77b0a2f82005a82976a50cde637f8ad1))
* **extras:** set execute permissions ([c8ab889](https://github.com/shpoont/kanagawa-paper.nvim/commit/c8ab889933cdc96e9b2e0c613c71187f0ce1c0dd))
* fix border colours ([8ee750a](https://github.com/shpoont/kanagawa-paper.nvim/commit/8ee750a5201e1ca5db288ad12ace299dfb7f0535))
* fix bufferline close button transparency ([3848c69](https://github.com/shpoont/kanagawa-paper.nvim/commit/3848c69016af4cdb9b48b4444b67ae1c43bd14d0))
* fix bufferline tab background ([443d312](https://github.com/shpoont/kanagawa-paper.nvim/commit/443d31250e7541b40c3f1f1cbef621715d835ab9))
* fix msgarea background ([b502c37](https://github.com/shpoont/kanagawa-paper.nvim/commit/b502c3795322d5b550046ec3cdb51059d4f482f1))
* fix neotree transparency ([9218970](https://github.com/shpoont/kanagawa-paper.nvim/commit/921897017525b77e7d89a30f930860ff173ce7ab))
* fix pmenu bg color ([4dad8ed](https://github.com/shpoont/kanagawa-paper.nvim/commit/4dad8ed80d784c73ecf5b81073b196ee504d14ab))
* fix zsh ft groups ([77ec54a](https://github.com/shpoont/kanagawa-paper.nvim/commit/77ec54a2c6039a140b413a429c9b72bb1171b65b))
* flip colours ([e5f1946](https://github.com/shpoont/kanagawa-paper.nvim/commit/e5f1946dd3e07ea53e9a1951b96902c8b283bf5d))
* **float:** make float and pemu colors more consistent across themes ([d7be442](https://github.com/shpoont/kanagawa-paper.nvim/commit/d7be44294f58c96759e68377d395e52248103918))
* **fzf:** change fzf extension to rc ([9be1baa](https://github.com/shpoont/kanagawa-paper.nvim/commit/9be1baa6bfbc543c698d351e60fb63c6bb837804))
* get bufferline transparency working properly ([43e3cf3](https://github.com/shpoont/kanagawa-paper.nvim/commit/43e3cf3d4dd0dd2d4dd639fb3fced4b54c2328e4))
* **headlines:** reduce brightness of markdown header bg ([341adbe](https://github.com/shpoont/kanagawa-paper.nvim/commit/341adbef7b9ca09a3290fa855932ef8594c931bb))
* **highlights-plugins:** fix some CmpItemKind* referencing old TS highlights ([48c5517](https://github.com/shpoont/kanagawa-paper.nvim/commit/48c5517c6e5854e9fad1b9359512996cabbfe481))
* **highlights:** fix  nvimtree bg ([4357138](https://github.com/shpoont/kanagawa-paper.nvim/commit/43571385fbe0b2006c1a2d7b5172154a822fa6b3))
* **hlgroups:** symbol ([3784381](https://github.com/shpoont/kanagawa-paper.nvim/commit/378438188572afd5a7983c51137f1bcca57cd156))
* **hlgroups:** symbol ([01e88f9](https://github.com/shpoont/kanagawa-paper.nvim/commit/01e88f9e8af12c9bca069b12b66f17435b7fd099))
* **hlgroups:** tag attribute color ([476eb22](https://github.com/shpoont/kanagawa-paper.nvim/commit/476eb2289d47d132ebacc1a4d459e3204866599b))
* **hsluvcolor:** guard against 'NONE' colors ([8e9ef29](https://github.com/shpoont/kanagawa-paper.nvim/commit/8e9ef295bf4116573887e9681ec06baa1550d1bc))
* improve bufferline clarity ([3f9d612](https://github.com/shpoont/kanagawa-paper.nvim/commit/3f9d612b6c9724f76059f94668d50a7c35506c93))
* improve text readability of selected regions ([5547588](https://github.com/shpoont/kanagawa-paper.nvim/commit/5547588b6482095d095b965cbca512cb7dfc9420))
* increase contrast of inactive lualine components ([416a7f8](https://github.com/shpoont/kanagawa-paper.nvim/commit/416a7f8e3790193c76be0aee67133986c5703ecc))
* **indent:** make indent lines brighter ([71b3360](https://github.com/shpoont/kanagawa-paper.nvim/commit/71b33609ec2b782921c763054a37472b507c1e43))
* **ink:** create better distinction between visual and cursorline ([027aa65](https://github.com/shpoont/kanagawa-paper.nvim/commit/027aa6587b08d9af31cdd38f99a39ccc0ebc1669))
* **ink:** make diag backgrounds brighter ([3c386ad](https://github.com/shpoont/kanagawa-paper.nvim/commit/3c386ad2993fb0b9f9acf4e9a0263da53965f6f2))
* **ink:** make gray more readable ([660e70d](https://github.com/shpoont/kanagawa-paper.nvim/commit/660e70d33355a34c98c2344a53a2d5700d872258))
* **lazy:** fix consistency of lazy buttons ([5983df2](https://github.com/shpoont/kanagawa-paper.nvim/commit/5983df26b5afb7abcf131c29e5f110a67f28ab60))
* **lsp:** extend typemod.function.readonly to all languages; fix [#144](https://github.com/shpoont/kanagawa-paper.nvim/issues/144) ([963824e](https://github.com/shpoont/kanagawa-paper.nvim/commit/963824e979f33bf2b39838d9ea7a59467d34ec9b))
* **lsp:** make inlays and refs more subtle ([57363b5](https://github.com/shpoont/kanagawa-paper.nvim/commit/57363b53976eec468f925cef803d5419e5b17977))
* **lsp:** remove inlay and codelens bg for transparent themes ([e7eb180](https://github.com/shpoont/kanagawa-paper.nvim/commit/e7eb180bfd776fe41dba613fe19fbc6ff7229484))
* **lsp:** remove lsp.type.comment hl ([09a050b](https://github.com/shpoont/kanagawa-paper.nvim/commit/09a050be9b2eaec71bd1abf593343d2f8895b27f))
* **lsp:** tweak some LSP colors (inlayhints, modules) ([5969bfa](https://github.com/shpoont/kanagawa-paper.nvim/commit/5969bfa1b0e464ddc87f4f1b788b89103245a7cb))
* **lsp:** unset lsp comment fg to allow TODO notes to show up correctly ([dd3a8d8](https://github.com/shpoont/kanagawa-paper.nvim/commit/dd3a8d88df800277e1828dc70b90ca993ccc4a7f))
* **lualine:** add default theme for backward compat ([5ab4d0d](https://github.com/shpoont/kanagawa-paper.nvim/commit/5ab4d0d6d0db19e15071c4d63a69489d14307ffd))
* **lualine:** fix lualine integration ([1789033](https://github.com/shpoont/kanagawa-paper.nvim/commit/1789033803c32464c3eaf8c062f2d65ea236aa1d))
* **lualine:** fix lualine integration ([5173878](https://github.com/shpoont/kanagawa-paper.nvim/commit/5173878eb6bea1bc50f01e143fc08db3c022cf6a))
* **lualine:** set the correct statusline color ([8da902e](https://github.com/shpoont/kanagawa-paper.nvim/commit/8da902efd40818ec96d6881597efb60222a1c469))
* **lualine:** Shall it be boatYellow2; fix [#125](https://github.com/shpoont/kanagawa-paper.nvim/issues/125) ([d8800c3](https://github.com/shpoont/kanagawa-paper.nvim/commit/d8800c36a7f3bcec953288926b00381c028ed97f))
* **lualine:** use darker color for inactive statusline ([108f0f5](https://github.com/shpoont/kanagawa-paper.nvim/commit/108f0f52539a8c068796f277d1219f3d89a80960))
* **lualine:** visual used to be violet; fix [#105](https://github.com/shpoont/kanagawa-paper.nvim/issues/105) ([ebc6013](https://github.com/shpoont/kanagawa-paper.nvim/commit/ebc6013af68f70b5999727d1a2e4395b29ea4735))
* make float borders transparent ([761e718](https://github.com/shpoont/kanagawa-paper.nvim/commit/761e71859f6ddc6dc061ff1d56c8faf1f4f2a81c))
* make line numbers brighter ([b15467f](https://github.com/shpoont/kanagawa-paper.nvim/commit/b15467f8f0643bbd74ba0defbccac7d85fa6386a))
* make selection colors fit the theme a bit better ([a3a3021](https://github.com/shpoont/kanagawa-paper.nvim/commit/a3a3021c144108d61f773f835c23f51a2d010c21))
* make separator bg transparent ([ee98ba2](https://github.com/shpoont/kanagawa-paper.nvim/commit/ee98ba2682dae563d8b4d818499f67ea33c815b0))
* make tabs and buffers easier to identify ([832c50f](https://github.com/shpoont/kanagawa-paper.nvim/commit/832c50f61bef540f71cb76dff88127ed6fabc0ab))
* make variable types in completion popup more readable ([15cb02f](https://github.com/shpoont/kanagawa-paper.nvim/commit/15cb02f3d889b0296efc294ef2be6b2f6753bd7f))
* **markdown:** fix header colors ([cb5b597](https://github.com/shpoont/kanagawa-paper.nvim/commit/cb5b5978654651d37d22066c9b59d2a38489bc36))
* **markdown:** remove underline from markdown links ([4376cd2](https://github.com/shpoont/kanagawa-paper.nvim/commit/4376cd26f43b5b8ddf58f25b3908347b34754e09))
* **methods:** remove specialized method theme color ([207ebd2](https://github.com/shpoont/kanagawa-paper.nvim/commit/207ebd2c0ef953b559b5084e08b1d67bfec0da4e))
* **mini:** match statusline colors to lualine ([9e4c9aa](https://github.com/shpoont/kanagawa-paper.nvim/commit/9e4c9aa8ef849e01c74a20c22b23e5356ed19ab2))
* more readable lsp mini title color ([2f8f91b](https://github.com/shpoont/kanagawa-paper.nvim/commit/2f8f91b53a69138e619cde4ecefc176cfbe44d89))
* **neo-tree:** add missing group for hidden and dotfiles ([#54](https://github.com/shpoont/kanagawa-paper.nvim/issues/54)) ([f7b1ef3](https://github.com/shpoont/kanagawa-paper.nvim/commit/f7b1ef3766081cf6f3d989f8fd67ae861d8e89fa))
* **neogit:** use default neogit colors for diffs ([2856b25](https://github.com/shpoont/kanagawa-paper.nvim/commit/2856b250977c3c7a30f10019a82328f660a7f730)), closes [#18](https://github.com/shpoont/kanagawa-paper.nvim/issues/18)
* **neotree:** make colors more distinctive ([fe859eb](https://github.com/shpoont/kanagawa-paper.nvim/commit/fe859eb835d4cf2db7d2ac23ef23be10ab7cedf2))
* **noice:** fix command line search text readability ([b66f6fc](https://github.com/shpoont/kanagawa-paper.nvim/commit/b66f6fc5fd331186483402432eb73ae7c91ceb53))
* **noice:** match cmdline search text to match color ([4abc704](https://github.com/shpoont/kanagawa-paper.nvim/commit/4abc704f0f1ab68c8e10e5169ea7c4676b3adadf))
* **nvimtree:** link NvimTreeNormal to Normal; fix [#103](https://github.com/shpoont/kanagawa-paper.nvim/issues/103) ([6b5df41](https://github.com/shpoont/kanagawa-paper.nvim/commit/6b5df4199b50e8324fe3141e98212bcfd99d09c6))
* **plugins:** add missing neogit highlights; fix [#139](https://github.com/shpoont/kanagawa-paper.nvim/issues/139) ([172d858](https://github.com/shpoont/kanagawa-paper.nvim/commit/172d858162c4fdeca9cb2cab56eb4b8237af5df1))
* **plugins:** NeoTreeRootName remove italic ([9d9733c](https://github.com/shpoont/kanagawa-paper.nvim/commit/9d9733ca8ec0c7f413df80fd7f55e802a9c2f8d7))
* **presets:** fix telescope preset ([fde88c7](https://github.com/shpoont/kanagawa-paper.nvim/commit/fde88c7a86d2724276be35c4366722c773e9ba08))
* **readme:** add FloatTitle to transparent floats example ([3c87bfa](https://github.com/shpoont/kanagawa-paper.nvim/commit/3c87bfacd5f51033bbeeb04f837c88f94861f6af))
* **readme:** add missing comma ([eb5f0fa](https://github.com/shpoont/kanagawa-paper.nvim/commit/eb5f0fa724030ce6eec9bd20a0fd6f9ced39065c))
* remove lsp highlight color ([361f75f](https://github.com/shpoont/kanagawa-paper.nvim/commit/361f75f674348b04fbb976e6ce5da38ea6b33599))
* revert color for satellite bar bg ([68f8194](https://github.com/shpoont/kanagawa-paper.nvim/commit/68f81940300f2350fca19a968270af68e2e5cb91))
* **snacks:** more consistent cursorline colors for pickers and input ([4f0dbbf](https://github.com/shpoont/kanagawa-paper.nvim/commit/4f0dbbfd9494408c3518f52da61fe8284a6eb90d))
* **snacks:** set color for indents ([74f9110](https://github.com/shpoont/kanagawa-paper.nvim/commit/74f911042c9901d8556fa7a5093912126cb3db2a))
* **syntax:** better distinction between member and variable colors ([d1b21ab](https://github.com/shpoont/kanagawa-paper.nvim/commit/d1b21ab79dc31c592f3fde20e9f81512c836d19d)), closes [#38](https://github.com/shpoont/kanagawa-paper.nvim/issues/38)
* **syntax:** make strings feel less christmasy ([1d670eb](https://github.com/shpoont/kanagawa-paper.nvim/commit/1d670eb3c87c45d0ea0b00c84887583397952920))
* **tabline:** make tabline colors easier to read ([9e93947](https://github.com/shpoont/kanagawa-paper.nvim/commit/9e93947b4fc7bec733e8beaa6f2f18b55050aaac))
* **telescope:** add missing hlgroups ([917dcb8](https://github.com/shpoont/kanagawa-paper.nvim/commit/917dcb84f9d72cfb59ad2c92d1d96af19e4fc292))
* terraform quotes ([9de2520](https://github.com/shpoont/kanagawa-paper.nvim/commit/9de252075f26797ef859ef02697bb723ba5d4713))
* **theme:** add additional cursorline group ([9061ac5](https://github.com/shpoont/kanagawa-paper.nvim/commit/9061ac50a57a6c5c72b5b26ad3597fc12d80a285))
* **theme:** fix background changing behavior of static themes ([846941f](https://github.com/shpoont/kanagawa-paper.nvim/commit/846941f54597f1864e932d5d48be16fbd70f1c9d))
* **theme:** fix dynamic theme loading ([67101b9](https://github.com/shpoont/kanagawa-paper.nvim/commit/67101b9fbccd2f5d91c6d584925c7cdd13c3ef0f))
* **theme:** set relative light and dark colors for diag ([1c7c7e5](https://github.com/shpoont/kanagawa-paper.nvim/commit/1c7c7e552711014294a01ccfb6e6abbe3888528b))
* **themes:** fix theme names in colors.vim ([4834f7c](https://github.com/shpoont/kanagawa-paper.nvim/commit/4834f7cf1063ce894c92c3c5db3d82f01f0d2db4))
* **theme:** use blend for diag backgrounds ([d3dad2b](https://github.com/shpoont/kanagawa-paper.nvim/commit/d3dad2b25b64450bef23e857c145d13e4110a96f))
* this tab separator is really annoying ([782c442](https://github.com/shpoont/kanagawa-paper.nvim/commit/782c44224accefd62a36ce0dfbfb3fd36aaaad9b))
* **tree-sitter:** update descriptions, add markup.link (fix [#225](https://github.com/shpoont/kanagawa-paper.nvim/issues/225)) ([8ed74ad](https://github.com/shpoont/kanagawa-paper.nvim/commit/8ed74ada47d3138385c1a3df2b257c9a1f6182d0))
* **treesitter_context:** fix line number coloring ([45ba977](https://github.com/shpoont/kanagawa-paper.nvim/commit/45ba977cb9ff0fcd50e6c62b7959315c2f631de6))
* **treesitter:** set underline color ([63e61fd](https://github.com/shpoont/kanagawa-paper.nvim/commit/63e61fdc784dc5a13e2301a60d354a0ce58a0096))
* **treesitter:** standardize markdown headers on rainbow ([84511f2](https://github.com/shpoont/kanagawa-paper.nvim/commit/84511f202e5427528f53ac26cf06d1b14302befa))
* **treesitter:** use underline for urls ([728081f](https://github.com/shpoont/kanagawa-paper.nvim/commit/728081fe096c645a937a7784e6cbf73ec1b97d83))
* **trouble:** make trouble counts more readable ([21c86a4](https://github.com/shpoont/kanagawa-paper.nvim/commit/21c86a44e7294526d4f65394c997b5c60280ea73))
* **ts-context:** improve style of context window ([793dbbd](https://github.com/shpoont/kanagawa-paper.nvim/commit/793dbbd14c48642a4ae2a8a7b56961f0b0091f15))
* **TS:** text.diff.{add,delete} use vcs added/removed instead of diff hl ([52ec9e6](https://github.com/shpoont/kanagawa-paper.nvim/commit/52ec9e690735f541b7b4d635605e0c0b1e045750))
* Unclosed quote in `Customizing colors` section of README. ([2aa3d10](https://github.com/shpoont/kanagawa-paper.nvim/commit/2aa3d10ccca8bc4284d8415a222c6e3a6d53b431))
* use regular fg text color for dimmed windows ([567f282](https://github.com/shpoont/kanagawa-paper.nvim/commit/567f282e70ca3e225f0bff82372f58d5818f94ce))
* use theme mode colors for mini statusline ([5c2e091](https://github.com/shpoont/kanagawa-paper.nvim/commit/5c2e091e2d783e077f042d1dff9d2b1a0fab4c9c))
* **vcs:** add darker diff colors ([928f0f4](https://github.com/shpoont/kanagawa-paper.nvim/commit/928f0f4f28475111d0b507c27b243744648bac1f))
* **vcs:** use new vcs colors instead of base groups ([f5ab058](https://github.com/shpoont/kanagawa-paper.nvim/commit/f5ab058de5b9b7020a10cf4646c48f29131ae4e4)), closes [#25](https://github.com/shpoont/kanagawa-paper.nvim/issues/25)
* **wezterm_tabline:** add tab colors ([fed9212](https://github.com/shpoont/kanagawa-paper.nvim/commit/fed9212989af02884cb5815c11c672ecc51aa195))
* **wezterm_tabline:** fix section A fg color ([bdd93df](https://github.com/shpoont/kanagawa-paper.nvim/commit/bdd93df0f430f938cd62f740e283d41e71f25591))
* **yanky:** dont alter the fg color on yank and put ([04af607](https://github.com/shpoont/kanagawa-paper.nvim/commit/04af607d7d7b5b184262102678e7ecea340d5ce3))
* **yanky:** link highlights to visual and insert mode colors ([66596b9](https://github.com/shpoont/kanagawa-paper.nvim/commit/66596b9260b17542e5f7eb6faf7b27f044970b77))
* **yanky:** match yank highlight to visual selection color for consistency ([5b3327b](https://github.com/shpoont/kanagawa-paper.nvim/commit/5b3327b91cc11fa94a949300fc4a1391eaf956d6))


### Performance Improvements

* don't require color module where it is not needed ([aa66e79](https://github.com/shpoont/kanagawa-paper.nvim/commit/aa66e795bf01afd13d23d3a8ec746631951bfc85))
* **groups:** use simpler api for listing directory files ([49b7a23](https://github.com/shpoont/kanagawa-paper.nvim/commit/49b7a23197157c2122030acfa711187d886f36c1))
* **integrations:** use new theme override api for tabline theme switcher ([c7c5f33](https://github.com/shpoont/kanagawa-paper.nvim/commit/c7c5f3306ebc420d46ba5812e578bcf24def7fe0))
* **lib:** cache common function calls ([c63eeb5](https://github.com/shpoont/kanagawa-paper.nvim/commit/c63eeb54c127e2cc08c9b0801a23361442a12fd1))
* **plugins:** add cache for plugin lookup ([0095456](https://github.com/shpoont/kanagawa-paper.nvim/commit/0095456027c0474f0659b8c669ba4c7e6ce7b971))
* **treesitter:** better hl color for [@string](https://github.com/string).special.url ([8c60549](https://github.com/shpoont/kanagawa-paper.nvim/commit/8c60549b8588e7dc7e9084f836b0471735d10bf6))


### Reverts

* **config:** dim active should be opt-in ([f283017](https://github.com/shpoont/kanagawa-paper.nvim/commit/f283017eca5e715f7ea2b17a0c68354fb1ac0e1e))
* remove presets ([d3de16c](https://github.com/shpoont/kanagawa-paper.nvim/commit/d3de16cba3be97ac4598f5030220adfa6120bf6f))


### Miscellaneous Chores

* **config:** remove check_config logic, but keep it for the future ([5ff1359](https://github.com/shpoont/kanagawa-paper.nvim/commit/5ff1359ea1fa6aa30eedb2db75900b30378a3c17))


### Code Refactoring

* **overhaul:** WIP deep refactor of theme colors ([ff3ce26](https://github.com/shpoont/kanagawa-paper.nvim/commit/ff3ce261c0ca4bd478f6a22d7589de52651f78cc))
* **theme:** theme -&gt; background; add theme option to be used when bg is not specified ([a2be0b1](https://github.com/shpoont/kanagawa-paper.nvim/commit/a2be0b1caa87250d317652fb16614dafa64e870c))

## [2.1.0](https://github.com/thesimonho/kanagawa-paper.nvim/compare/v2.0.2...v2.1.0) (2025-05-18)


### Features

* **editor:** add group for marks ([a038398](https://github.com/thesimonho/kanagawa-paper.nvim/commit/a038398036be89002094a40dea656537be64db55))
* **leap:** add groups for jump motion plugins ([4f41353](https://github.com/thesimonho/kanagawa-paper.nvim/commit/4f41353f6a2bf9f25b2466a0f1eb6883d8fd09c1))


### Bug Fixes

* **syntax:** better distinction between member and variable colors ([d1b21ab](https://github.com/thesimonho/kanagawa-paper.nvim/commit/d1b21ab79dc31c592f3fde20e9f81512c836d19d)), closes [#38](https://github.com/thesimonho/kanagawa-paper.nvim/issues/38)

## [2.0.2](https://github.com/thesimonho/kanagawa-paper.nvim/compare/v2.0.1...v2.0.2) (2025-04-21)


### Bug Fixes

* **blink:** re-enable icon colors ([04b5985](https://github.com/thesimonho/kanagawa-paper.nvim/commit/04b59856dcab6a0569ec88568ae1ccdb46dcbe7b))
* **mini:** match statusline colors to lualine ([9e4c9aa](https://github.com/thesimonho/kanagawa-paper.nvim/commit/9e4c9aa8ef849e01c74a20c22b23e5356ed19ab2))
* **snacks:** more consistent cursorline colors for pickers and input ([4f0dbbf](https://github.com/thesimonho/kanagawa-paper.nvim/commit/4f0dbbfd9494408c3518f52da61fe8284a6eb90d))
* **syntax:** make strings feel less christmasy ([1d670eb](https://github.com/thesimonho/kanagawa-paper.nvim/commit/1d670eb3c87c45d0ea0b00c84887583397952920))
* Unclosed quote in `Customizing colors` section of README. ([2aa3d10](https://github.com/thesimonho/kanagawa-paper.nvim/commit/2aa3d10ccca8bc4284d8415a222c6e3a6d53b431))
* **yanky:** dont alter the fg color on yank and put ([04af607](https://github.com/thesimonho/kanagawa-paper.nvim/commit/04af607d7d7b5b184262102678e7ecea340d5ce3))


### Performance Improvements

* **integrations:** use new theme override api for tabline theme switcher ([c7c5f33](https://github.com/thesimonho/kanagawa-paper.nvim/commit/c7c5f3306ebc420d46ba5812e578bcf24def7fe0))


### Reverts

* **config:** dim active should be opt-in ([f283017](https://github.com/thesimonho/kanagawa-paper.nvim/commit/f283017eca5e715f7ea2b17a0c68354fb1ac0e1e))

## [2.0.1](https://github.com/thesimonho/kanagawa-paper.nvim/compare/v2.0.0...v2.0.1) (2025-03-11)


### Bug Fixes

* **cache:** correct scope for encapsulation pattern ([#29](https://github.com/thesimonho/kanagawa-paper.nvim/issues/29)) ([76633c3](https://github.com/thesimonho/kanagawa-paper.nvim/commit/76633c3035aa4c626b00b4487048077786c271d8))
* **editor:** keep syntax colors on visual selections ([1afb15d](https://github.com/thesimonho/kanagawa-paper.nvim/commit/1afb15de43b6c25930f56eda948c7b4d15906037))
* **ink:** create better distinction between visual and cursorline ([027aa65](https://github.com/thesimonho/kanagawa-paper.nvim/commit/027aa6587b08d9af31cdd38f99a39ccc0ebc1669))
* **theme:** add additional cursorline group ([9061ac5](https://github.com/thesimonho/kanagawa-paper.nvim/commit/9061ac50a57a6c5c72b5b26ad3597fc12d80a285))

## [2.0.0](https://github.com/thesimonho/kanagawa-paper.nvim/compare/v1.8.0...v2.0.0) (2025-03-08)


### ⚠ BREAKING CHANGES

* **config:** rename config options for consistency
* **pywal:** remove pywal extra
* **fish:** remove fish extra
* add ability to choose plugin themes to apply

### Features

* add ability to choose plugin themes to apply ([72a85ab](https://github.com/thesimonho/kanagawa-paper.nvim/commit/72a85abca725111b33d916abce5400e567493062))
* **alacritty:** add template for alacritty extra ([a8d59a1](https://github.com/thesimonho/kanagawa-paper.nvim/commit/a8d59a1e8081a064e60bc58d3caa2eb53f713fab))
* **canvas:** add canvas palette ([524683a](https://github.com/thesimonho/kanagawa-paper.nvim/commit/524683ad8d13069a0b484e13dec3cfb9bc12625d))
* **config:** add brightness offset option ([0429b5f](https://github.com/thesimonho/kanagawa-paper.nvim/commit/0429b5fae555bf4bee497193f96657a1cd6982b6))
* **config:** add option to enable/disable background for virtual text ([71206ee](https://github.com/thesimonho/kanagawa-paper.nvim/commit/71206ee3f4e9b5ba7913f3574628ce5202821dc7))
* **config:** add saturation offset option ([10075f0](https://github.com/thesimonho/kanagawa-paper.nvim/commit/10075f02e2c5315503614aa211a4871325c2594c))
* **config:** add theme caching option ([bd5b271](https://github.com/thesimonho/kanagawa-paper.nvim/commit/bd5b2714852c6c6113ba3f63dc8622b9d38eece3))
* **config:** auto plugin loading option for lazy.nvim ([c19ce6f](https://github.com/thesimonho/kanagawa-paper.nvim/commit/c19ce6f475252eeb9a87ab84b48208f068941b7d))
* **editor:** add highlight for examples in help files ([ff004f1](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ff004f192dd15631981b7ab595aa8084fea787e6))
* **extras:** add build process for extras ([ed1119a](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **fish:** remove fish extra ([3e465db](https://github.com/thesimonho/kanagawa-paper.nvim/commit/3e465db0f33bee501135e03bdcb745f1b592d0f1))
* **fzf:** add template for fzf extra ([f1a86cf](https://github.com/thesimonho/kanagawa-paper.nvim/commit/f1a86cff532e89c3a8c79f37c44828fb39a28b6d))
* **ghostty:** add template for ghostty theme ([8306edb](https://github.com/thesimonho/kanagawa-paper.nvim/commit/8306edbee319320de020300eb6f634239c0cb89b))
* **ink:** set scrollbar to shade of the bg ([4c34918](https://github.com/thesimonho/kanagawa-paper.nvim/commit/4c349188c0876b020c08753ee2d9ab38a83a9327))
* **ink:** use brightened colors for bright ansi colors ([b2a8360](https://github.com/thesimonho/kanagawa-paper.nvim/commit/b2a8360b73d913f8a1c008e78b0ce9c6fee55591))
* **kitty:** add template for kitty extra ([191a5dc](https://github.com/thesimonho/kanagawa-paper.nvim/commit/191a5dc9f3d3eefc13f315ebdd977d7dde2503b3))
* **lazygit:** add template for lazygit extra ([c8b7cdf](https://github.com/thesimonho/kanagawa-paper.nvim/commit/c8b7cdf0b488bed83e24cb664c7d5120e55fd7af))
* **lsp:** using bg highlight for lspreferences ([89f65b7](https://github.com/thesimonho/kanagawa-paper.nvim/commit/89f65b7b9c0b8751318d7e98d58a9a7218afe3ce))
* **pywal:** remove pywal extra ([4c98a06](https://github.com/thesimonho/kanagawa-paper.nvim/commit/4c98a06c10962ede0f64c483c80c7fcb1702d38a))
* **terminal:** add template for windows terminal extra ([1524591](https://github.com/thesimonho/kanagawa-paper.nvim/commit/15245916aabae33ff060c66275eca1f17979f5d1))
* **terminator:** add template for terminator extra ([2f191bf](https://github.com/thesimonho/kanagawa-paper.nvim/commit/2f191bf69dafbf3f5100ad9ffbea631ca4147218))
* **termux:** add template for termux extra ([e9761e1](https://github.com/thesimonho/kanagawa-paper.nvim/commit/e9761e1dd31efca8fd82bb1713f9a9ba1099e1c3))
* **theme:** add default lotus colors ([aa96c99](https://github.com/thesimonho/kanagawa-paper.nvim/commit/aa96c99b85201505311d3d56c043c3b8f4b5a597))
* **theme:** add theme switching ([2220c56](https://github.com/thesimonho/kanagawa-paper.nvim/commit/2220c56a61093e51fe22be0ccfaeac3e25bf4824))
* **theme:** create new accent color ([651acd8](https://github.com/thesimonho/kanagawa-paper.nvim/commit/651acd83e524d9d8bcdddfce77c6c80a18e2e546))
* **tilix:** add template for tilix extra ([b246761](https://github.com/thesimonho/kanagawa-paper.nvim/commit/b24676178ccbd3470daca2543f5c272c56277e67))
* **utils:** add utils lib and hot reload for palette ([ed1119a](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **vscode_terminal:** add template for vscode terminal extra ([d8942ed](https://github.com/thesimonho/kanagawa-paper.nvim/commit/d8942eddd628e3da7c833b78fa79240e73b00bc4))
* **wezterm_tabline:** add template for wezterm tabline plugin ([bdd93df](https://github.com/thesimonho/kanagawa-paper.nvim/commit/bdd93df0f430f938cd62f740e283d41e71f25591))
* **wezterm:** add wezterm integration to auto switch the theme ([bd51421](https://github.com/thesimonho/kanagawa-paper.nvim/commit/bd514210dcfef8af4629fb02561420212e7923db))
* **wezterm:** add wezterm template ([66bae38](https://github.com/thesimonho/kanagawa-paper.nvim/commit/66bae38175261db0df9a0e5e6be397346e72f7b8))


### Bug Fixes

* **canvas:** bolder colors ([e7c9255](https://github.com/thesimonho/kanagawa-paper.nvim/commit/e7c92555efe43521add43da0975784e14e0707ca))
* **canvas:** improve indent colors ([e7c9255](https://github.com/thesimonho/kanagawa-paper.nvim/commit/e7c92555efe43521add43da0975784e14e0707ca))
* **canvas:** reduce saturation of canvas colors ([0449f68](https://github.com/thesimonho/kanagawa-paper.nvim/commit/0449f68a7963cb82571bb042a3f6e4d9fba2632c))
* **config:** fix theme overrides for multiple themes ([ad35e0e](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ad35e0ec1a8a85eacb4f48384011fee4fc8113e2))
* **config:** rename config options for consistency ([908f6a9](https://github.com/thesimonho/kanagawa-paper.nvim/commit/908f6a905cd103cb77f76f5c2e2e4b733b03e81a))
* **dev:** fix colour indicators during dev mode ([ed1119a](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ed1119a9841b04782e31b1673922cfd228b34286))
* **editor:** add fg color to visual selections so they're easier to read ([03969da](https://github.com/thesimonho/kanagawa-paper.nvim/commit/03969da8b17a1d47b1c630a96c0654c54e033322))
* **extras:** building with the wrong theme field ([52e7781](https://github.com/thesimonho/kanagawa-paper.nvim/commit/52e7781985f1c3ca82a6a69336e7b16bddd670e6))
* **extras:** set execute permissions ([c8ab889](https://github.com/thesimonho/kanagawa-paper.nvim/commit/c8ab889933cdc96e9b2e0c613c71187f0ce1c0dd))
* **float:** make float and pemu colors more consistent across themes ([d7be442](https://github.com/thesimonho/kanagawa-paper.nvim/commit/d7be44294f58c96759e68377d395e52248103918))
* **ink:** make diag backgrounds brighter ([3c386ad](https://github.com/thesimonho/kanagawa-paper.nvim/commit/3c386ad2993fb0b9f9acf4e9a0263da53965f6f2))
* **ink:** make gray more readable ([660e70d](https://github.com/thesimonho/kanagawa-paper.nvim/commit/660e70d33355a34c98c2344a53a2d5700d872258))
* **lazy:** fix consistency of lazy buttons ([5983df2](https://github.com/thesimonho/kanagawa-paper.nvim/commit/5983df26b5afb7abcf131c29e5f110a67f28ab60))
* **lsp:** make inlays and refs more subtle ([57363b5](https://github.com/thesimonho/kanagawa-paper.nvim/commit/57363b53976eec468f925cef803d5419e5b17977))
* **lsp:** unset lsp comment fg to allow TODO notes to show up correctly ([dd3a8d8](https://github.com/thesimonho/kanagawa-paper.nvim/commit/dd3a8d88df800277e1828dc70b90ca993ccc4a7f))
* **lualine:** add default theme for backward compat ([5ab4d0d](https://github.com/thesimonho/kanagawa-paper.nvim/commit/5ab4d0d6d0db19e15071c4d63a69489d14307ffd))
* **neotree:** make colors more distinctive ([fe859eb](https://github.com/thesimonho/kanagawa-paper.nvim/commit/fe859eb835d4cf2db7d2ac23ef23be10ab7cedf2))
* **noice:** fix command line search text readability ([b66f6fc](https://github.com/thesimonho/kanagawa-paper.nvim/commit/b66f6fc5fd331186483402432eb73ae7c91ceb53))
* **tabline:** make tabline colors easier to read ([9e93947](https://github.com/thesimonho/kanagawa-paper.nvim/commit/9e93947b4fc7bec733e8beaa6f2f18b55050aaac))
* **telescope:** add missing hlgroups ([917dcb8](https://github.com/thesimonho/kanagawa-paper.nvim/commit/917dcb84f9d72cfb59ad2c92d1d96af19e4fc292))
* **theme:** fix background changing behavior of static themes ([846941f](https://github.com/thesimonho/kanagawa-paper.nvim/commit/846941f54597f1864e932d5d48be16fbd70f1c9d))
* **theme:** fix dynamic theme loading ([67101b9](https://github.com/thesimonho/kanagawa-paper.nvim/commit/67101b9fbccd2f5d91c6d584925c7cdd13c3ef0f))
* **theme:** set relative light and dark colors for diag ([1c7c7e5](https://github.com/thesimonho/kanagawa-paper.nvim/commit/1c7c7e552711014294a01ccfb6e6abbe3888528b))
* **theme:** use blend for diag backgrounds ([d3dad2b](https://github.com/thesimonho/kanagawa-paper.nvim/commit/d3dad2b25b64450bef23e857c145d13e4110a96f))
* **treesitter_context:** fix line number coloring ([45ba977](https://github.com/thesimonho/kanagawa-paper.nvim/commit/45ba977cb9ff0fcd50e6c62b7959315c2f631de6))
* **treesitter:** standardize markdown headers on rainbow ([84511f2](https://github.com/thesimonho/kanagawa-paper.nvim/commit/84511f202e5427528f53ac26cf06d1b14302befa))
* **ts-context:** improve style of context window ([793dbbd](https://github.com/thesimonho/kanagawa-paper.nvim/commit/793dbbd14c48642a4ae2a8a7b56961f0b0091f15))
* **vcs:** use new vcs colors instead of base groups ([f5ab058](https://github.com/thesimonho/kanagawa-paper.nvim/commit/f5ab058de5b9b7020a10cf4646c48f29131ae4e4)), closes [#25](https://github.com/thesimonho/kanagawa-paper.nvim/issues/25)
* **wezterm_tabline:** add tab colors ([fed9212](https://github.com/thesimonho/kanagawa-paper.nvim/commit/fed9212989af02884cb5815c11c672ecc51aa195))
* **wezterm_tabline:** fix section A fg color ([bdd93df](https://github.com/thesimonho/kanagawa-paper.nvim/commit/bdd93df0f430f938cd62f740e283d41e71f25591))
* **yanky:** match yank highlight to visual selection color for consistency ([5b3327b](https://github.com/thesimonho/kanagawa-paper.nvim/commit/5b3327b91cc11fa94a949300fc4a1391eaf956d6))


### Performance Improvements

* **groups:** use simpler api for listing directory files ([49b7a23](https://github.com/thesimonho/kanagawa-paper.nvim/commit/49b7a23197157c2122030acfa711187d886f36c1))
* **lib:** cache common function calls ([c63eeb5](https://github.com/thesimonho/kanagawa-paper.nvim/commit/c63eeb54c127e2cc08c9b0801a23361442a12fd1))
* **plugins:** add cache for plugin lookup ([0095456](https://github.com/thesimonho/kanagawa-paper.nvim/commit/0095456027c0474f0659b8c669ba4c7e6ce7b971))

## [1.8.0](https://github.com/thesimonho/kanagawa-paper.nvim/compare/v1.7.0...v1.8.0) (2025-02-08)


### Features

* **blink:** add additional blink highlights ([a38356b](https://github.com/thesimonho/kanagawa-paper.nvim/commit/a38356b6520fadd710116352e9e98406c9e171c1))
* **blink:** add highlights for blink completion ([79bdc98](https://github.com/thesimonho/kanagawa-paper.nvim/commit/79bdc98ffdadaf5a9536a6fa108d3fcb235228ed))
* **extras:** add ghostty ([0aee289](https://github.com/thesimonho/kanagawa-paper.nvim/commit/0aee2893f0178fb7078b4c6e51fd780d64b046d4))
* **lsp:** add additional lsp types ([ec651cb](https://github.com/thesimonho/kanagawa-paper.nvim/commit/ec651cb118a2e5671b1f148a9e432f09e7bda7c3))
* **palette:** add darker sumiInk color ([dca5578](https://github.com/thesimonho/kanagawa-paper.nvim/commit/dca55783f2e4b847ba064370c61d877fd0a62cde))


### Bug Fixes

* **blink:** make source text more readable ([502cd71](https://github.com/thesimonho/kanagawa-paper.nvim/commit/502cd718eec01bb9fd6cbbd12bc6508f07ce1312))
* **dap:** make breakpoints and UI buttons more readable ([bf4a8a9](https://github.com/thesimonho/kanagawa-paper.nvim/commit/bf4a8a986cbc8f5c193adb2ed0cd2970f672040f))
* **lualine:** set the correct statusline color ([8da902e](https://github.com/thesimonho/kanagawa-paper.nvim/commit/8da902efd40818ec96d6881597efb60222a1c469))
* **lualine:** use darker color for inactive statusline ([108f0f5](https://github.com/thesimonho/kanagawa-paper.nvim/commit/108f0f52539a8c068796f277d1219f3d89a80960))
* **noice:** match cmdline search text to match color ([4abc704](https://github.com/thesimonho/kanagawa-paper.nvim/commit/4abc704f0f1ab68c8e10e5169ea7c4676b3adadf))
* **snacks:** set color for indents ([74f9110](https://github.com/thesimonho/kanagawa-paper.nvim/commit/74f911042c9901d8556fa7a5093912126cb3db2a))
* **treesitter:** set underline color ([63e61fd](https://github.com/thesimonho/kanagawa-paper.nvim/commit/63e61fdc784dc5a13e2301a60d354a0ce58a0096))
* **treesitter:** use underline for urls ([728081f](https://github.com/thesimonho/kanagawa-paper.nvim/commit/728081fe096c645a937a7784e6cbf73ec1b97d83))
* **trouble:** make trouble counts more readable ([21c86a4](https://github.com/thesimonho/kanagawa-paper.nvim/commit/21c86a44e7294526d4f65394c997b5c60280ea73))

## [1.7.0](https://github.com/sho-87/kanagawa-paper.nvim/compare/v1.6.0...v1.7.0) (2024-12-03)


### Features

* **fzf:** add color scheme for fzf ([c510f4c](https://github.com/sho-87/kanagawa-paper.nvim/commit/c510f4c6461f00753ff0c03e68e368eb6ba217e1)), closes [#17](https://github.com/sho-87/kanagawa-paper.nvim/issues/17)


### Bug Fixes

* **diff:** make changed diff text more readable ([a3a6320](https://github.com/sho-87/kanagawa-paper.nvim/commit/a3a6320997a022b3546f62335b6442853fc76191))
* **extras:** make wezterm highlights more readable ([ca32d10](https://github.com/sho-87/kanagawa-paper.nvim/commit/ca32d10d59d73f5fee728b9e03bb88e966e5ca18))
* **neogit:** use default neogit colors for diffs ([2856b25](https://github.com/sho-87/kanagawa-paper.nvim/commit/2856b250977c3c7a30f10019a82328f660a7f730)), closes [#18](https://github.com/sho-87/kanagawa-paper.nvim/issues/18)

## [1.6.0](https://github.com/sho-87/kanagawa-paper.nvim/compare/v1.5.0...v1.6.0) (2024-10-12)


### Features

* add hl for markdown.nvim headers ([c1fac34](https://github.com/sho-87/kanagawa-paper.nvim/commit/c1fac349097dab206f1bf8481976bdb89bba995c))
* **barbar:** fix background when using transparent theme ([e264574](https://github.com/sho-87/kanagawa-paper.nvim/commit/e2645741fd9f6ec7da149135e181a70bc3725ad6))
* **extras:** add color overrides for wezterm tabline ([66053e5](https://github.com/sho-87/kanagawa-paper.nvim/commit/66053e59a7e28cb9e8df542c41f588acebec223e))
* **grug-far:** add hl for grug-far ([197f0e8](https://github.com/sho-87/kanagawa-paper.nvim/commit/197f0e83876997be12aaedf20d7c608c3a469daa))


### Bug Fixes

* **barbar:** fix bolding of a few elements ([07d9685](https://github.com/sho-87/kanagawa-paper.nvim/commit/07d9685e9e1724bb30d543959c8ccf2432e4f2bc))
* **editor:** differentiate cursorline and visual selection colors ([1a4909c](https://github.com/sho-87/kanagawa-paper.nvim/commit/1a4909caf86013280226a8391391e44ff3fe35e4)), closes [#14](https://github.com/sho-87/kanagawa-paper.nvim/issues/14)
* **editor:** winbar typo ([5067fa5](https://github.com/sho-87/kanagawa-paper.nvim/commit/5067fa5a27c57bfee29cb2c4099933da3bb12707))
* **headlines:** reduce brightness of markdown header bg ([341adbe](https://github.com/sho-87/kanagawa-paper.nvim/commit/341adbef7b9ca09a3290fa855932ef8594c931bb))
* **indent:** make indent lines brighter ([71b3360](https://github.com/sho-87/kanagawa-paper.nvim/commit/71b33609ec2b782921c763054a37472b507c1e43))
* **lsp:** remove inlay and codelens bg for transparent themes ([e7eb180](https://github.com/sho-87/kanagawa-paper.nvim/commit/e7eb180bfd776fe41dba613fe19fbc6ff7229484))
* **lsp:** tweak some LSP colors (inlayhints, modules) ([5969bfa](https://github.com/sho-87/kanagawa-paper.nvim/commit/5969bfa1b0e464ddc87f4f1b788b89103245a7cb))
* **markdown:** fix header colors ([cb5b597](https://github.com/sho-87/kanagawa-paper.nvim/commit/cb5b5978654651d37d22066c9b59d2a38489bc36))
* **markdown:** remove underline from markdown links ([4376cd2](https://github.com/sho-87/kanagawa-paper.nvim/commit/4376cd26f43b5b8ddf58f25b3908347b34754e09))
* **vcs:** add darker diff colors ([928f0f4](https://github.com/sho-87/kanagawa-paper.nvim/commit/928f0f4f28475111d0b507c27b243744648bac1f))

## [1.5.0](https://github.com/sho-87/kanagawa-paper.nvim/compare/v1.4.1...v1.5.0) (2024-07-15)


### Features

* **gitgutter:** add hl for gitgutter ([5c8095c](https://github.com/sho-87/kanagawa-paper.nvim/commit/5c8095c1fba5f133810e70926ede58620474c879))
* **indent:** add hl for indent line character ([06bc994](https://github.com/sho-87/kanagawa-paper.nvim/commit/06bc994416ea2a503a3a171f2fff929f9b12c623))
* **neotest:** add hl for neotest ([3407e75](https://github.com/sho-87/kanagawa-paper.nvim/commit/3407e75ab67131dcd0045a9a3854e429de9fff19))
* **octo:** add hl for octo ([94954b6](https://github.com/sho-87/kanagawa-paper.nvim/commit/94954b6e6771e381ba85a8f21597eaa8d6403d8e))
* **overseer:** add hl for overseer ([8a40bf2](https://github.com/sho-87/kanagawa-paper.nvim/commit/8a40bf2cb9d81af1c036de378beb04417280e3e2))
* **rainbow:** add hl for rainbow ([8858669](https://github.com/sho-87/kanagawa-paper.nvim/commit/8858669f93a9b66c44d5734e0b7283bfa747cc0a))
* **which-key:** add hl for the title ([05c0e0b](https://github.com/sho-87/kanagawa-paper.nvim/commit/05c0e0b02d75254dc7ccadb06caff48ae6b67177))
* **windowpicker:** add hl for window picker letter ([bbf1a7b](https://github.com/sho-87/kanagawa-paper.nvim/commit/bbf1a7b1d3a0b7eb61d69c371401e59062f31f55))


### Bug Fixes

* **yanky:** link highlights to visual and insert mode colors ([66596b9](https://github.com/sho-87/kanagawa-paper.nvim/commit/66596b9260b17542e5f7eb6faf7b27f044970b77))

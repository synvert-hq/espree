# Changelog

## [11.0.0](https://github.com/xinminlabs/espree/compare/v10.0.1...v11.0.0) (2024-04-07)


### ⚠ BREAKING CHANGES

* Require Node.js ^18.18.0 || ^20.9.0 || >=21.1.0 ([#589](https://github.com/xinminlabs/espree/issues/589))

### Features

* add `allowReserved` for ES3 ([#522](https://github.com/xinminlabs/espree/issues/522)) ([e807c20](https://github.com/xinminlabs/espree/commit/e807c2061f97fb0f8c8db3d2c5981731f9bf4a22))
* Add parser name ([#562](https://github.com/xinminlabs/espree/issues/562)) ([4368788](https://github.com/xinminlabs/espree/commit/43687882d30855033ec4db0a11514aa85c0dd8d0))
* Add sourceType:commonjs support ([#520](https://github.com/xinminlabs/espree/issues/520)) ([27713ac](https://github.com/xinminlabs/espree/commit/27713aca32c73347750f9033841f176f5cb83951))
* Require Node.js ^18.18.0 || ^20.9.0 || &gt;=21.1.0 ([#589](https://github.com/xinminlabs/espree/issues/589)) ([e79cfa4](https://github.com/xinminlabs/espree/commit/e79cfa490aa2d23c7d4deda0e99f2190e508a638))
* support arbitrary module namespace names ([#528](https://github.com/xinminlabs/espree/issues/528)) ([8655f3d](https://github.com/xinminlabs/espree/commit/8655f3d4d442da3b170ddbf2a84d29dfc41ba072))
* support class static blocks ([#518](https://github.com/xinminlabs/espree/issues/518)) ([fe07aae](https://github.com/xinminlabs/espree/commit/fe07aae683f3c09fe1cd0165a98e11339c22ab7c))
* Support ES2023 and hashbangs ([#556](https://github.com/xinminlabs/espree/issues/556)) ([411d697](https://github.com/xinminlabs/espree/commit/411d697af3e65c92c13921bfb7baa7aad60242eb))
* Support ES2024 and regexp v flag ([#575](https://github.com/xinminlabs/espree/issues/575)) ([4cfc062](https://github.com/xinminlabs/espree/commit/4cfc0626c534377601d48e8cad38976da6b85964))
* support for private-in syntax ([#521](https://github.com/xinminlabs/espree/issues/521)) ([6839389](https://github.com/xinminlabs/espree/commit/6839389b9c67f0e6cbda00802867e7cf0ccd75eb))


### Bug Fixes

* "await" is a future reserved word (fixes [#151](https://github.com/xinminlabs/espree/issues/151)) ([95d388d](https://github.com/xinminlabs/espree/commit/95d388dcf03b71f70f25b8429f78a1333c41c491))
* "use strict" should not trigger strict mode in es3. ([#547](https://github.com/xinminlabs/espree/issues/547)) ([6c718af](https://github.com/xinminlabs/espree/commit/6c718af090c1b5dd25d74a2ecfc65fbee0c00716))
* `}` token followed by template had been lost (fixes [#293](https://github.com/xinminlabs/espree/issues/293)) ([#294](https://github.com/xinminlabs/espree/issues/294)) ([80abdce](https://github.com/xinminlabs/espree/commit/80abdcee41d0c6b1cd33cd70b2fd1706ff41fe8e))
* 0x2028 and 0x2029 in string literals should increment line number ([#514](https://github.com/xinminlabs/espree/issues/514)) ([ee1d3ec](https://github.com/xinminlabs/espree/commit/ee1d3eca310cab1b1cf1563294434977d26358d4))
* Actuall fix tokenization issue with templates (fixes [#44](https://github.com/xinminlabs/espree/issues/44)) ([4f4e524](https://github.com/xinminlabs/espree/commit/4f4e524ad3df40c736ba6f99c33ea96b3b9dfd70))
* add AwaitExpression to espree.Syntax (fixes [#331](https://github.com/xinminlabs/espree/issues/331)) ([#332](https://github.com/xinminlabs/espree/issues/332)) ([343590a](https://github.com/xinminlabs/espree/commit/343590a66e7f210689766dbdf5c6a4b0ca91c58a))
* Add test for leading comments (fixes [#136](https://github.com/xinminlabs/espree/issues/136)) ([22290b9](https://github.com/xinminlabs/espree/commit/22290b982ae456449da39fa91de83c1fa3452f01))
* Allow AssignmentExpression in object spread (fixes [#167](https://github.com/xinminlabs/espree/issues/167)) ([b12548b](https://github.com/xinminlabs/espree/commit/b12548bb4a92f854c000bd8329167880ee665c5a))
* Allow computed generators in classes (fixes [#123](https://github.com/xinminlabs/espree/issues/123)) ([afca198](https://github.com/xinminlabs/espree/commit/afca1982d03f4e417c0eb847adf1ac8b3d54043e))
* Allow let/const in switchcase (fixes [#54](https://github.com/xinminlabs/espree/issues/54)) ([457de85](https://github.com/xinminlabs/espree/commit/457de854bfa2232fb2274154d575b55b6bf10983))
* Allow super in classes by default (fixes [#87](https://github.com/xinminlabs/espree/issues/87)) ([6cae452](https://github.com/xinminlabs/espree/commit/6cae4521c9747d80266a708ad300de62d901d0ca))
* Allow yield without value as function param (fixes [#134](https://github.com/xinminlabs/espree/issues/134)) ([d56a2b1](https://github.com/xinminlabs/espree/commit/d56a2b170f5e247400033c4c0ead2599412f333e))
* async shorthand properties (fixes [#340](https://github.com/xinminlabs/espree/issues/340)) ([#341](https://github.com/xinminlabs/espree/issues/341)) ([be85b8e](https://github.com/xinminlabs/espree/commit/be85b8e97eafc502f9d3150eb5d324639d308051))
* bad error in parsing invalid class setter (fixes [#98](https://github.com/xinminlabs/espree/issues/98)) ([03b1fa4](https://github.com/xinminlabs/espree/commit/03b1fa42912e4982f855890d11ee20d27d60ccff))
* build failing due to incorrectly super() call (fixes [#398](https://github.com/xinminlabs/espree/issues/398)) ([#399](https://github.com/xinminlabs/espree/issues/399)) ([7c278d6](https://github.com/xinminlabs/espree/commit/7c278d6acc6b5db86b803d0cd21b830deb6f569e))
* Catch ES2016 invalid syntax (fixes [#284](https://github.com/xinminlabs/espree/issues/284)) ([#285](https://github.com/xinminlabs/espree/issues/285)) ([ff15922](https://github.com/xinminlabs/espree/commit/ff15922f3c9b06d0bbf5b01c1ce17ab44f3326b5))
* Class name should be id (fixes [#78](https://github.com/xinminlabs/espree/issues/78)) ([7b6ed2c](https://github.com/xinminlabs/espree/commit/7b6ed2c92d00fd63db9ed81e39c1b1aeb9d2e07c))
* Convert ~ and ! prefix tokens to esprima (fixes [#274](https://github.com/xinminlabs/espree/issues/274)) ([#276](https://github.com/xinminlabs/espree/issues/276)) ([7df2e4a](https://github.com/xinminlabs/espree/commit/7df2e4ae48ee91c54f42f5ecbb1473bcd80a9021))
* Deeply nested template literals (fixes [#86](https://github.com/xinminlabs/espree/issues/86)) ([6fd88d3](https://github.com/xinminlabs/espree/commit/6fd88d322e201ffd7cc332929e0dc091ec50bc3e))
* Derive espree.Syntax from espree.VisitorKeys ([#532](https://github.com/xinminlabs/espree/issues/532)) ([64010de](https://github.com/xinminlabs/espree/commit/64010de254892c89376f56bd88aa07ef9382dda8))
* Destructured arg for catch (fixes [#105](https://github.com/xinminlabs/espree/issues/105)) ([d8a6f69](https://github.com/xinminlabs/espree/commit/d8a6f698cdd493cfd0c9cf29de7f296142d20712))
* Destructured Defaults (fixes [#56](https://github.com/xinminlabs/espree/issues/56)) ([0ddf492](https://github.com/xinminlabs/espree/commit/0ddf4929be7897b410aad4d1ac9a7d1b3ddc2232))
* disallow import/export in functions (refs [#72](https://github.com/xinminlabs/espree/issues/72)) ([e715c06](https://github.com/xinminlabs/espree/commit/e715c06ee7a69b1007e2c819a9bd6d0be68f3c04))
* Disallow namespaces objects in JSX (fixes [#261](https://github.com/xinminlabs/espree/issues/261)) ([c7e5a13](https://github.com/xinminlabs/espree/commit/c7e5a13b7f3029a1eddf7d7edbba53ec714cb498))
* Disallow octals in template strings (fixes [#96](https://github.com/xinminlabs/espree/issues/96)) ([4f763b0](https://github.com/xinminlabs/espree/commit/4f763b0ee1224c3c16ae2ef384b64161ce982335))
* Don't allow arrow function rest param (fixes [#130](https://github.com/xinminlabs/espree/issues/130)) ([491f879](https://github.com/xinminlabs/espree/commit/491f879aa2b0a71cd99a48a185698c894e8e637a))
* Don't allow default export class by mistake (fixes [#82](https://github.com/xinminlabs/espree/issues/82)) ([66fa479](https://github.com/xinminlabs/espree/commit/66fa479dcc281c9d1c1cfdde0852011a11700669))
* Don't allow regex y flag in ES5 ([73a079c](https://github.com/xinminlabs/espree/commit/73a079c7e17ed0a68b44ab0b3f480ace6776fe4d))
* don't mutate user-provided configs (fixes [#329](https://github.com/xinminlabs/espree/issues/329)) ([#330](https://github.com/xinminlabs/espree/issues/330)) ([628cf3a](https://github.com/xinminlabs/espree/commit/628cf3a1006b6d8bbc47c25438521b1d57c10371))
* don't recognize directives in ES3, allow parenthesized rest target ([#554](https://github.com/xinminlabs/espree/issues/554)) ([b1eac6d](https://github.com/xinminlabs/espree/commit/b1eac6d9687b2cb48dd28e8c11626afde22fa6cf))
* Ensur object rest works in destructed arg (fixes [#213](https://github.com/xinminlabs/espree/issues/213)) ([8aa05fa](https://github.com/xinminlabs/espree/commit/8aa05fad8c381f23c6c37108099c2b422a5e8953))
* Ensure 'var let' works (fixes [#149](https://github.com/xinminlabs/espree/issues/149)) ([a2b23ca](https://github.com/xinminlabs/espree/commit/a2b23ca088662335624694930509aefc4012c59d))
* Ensure class declarations must have IDs outside of exports (refs [#72](https://github.com/xinminlabs/espree/issues/72)) ([7fe5865](https://github.com/xinminlabs/espree/commit/7fe58655306c4824d8bc9ec89b5f9f92394eaec0))
* Ensure node type is correct for destructured (fixes [#195](https://github.com/xinminlabs/espree/issues/195)) ([98e5fd9](https://github.com/xinminlabs/espree/commit/98e5fd94958d26890fc18b39179d6a408f038f5e))
* exponentiation operator token (fixes [#254](https://github.com/xinminlabs/espree/issues/254)) ([3614e81](https://github.com/xinminlabs/espree/commit/3614e81dea835a07911a5ae815be688caff43398))
* export class expression support (refs [#72](https://github.com/xinminlabs/espree/issues/72)) ([8d86b85](https://github.com/xinminlabs/espree/commit/8d86b85985f6024215277d396f8f11f075fef44a))
* Export default function should be FunctionDeclaration (fixes [#81](https://github.com/xinminlabs/espree/issues/81)) ([42ce538](https://github.com/xinminlabs/espree/commit/42ce538f1afe5e57e1e87b9bcece696f6a81fd57))
* Extend property method range and loc to include params (fixes [#36](https://github.com/xinminlabs/espree/issues/36)) ([b4aa879](https://github.com/xinminlabs/espree/commit/b4aa87962369849738eb181358aec8fff98d8dd3))
* Fix behavior of ignoring comments within previous nodes (refs [#256](https://github.com/xinminlabs/espree/issues/256)) ([98441cb](https://github.com/xinminlabs/espree/commit/98441cb4eb3dd1ad34c0b97df862aa89816f80c2))
* Fix parsing of async keyword-named object methods ([#352](https://github.com/xinminlabs/espree/issues/352)) ([#353](https://github.com/xinminlabs/espree/issues/353)) ([5eb1388](https://github.com/xinminlabs/espree/commit/5eb1388809c789e50cdb56bf90192f0df36a3987))
* generator methods in classes (fixes [#85](https://github.com/xinminlabs/espree/issues/85)) ([9eac2ef](https://github.com/xinminlabs/espree/commit/9eac2efdc99e1db6993a49301e4df5cb68e348e8))
* generic error for invalid ecmaVersion(fixes eslint[#7405](https://github.com/xinminlabs/espree/issues/7405)) ([#303](https://github.com/xinminlabs/espree/issues/303)) ([58f75be](https://github.com/xinminlabs/espree/commit/58f75be6b89d8904b6366ed368045cb02c4a4e33))
* Incomplete Switch Statement Hangs (Fixes [#146](https://github.com/xinminlabs/espree/issues/146)) ([8adbbc8](https://github.com/xinminlabs/espree/commit/8adbbc8f38987252dc8ce3a1213673f71ee2a4e8))
* Incorrect error location (fixes [#173](https://github.com/xinminlabs/espree/issues/173)) ([38576c5](https://github.com/xinminlabs/espree/commit/38576c59e57463d277f026cac2dd33bba5d52566))
* incorrectly parsed arrow fragment (refs [#58](https://github.com/xinminlabs/espree/issues/58)) ([999e031](https://github.com/xinminlabs/espree/commit/999e0314d5b1520e5299465dfb3dead759feee9d))
* lastToken not reset between calls to parse (fixes [#229](https://github.com/xinminlabs/espree/issues/229)) ([ef7a06d](https://github.com/xinminlabs/espree/commit/ef7a06dfc6a5e3b397d8cce483b9e1ce331d0da1))
* leading comments added from previous node (fixes [#256](https://github.com/xinminlabs/espree/issues/256)) ([d1b4929](https://github.com/xinminlabs/espree/commit/d1b4929595aa9030374afaf74db074d08cd92a03))
* Leading comments for anonymous classes (fixes [#155](https://github.com/xinminlabs/espree/issues/155), fixes [#158](https://github.com/xinminlabs/espree/issues/158)) ([d535900](https://github.com/xinminlabs/espree/commit/d535900533b895a88ee6caf1d58c4799b2f9d261))
* Make obj.await work in modules (fixes [#258](https://github.com/xinminlabs/espree/issues/258)) ([5783282](https://github.com/xinminlabs/espree/commit/5783282aa8e4133f2468be564a01187d1a547caf))
* Make template token objects adhere to token object structure ([#343](https://github.com/xinminlabs/espree/issues/343)) ([d4bdcb6](https://github.com/xinminlabs/espree/commit/d4bdcb60a01ca3988e9c5aebb1036d7fc304386c)), closes [#319](https://github.com/xinminlabs/espree/issues/319)
* misuse token types (fixes [#393](https://github.com/xinminlabs/espree/issues/393), refs eslint/eslint[#11018](https://github.com/xinminlabs/espree/issues/11018)) ([#426](https://github.com/xinminlabs/espree/issues/426)) ([70c4970](https://github.com/xinminlabs/espree/commit/70c4970e5eba6f060e1e32a22d231647f2d0e0f8))
* nested arrow function as default param (fixes [#145](https://github.com/xinminlabs/espree/issues/145)) ([ee4ea43](https://github.com/xinminlabs/espree/commit/ee4ea437c221ec1353838db86d14057e46f192c0))
* newlines in arrow functions (fixes [#172](https://github.com/xinminlabs/espree/issues/172)) ([2b85a1d](https://github.com/xinminlabs/espree/commit/2b85a1d2175f28f211b41521a4178049e08eb507))
* npm browserify (fixes [#156](https://github.com/xinminlabs/espree/issues/156)) ([f4c2642](https://github.com/xinminlabs/espree/commit/f4c2642c008548597148e877c0d7c83c9cce7b77))
* Object rest/spread in assign (fixes [#247](https://github.com/xinminlabs/espree/issues/247)) ([ea6261e](https://github.com/xinminlabs/espree/commit/ea6261eb962a04a191c01e16387faddfdea48352))
* parse unicode escapes in identifiers (fixes [#181](https://github.com/xinminlabs/espree/issues/181)) ([72f22bf](https://github.com/xinminlabs/espree/commit/72f22bf452cc439c727cbb793373e0d092c93c88))
* parsing error on `async` as property name. ([#295](https://github.com/xinminlabs/espree/issues/295)) ([9810bab](https://github.com/xinminlabs/espree/commit/9810babfa585255d63a38c5d15e525fef94d94a7))
* raise error for trailing commas after rest properties (fixes [#310](https://github.com/xinminlabs/espree/issues/310)) ([#323](https://github.com/xinminlabs/espree/issues/323)) ([652990a](https://github.com/xinminlabs/espree/commit/652990a7bfeb9eca2041e8cbb696de671522d420))
* Remove blockBindings from docs (fixes [#307](https://github.com/xinminlabs/espree/issues/307), fixes [#339](https://github.com/xinminlabs/espree/issues/339)) ([#356](https://github.com/xinminlabs/espree/issues/356)) ([019b70a](https://github.com/xinminlabs/espree/commit/019b70a13583cbb2aa801f8b9161dafc2a7fe982))
* remove extra leading comments at node level (fixes [#264](https://github.com/xinminlabs/espree/issues/264)) ([e044705](https://github.com/xinminlabs/espree/commit/e04470519f181baa281f406c112d4184d10031a7))
* remove useless sourcemap url (fixes [#566](https://github.com/xinminlabs/espree/issues/566)) ([#567](https://github.com/xinminlabs/espree/issues/567)) ([37f6b17](https://github.com/xinminlabs/espree/commit/37f6b17376efc2e93441ef3dc28d347918c475f0))
* remove workarounds for acorn &lt; 4 ([#372](https://github.com/xinminlabs/espree/issues/372)) ([56c5a9c](https://github.com/xinminlabs/espree/commit/56c5a9c7fb01bd7ba338d16c1c63d89d5b8ee8b6)), closes [#338](https://github.com/xinminlabs/espree/issues/338)
* reset `isAsync` flag for each property (fixes [#298](https://github.com/xinminlabs/espree/issues/298)) ([#299](https://github.com/xinminlabs/espree/issues/299)) ([7d3e2fc](https://github.com/xinminlabs/espree/commit/7d3e2fc812fe6aa1e656b2b7c4b86ac323baf421))
* Rest Params & Arrow Functions (fixes [#187](https://github.com/xinminlabs/espree/issues/187)) ([908617d](https://github.com/xinminlabs/espree/commit/908617d3410de8e35aea584afeb9db9115eaf2a0))
* shorthand properties named get or set (fixes [#100](https://github.com/xinminlabs/espree/issues/100)) ([de5d97a](https://github.com/xinminlabs/espree/commit/de5d97a9466ee8d8c00fe36be98c70e0b74a5d5d))
* Tagged template strings (fixes [#110](https://github.com/xinminlabs/espree/issues/110)) ([b6301f9](https://github.com/xinminlabs/espree/commit/b6301f92c05f8d8979a0c9f347c84f34bb5013bb))
* Template string parsing (fixes [#95](https://github.com/xinminlabs/espree/issues/95)) ([d02deed](https://github.com/xinminlabs/espree/commit/d02deed4341f3a6a7a1fa6b7f456c2176236c6b2))
* tests for importing keywords (fixes [#225](https://github.com/xinminlabs/espree/issues/225)) ([b07696f](https://github.com/xinminlabs/espree/commit/b07696fa0924b33d33fd02986439c03e0e35cb59))
* tokenize the latest right curly brace (fixes [#403](https://github.com/xinminlabs/espree/issues/403)) ([#419](https://github.com/xinminlabs/espree/issues/419)) ([3f49224](https://github.com/xinminlabs/espree/commit/3f49224eb05f6b8cb1b996ce424a99c40978b389))
* trailing commas in import/export (fixes [#148](https://github.com/xinminlabs/espree/issues/148)) ([7cdc7e4](https://github.com/xinminlabs/espree/commit/7cdc7e4c4dd802c949c5bc2fad8c6cedbb40d82c))
* Update broken tests ([f3ed96a](https://github.com/xinminlabs/espree/commit/f3ed96a39eb8201caf12f3fc44a10fa065fac300))
* upgrade acorn v8.11.3 ([#590](https://github.com/xinminlabs/espree/issues/590)) ([6d30382](https://github.com/xinminlabs/espree/commit/6d303829686dd1e3a425438e816025d7193ec915))
* use the plugins feature of acorn (fixes [#250](https://github.com/xinminlabs/espree/issues/250)) ([106000f](https://github.com/xinminlabs/espree/commit/106000f10a8ab26a6bf2fd0de8ba01f1e525b891))
* Yield as identifier in arrow func args (fixes [#165](https://github.com/xinminlabs/espree/issues/165)) ([725e9f9](https://github.com/xinminlabs/espree/commit/725e9f9829c04c4ed75a503fec356aed3c9ab4e1))
* Yield should parse without an argument (fixes [#121](https://github.com/xinminlabs/espree/issues/121)) ([8ae98cf](https://github.com/xinminlabs/espree/commit/8ae98cf7e2c2816f7961ab47fe56ade9f8f396b1))


### Documentation

* Add badges ([#326](https://github.com/xinminlabs/espree/issues/326)) ([15ef24f](https://github.com/xinminlabs/espree/commit/15ef24fa00c79fb581b54cb0cd04927c8729288a))
* add private-in syntax ([#523](https://github.com/xinminlabs/espree/issues/523)) ([34b9a6a](https://github.com/xinminlabs/espree/commit/34b9a6a08efe6089748c1a330c0e30b18eaf6785))
* Add security policy ([#447](https://github.com/xinminlabs/espree/issues/447)) ([91c2d58](https://github.com/xinminlabs/espree/commit/91c2d5896889042058399cd64de4b218c5add0eb))
* added missing `ecmaFeatures.superInFunctions` option from doc ([906adad](https://github.com/xinminlabs/espree/commit/906adad3086a81b3cde5b0c69918b1056c2b1f55))
* Autogenerated changelog for 3.0.2 ([55d7f22](https://github.com/xinminlabs/espree/commit/55d7f22d1d92bd7321577501c2774fe586630374))
* Autogenerated changelog for 3.1.0 ([50286d5](https://github.com/xinminlabs/espree/commit/50286d50a3437ed65895173c4256a016dc8c3181))
* Autogenerated changelog for 3.1.1 ([2d69214](https://github.com/xinminlabs/espree/commit/2d6921498f3056ae690e200d169a4fd3d59fb5cf))
* Autogenerated changelog for 3.1.2 ([3ef57a1](https://github.com/xinminlabs/espree/commit/3ef57a16543484564a5e20c134c0c2f05f13f9a7))
* Autogenerated changelog for 3.1.3 ([27eea64](https://github.com/xinminlabs/espree/commit/27eea648f2bcfe15e546e95e170f484073d36ab0))
* Autogenerated changelog for 3.1.4 ([ba47069](https://github.com/xinminlabs/espree/commit/ba47069ecda1a14fc5a578c646251ce95c09cc96))
* Autogenerated changelog for 3.1.5 ([08e071a](https://github.com/xinminlabs/espree/commit/08e071a1218b021773ce93797a37928941cf6a7b))
* Autogenerated changelog for 3.1.6 ([60d263d](https://github.com/xinminlabs/espree/commit/60d263d8b66a8b21ed8f69dcd474d25b7f30fc76))
* Autogenerated changelog for v3.0.0 ([3a331c2](https://github.com/xinminlabs/espree/commit/3a331c2cb14d46f5615e9e81efb3b7742844ae97))
* Autogenerated changelog for v3.0.1 ([af1a1ba](https://github.com/xinminlabs/espree/commit/af1a1ba27396ef54f178fdeaccae7d998fb5262a))
* Clarify ecmaFeatures usage ([bea54c7](https://github.com/xinminlabs/espree/commit/bea54c780d2c41736f1925cd2622800493ab0bf4))
* Clean up LICENSE file ([#445](https://github.com/xinminlabs/espree/issues/445)) ([0cc7800](https://github.com/xinminlabs/espree/commit/0cc78007c933564f32fd849bd8022992845c3ac1))
* Correct license info on README (fixes [#117](https://github.com/xinminlabs/espree/issues/117)) ([a167542](https://github.com/xinminlabs/espree/commit/a1675428aa78967c2946e8817c7d3288b4714bb3))
* documenting public API (fixes [#431](https://github.com/xinminlabs/espree/issues/431)) ([#442](https://github.com/xinminlabs/espree/issues/442)) ([6048bfe](https://github.com/xinminlabs/espree/commit/6048bfe3939fa7dc162c0b3c4b043bb410736b0b))
* fix `options.comment` typo ([7e57ee0](https://github.com/xinminlabs/espree/commit/7e57ee0f384de9bb3970d69eff22de627bad4123))
* Fix some minor typos in the READMEs ([#455](https://github.com/xinminlabs/espree/issues/455)) ([4c70052](https://github.com/xinminlabs/espree/commit/4c70052df0b0ba903602c1f838918cbc07ee5eca))
* Fix some typos in the README ([#386](https://github.com/xinminlabs/espree/issues/386)) ([6bf2ebf](https://github.com/xinminlabs/espree/commit/6bf2ebf272d13e5df24f62e9e1a5d09471cde963))
* new site for docs ([#436](https://github.com/xinminlabs/espree/issues/436)) ([9b91bcc](https://github.com/xinminlabs/espree/commit/9b91bccacea15c75025a62bae828f83598aef5fe))
* replace a dead link with the correct contributing guide URL ([3a90886](https://github.com/xinminlabs/espree/commit/3a908866528f565e0f856812cec9daf6515724cc))
* Specify default values of options (fixes [#325](https://github.com/xinminlabs/espree/issues/325)) ([#342](https://github.com/xinminlabs/espree/issues/342)) ([16e1fec](https://github.com/xinminlabs/espree/commit/16e1fec5a30e298de441d682575e0c6055afb583))
* update Build Status badge ([#536](https://github.com/xinminlabs/espree/issues/536)) ([c915190](https://github.com/xinminlabs/espree/commit/c9151901be91b21a027478d2603862460fccf78f))
* Update license copyright ([d6b383d](https://github.com/xinminlabs/espree/commit/d6b383d72002729d1d4b509d07c9aeb39987a9cc))
* Update README ([e4b561c](https://github.com/xinminlabs/espree/commit/e4b561c2dd543cce0869a077c0fc158e1d5b1990))
* update README for ECMAScript 2023 ([#557](https://github.com/xinminlabs/espree/issues/557)) ([30f5f2f](https://github.com/xinminlabs/espree/commit/30f5f2fe258fc32bb4d5b4b3bbf4d6aef13b6d1d))
* update readme to mention ES2020 ([#422](https://github.com/xinminlabs/espree/issues/422)) ([c0635ba](https://github.com/xinminlabs/espree/commit/c0635bac4cd891cb612fb81655012e2579f4e2b1))
* Update README with ESM instructions (fixes [#474](https://github.com/xinminlabs/espree/issues/474)) ([#477](https://github.com/xinminlabs/espree/issues/477)) ([671c3aa](https://github.com/xinminlabs/espree/commit/671c3aa55bd9ece231f2f28417d557d264994107))
* Update README with latest info ([9b5ad0f](https://github.com/xinminlabs/espree/commit/9b5ad0f970ebe51e3c0c9d29bdaeafb400cf4d25))
* Update README.md ([b942b31](https://github.com/xinminlabs/espree/commit/b942b31b1b9844ad2604c8fca46ac284016c03ad))


### Build Related

* Add CI release ([8f6cfbd](https://github.com/xinminlabs/espree/commit/8f6cfbdf160f31a865e9e58b705b80d363b90e83))
* Add CI release scripts ([8d9767d](https://github.com/xinminlabs/espree/commit/8d9767d4344c5a95894ba8a3f5ce87c9d4cf325a))
* add node 10 ([#381](https://github.com/xinminlabs/espree/issues/381)) ([4207773](https://github.com/xinminlabs/espree/commit/4207773d475b4096856ed0604e30da525999b122))
* add node 11 ([#400](https://github.com/xinminlabs/espree/issues/400)) ([4b86a7d](https://github.com/xinminlabs/espree/commit/4b86a7dc7c447c11bb6530e46dc43428ce2bd372))
* add node 12 ([#414](https://github.com/xinminlabs/espree/issues/414)) ([a988a36](https://github.com/xinminlabs/espree/commit/a988a36e436a1ab6c84005ba0adb6cf9c262c1ec))
* add node v16 ([#481](https://github.com/xinminlabs/espree/issues/481)) ([ecaf510](https://github.com/xinminlabs/espree/commit/ecaf510e03f5864e546eb7f60728fbc488fc8543))
* add node v17 ([#516](https://github.com/xinminlabs/espree/issues/516)) ([6be7bcb](https://github.com/xinminlabs/espree/commit/6be7bcb43f7bc10cc1f04f53ace3eb1e2d3f11bb))
* add node v18 ([#546](https://github.com/xinminlabs/espree/issues/546)) ([75f65eb](https://github.com/xinminlabs/espree/commit/75f65eb2915438abd3ebd91dd62431456502e1db))
* Add Node.js 0.12 testing ([cffe44e](https://github.com/xinminlabs/espree/commit/cffe44ef5016332a0578712c5c5635d116db5c58))
* Add node@5 to CI (fixes [#237](https://github.com/xinminlabs/espree/issues/237)) ([2e2808a](https://github.com/xinminlabs/espree/commit/2e2808a83a2251005c14d87799a621fa484abf79))
* Add prerelease script ([dd5863e](https://github.com/xinminlabs/espree/commit/dd5863e569473f2d72973a416687f41fdd5f9420))
* Add tests (fixes [#243](https://github.com/xinminlabs/espree/issues/243)) ([36d84c7](https://github.com/xinminlabs/espree/commit/36d84c736d7890a95e4d4682cefb9c5e13931dc0))
* Added sudo false to Travis to build faster (fixes [#177](https://github.com/xinminlabs/espree/issues/177)) ([87c6b2f](https://github.com/xinminlabs/espree/commit/87c6b2f0dc439399b57f270b4eb4284cf841ea1f))
* Adding rc release script to package.json ([#383](https://github.com/xinminlabs/espree/issues/383)) ([d8224c4](https://github.com/xinminlabs/espree/commit/d8224c458fe4dfa139bb13a6559c889b047b7f2f))
* changelog update for 3.4.1 ([aea631f](https://github.com/xinminlabs/espree/commit/aea631ff138463cd8e318a73a316f8b3f49de9dd))
* changelog update for 3.4.2 ([5c9a692](https://github.com/xinminlabs/espree/commit/5c9a692fe9d0cc2c25b224dbc163b73ea577911e))
* changelog update for 3.4.3 ([4ecb96a](https://github.com/xinminlabs/espree/commit/4ecb96a6d7805d8ae0094f4fb6efb9f1bc3403ed))
* changelog update for 3.5.0 ([92ebe80](https://github.com/xinminlabs/espree/commit/92ebe80044240d0104aec07abd7c8d922aaaf052))
* changelog update for 3.5.1 ([748ce4f](https://github.com/xinminlabs/espree/commit/748ce4f566e93fce834b869a39ce5a8a66c4c5c9))
* changelog update for 3.5.2 ([c2a63e2](https://github.com/xinminlabs/espree/commit/c2a63e2d46d28bef9828562844d671f288ee172c))
* changelog update for 3.5.3 ([51400e9](https://github.com/xinminlabs/espree/commit/51400e9da9c2a99e148c3dcca19f62a95427f24e))
* changelog update for 3.5.4 ([ee991b7](https://github.com/xinminlabs/espree/commit/ee991b71349af9de8d34f61eac893ab06e0082fe))
* changelog update for 4.0.0 ([4742335](https://github.com/xinminlabs/espree/commit/4742335e475daa8f40a5418f8434485a86435c0e))
* changelog update for 4.0.0-alpha.0 ([f151028](https://github.com/xinminlabs/espree/commit/f151028b102cca407fe55ecb5117478ec3c94aa6))
* changelog update for 4.0.0-alpha.1 ([9a83504](https://github.com/xinminlabs/espree/commit/9a8350492171bf344cb63645cd30e6001a9f020d))
* changelog update for 4.0.0-rc.0 ([1ece96c](https://github.com/xinminlabs/espree/commit/1ece96cc9ae7fe2cfcfe405f881866c394f264c3))
* changelog update for 4.1.0 ([a67c1c9](https://github.com/xinminlabs/espree/commit/a67c1c931e00051dc3b5f38e34a4ff114841c8f4))
* changelog update for 5.0.0 ([b3ca44e](https://github.com/xinminlabs/espree/commit/b3ca44e1f750417aec040ad3e1d23174197a46bb))
* changelog update for 5.0.1 ([5e3f123](https://github.com/xinminlabs/espree/commit/5e3f12334f3e0c5fb5ede2edb641d2166a1c0e57))
* changelog update for 6.0.0 ([1974824](https://github.com/xinminlabs/espree/commit/19748245991be7d5165683ae5a489b3e89768211))
* changelog update for 6.0.0-alpha.0 ([4d17109](https://github.com/xinminlabs/espree/commit/4d1710981889d1761f1280beabb7a56016cf720a))
* changelog update for 6.1.0 ([a11ad1b](https://github.com/xinminlabs/espree/commit/a11ad1bfbf2d42a60c967098af9a9288fc7c0348))
* changelog update for 6.1.1 ([e49e746](https://github.com/xinminlabs/espree/commit/e49e746b6b2bc3b260ea13082175cf3fa271ac66))
* changelog update for 6.1.2 ([c2895aa](https://github.com/xinminlabs/espree/commit/c2895aa820b566ebe67bc45d007d38bdb4e2f938))
* changelog update for 6.2.0 ([105943b](https://github.com/xinminlabs/espree/commit/105943b18cdadfdcd09c719ffcb9955467f99367))
* changelog update for 6.2.1 ([1e2752c](https://github.com/xinminlabs/espree/commit/1e2752cdb2963f7f5ac242c7ac15a6f9e8d41c53))
* changelog update for 7.0.0 ([ae7ccbc](https://github.com/xinminlabs/espree/commit/ae7ccbc3a78fc9d2609e4b6161aded7c7027e17b))
* changelog update for 7.1.0 ([647eb13](https://github.com/xinminlabs/espree/commit/647eb136e5ca8f94612397d19eb2677fb8d2959e))
* changelog update for 7.2.0 ([4daabdc](https://github.com/xinminlabs/espree/commit/4daabdc03d06f686627cbb111983c369ab5c87f1))
* changelog update for 7.3.0 ([b78a36a](https://github.com/xinminlabs/espree/commit/b78a36a9e01d1df601cf954e2851fd981ef15a82))
* changelog update for 7.3.1 ([b4cabce](https://github.com/xinminlabs/espree/commit/b4cabceb8b38341efc4a37bc51bf42c5946d20ff))
* changelog update for 8.0.0 ([e584ef4](https://github.com/xinminlabs/espree/commit/e584ef422db80bc63ae4e73674246197751584e6))
* changelog update for 8.0.0-beta.0 ([997956b](https://github.com/xinminlabs/espree/commit/997956bfac74195127ebc2bfd54e42fe8b4184b4))
* changelog update for 8.0.0-beta.1 ([c8976d6](https://github.com/xinminlabs/espree/commit/c8976d66ba8c7a711d0150026c64d839ea1cd17b))
* changelog update for 9.0.0 ([a391887](https://github.com/xinminlabs/espree/commit/a391887c00ffbc860125b60563a69722fa67dadf))
* changelog update for 9.1.0 ([6298038](https://github.com/xinminlabs/espree/commit/6298038c8bccecbd34d84483170dbfadc5ef051e))
* changelog update for 9.2.0 ([2c30f94](https://github.com/xinminlabs/espree/commit/2c30f9418360ed97e9fe0f5c4651198613be52de))
* changelog update for 9.3.0 ([e8a56d9](https://github.com/xinminlabs/espree/commit/e8a56d9625bd125d20b576d691e7e71f675d502a))
* changelog update for 9.3.1 ([be29eb9](https://github.com/xinminlabs/espree/commit/be29eb90402490b276b5596fef278550e4dd0252))
* changelog update for 9.3.2 ([3c8ccc1](https://github.com/xinminlabs/espree/commit/3c8ccc1bab3cd108f525a8d84ebe7a1721bd7f29))
* changelog update for 9.3.3 ([4a780be](https://github.com/xinminlabs/espree/commit/4a780be0c810b4fa787d74ee4c0f272b351161ba))
* changelog update for 9.4.0 ([d694392](https://github.com/xinminlabs/espree/commit/d694392148061e79fbd89b39feaf0a9495d506f8))
* changelog update for 9.4.1 ([7eb1d22](https://github.com/xinminlabs/espree/commit/7eb1d22dfff2845522777eba150d569067c476d9))
* changelog update for 9.5.0 ([01160b0](https://github.com/xinminlabs/espree/commit/01160b0cb70def7fc0612d223f05273c13ea5127))
* changelog update for 9.5.1 ([7de61a1](https://github.com/xinminlabs/espree/commit/7de61a17df1b438310c2dda3d66be19077d51747))
* Fix package.json dependencies ([02b5284](https://github.com/xinminlabs/espree/commit/02b5284d35db127a47431630315f967cc9be7033))
* fix typos in package.json release scripts ([#375](https://github.com/xinminlabs/espree/issues/375)) ([95fa890](https://github.com/xinminlabs/espree/commit/95fa8901f07c2def60a2b2279a049fb7c8e9cdaa))
* Lock acorn to v4.0.4 ([#314](https://github.com/xinminlabs/espree/issues/314)) ([f55fa51](https://github.com/xinminlabs/espree/commit/f55fa51c6e50c296c15cbf1627dc8b8b2e0cdcd3))
* package.json and changelog update for 3.1.7 ([0687c1f](https://github.com/xinminlabs/espree/commit/0687c1fe1df4590ad79a453734d9a5729842e97f))
* package.json and changelog update for 3.2.0 ([e3360df](https://github.com/xinminlabs/espree/commit/e3360df0e9640db9a900b0ea64e3938dfd8fb6a8))
* package.json and changelog update for 3.3.0 ([b080efb](https://github.com/xinminlabs/espree/commit/b080efbfeeb71d82a71c66647dacb8de84486150))
* package.json and changelog update for 3.3.1 ([5f7bffc](https://github.com/xinminlabs/espree/commit/5f7bffcff82a4429141e8edf9a6e00cbf498d9f9))
* package.json and changelog update for 3.3.2 ([3dd64a2](https://github.com/xinminlabs/espree/commit/3dd64a21d4c2de75d84551167e9e6954db47e985))
* package.json and changelog update for 3.4.0 ([24e8221](https://github.com/xinminlabs/espree/commit/24e8221c1d5be412e84f771762480de2f4f20b64))
* remove browserify script ([#466](https://github.com/xinminlabs/espree/issues/466)) ([1a8ec00](https://github.com/xinminlabs/espree/commit/1a8ec00df416f08381152a9427378bd4bc1bec56))
* replace optimist with a simple native method ([55184a2](https://github.com/xinminlabs/espree/commit/55184a23d4e221f5fc1da3167df227a72313d390))
* Switch to eslint-release ([34d195b](https://github.com/xinminlabs/espree/commit/34d195bc287fbce63b42212752e33556e5356662))
* Update branch reference in CI ([#479](https://github.com/xinminlabs/espree/issues/479)) ([5dd3dee](https://github.com/xinminlabs/espree/commit/5dd3dee83616838451adad7183dd3dd8499a7335))
* Update release script ([0973cda](https://github.com/xinminlabs/espree/commit/0973cda919805336f4849d890ffc30954d87a89b))
* Update release tool ([5a37f80](https://github.com/xinminlabs/espree/commit/5a37f808d880f601fd00b9f2852a58abe99d63de))
* Update scripts for release (fixes [#475](https://github.com/xinminlabs/espree/issues/475)) ([#478](https://github.com/xinminlabs/espree/issues/478)) ([8209e4e](https://github.com/xinminlabs/espree/commit/8209e4e4a3302c1b205b248fc3efc264f1411769))
* upgrade eslint-release to v3.2.0 to support conventional commits ([#517](https://github.com/xinminlabs/espree/issues/517)) ([c0a8aa2](https://github.com/xinminlabs/espree/commit/c0a8aa2cbe5e683dfb416d2cfb3522906b15ba44))


### Chores

* add .npmrc ([#359](https://github.com/xinminlabs/espree/issues/359)) ([06c35c9](https://github.com/xinminlabs/espree/commit/06c35c90014f6e71edede161ab567e563307b446))
* Add `lint-staged` ([#565](https://github.com/xinminlabs/espree/issues/565)) ([5c85ea8](https://github.com/xinminlabs/espree/commit/5c85ea8a20d505342e48af456108e96edd8e20da))
* add `npm install` step to release-please workflow ([#573](https://github.com/xinminlabs/espree/issues/573)) ([d8900c1](https://github.com/xinminlabs/espree/commit/d8900c1598358dec85708ef5373fce4eafa5af1c))
* add class static blocks tests ([#515](https://github.com/xinminlabs/espree/issues/515)) ([93b24dd](https://github.com/xinminlabs/espree/commit/93b24dd1817e0678012a8841f70ad8370f64baae))
* Add jQuery Foundation copyright ([10709f0](https://github.com/xinminlabs/espree/commit/10709f08ab1c727edb1fe992b6ecf041cfd7d21b))
* add LICENSE file for tests ([#539](https://github.com/xinminlabs/espree/issues/539)) ([770b577](https://github.com/xinminlabs/espree/commit/770b5778a94676fed65b545299d4ace0512859af))
* add node v19 ([#558](https://github.com/xinminlabs/espree/issues/558)) ([ecb6cde](https://github.com/xinminlabs/espree/commit/ecb6cded6619cf57ce9945793b179323cfdc61f0))
* Add PRs to triage project ([#580](https://github.com/xinminlabs/espree/issues/580)) ([086555e](https://github.com/xinminlabs/espree/commit/086555ed960bd9cdbe9818cf962eaa1f5f32b737))
* Add test for valid non-string input ([#463](https://github.com/xinminlabs/espree/issues/463)) ([3b4ca9e](https://github.com/xinminlabs/espree/commit/3b4ca9e3141514ffac93bb7fef6c1329370df310))
* Add tests and comments (refs [#349](https://github.com/xinminlabs/espree/issues/349)) ([#487](https://github.com/xinminlabs/espree/issues/487)) ([34e1ab9](https://github.com/xinminlabs/espree/commit/34e1ab92abb5685aad859daac8d1edff816b7784))
* Add tests for ecmaVersion default value ([#460](https://github.com/xinminlabs/espree/issues/460)) ([0e09d9a](https://github.com/xinminlabs/espree/commit/0e09d9a4f213cb87073a6a87cb7d6317b77d1a23))
* Add triage action ([#560](https://github.com/xinminlabs/espree/issues/560)) ([5a70a0b](https://github.com/xinminlabs/espree/commit/5a70a0b361af7b8f04371a5b134c610c2fd9dc0f))
* added fixlint in Makefile.js ([#440](https://github.com/xinminlabs/espree/issues/440)) ([ad0543c](https://github.com/xinminlabs/espree/commit/ad0543c8b9f6981857ebebf23a37589a656e61a6))
* added lockfiles to .gitignore ([#438](https://github.com/xinminlabs/espree/issues/438)) ([99707f3](https://github.com/xinminlabs/espree/commit/99707f3f9d337ca719dce5720106f98b65bba7b1))
* added tests for options normalize ([#439](https://github.com/xinminlabs/espree/issues/439)) ([9a4cff3](https://github.com/xinminlabs/espree/commit/9a4cff3626d50a88428ca1b66610a2bdedd774dd))
* Adding .gitattributes file ([#366](https://github.com/xinminlabs/espree/issues/366)) ([cea4823](https://github.com/xinminlabs/espree/commit/cea4823b4e1f6fe3a1efba470f7dd8e076f97383))
* fix incorrect comment ([#491](https://github.com/xinminlabs/espree/issues/491)) ([864a73e](https://github.com/xinminlabs/espree/commit/864a73e05c00c90d517aa58d777713db643b7335))
* fix tests for Node 6+ ([#315](https://github.com/xinminlabs/espree/issues/315)) ([a3442b5](https://github.com/xinminlabs/espree/commit/a3442b5949dd249e1a81ce4e014ca5e0f17f732c))
* Fix/remove tools (fixes [#471](https://github.com/xinminlabs/espree/issues/471)) ([#476](https://github.com/xinminlabs/espree/issues/476)) ([651e204](https://github.com/xinminlabs/espree/commit/651e204f5dcbf67b31c3af2bac60d9aed53a1fc7))
* generate provenance statements when release ([#579](https://github.com/xinminlabs/espree/issues/579)) ([c1ef82c](https://github.com/xinminlabs/espree/commit/c1ef82c8671bca18f13911ff5c6ae40b40b72c87))
* Improve readability of `Program` position fix part ([#493](https://github.com/xinminlabs/espree/issues/493)) ([6ffd604](https://github.com/xinminlabs/espree/commit/6ffd604e1cf5874327dc628181c2394429d88d3c))
* lint tool files, add editorconfig, update devDeps. ([#545](https://github.com/xinminlabs/espree/issues/545)) ([e5982ef](https://github.com/xinminlabs/espree/commit/e5982ef11cc546826fc76467c93dbb33e981550c))
* move to GitHub Actions ([#449](https://github.com/xinminlabs/espree/issues/449)) ([4ba3eef](https://github.com/xinminlabs/espree/commit/4ba3eefdc4b32784565822b34f11977e99ca1a19))
* Refactor `TemplateElement` range fix ([#489](https://github.com/xinminlabs/espree/issues/489)) ([4c1f17d](https://github.com/xinminlabs/espree/commit/4c1f17ddb49dc2100fdb449462be11c3d03ba6c7))
* refactoring rest/spread properties ([#361](https://github.com/xinminlabs/espree/issues/361)) ([b2016cb](https://github.com/xinminlabs/espree/commit/b2016cb08f2048e0c72ac32450811fa4ac672a96))
* release 10.0.0 ([#581](https://github.com/xinminlabs/espree/issues/581)) ([8d6caaf](https://github.com/xinminlabs/espree/commit/8d6caafc69e15cf81d7ce58f5223a826aaf012d3))
* release 10.0.1 ([#596](https://github.com/xinminlabs/espree/issues/596)) ([5b82b84](https://github.com/xinminlabs/espree/commit/5b82b84a7d096cab68ebfc0e79eb0b87c2a58807))
* release 9.5.2 ([#572](https://github.com/xinminlabs/espree/issues/572)) ([114dafb](https://github.com/xinminlabs/espree/commit/114dafb6c19772eb20571cb7b5ba4cddbd273607))
* release 9.6.0 ([#576](https://github.com/xinminlabs/espree/issues/576)) ([8f49ade](https://github.com/xinminlabs/espree/commit/8f49ade3f245a6a8ae495750086cc572ed7afd63))
* release 9.6.1 ([#578](https://github.com/xinminlabs/espree/issues/578)) ([91ea350](https://github.com/xinminlabs/espree/commit/91ea3503112f380fba8eb2fb4cbeb7c6ebb71899))
* remove --legacy-peer-deps for Node 15 ([#485](https://github.com/xinminlabs/espree/issues/485)) ([e86f386](https://github.com/xinminlabs/espree/commit/e86f386a8ac959f13123d0f02d3f65a2b6f5f42c))
* Remove add-to-triage ([#583](https://github.com/xinminlabs/espree/issues/583)) ([3907385](https://github.com/xinminlabs/espree/commit/39073850d82db9f66af5c21017fdf2c250f9b419))
* Remove jQuery copyright from header of each file ([25c27fb](https://github.com/xinminlabs/espree/commit/25c27fb8d66f1f8f8ea96405a8b1d6165a7e4454))
* remove Object.assign polyfill ([#382](https://github.com/xinminlabs/espree/issues/382)) ([8cb3ceb](https://github.com/xinminlabs/espree/commit/8cb3ceba19eaa131348d0188a8bd0cc154ac3b97))
* Remove obsolete lib/visitor-keys.js ([#509](https://github.com/xinminlabs/espree/issues/509)) ([bf57077](https://github.com/xinminlabs/espree/commit/bf57077e02dd61f82ab533d6bb0c160e2dfe40b8))
* remove unused `devDependencies` ([#540](https://github.com/xinminlabs/espree/issues/540)) ([b578a66](https://github.com/xinminlabs/espree/commit/b578a66991985d96d5e6ee4f388c4356ad0b3594))
* rm devdep leche (fixes [#480](https://github.com/xinminlabs/espree/issues/480)) ([#482](https://github.com/xinminlabs/espree/issues/482)) ([b8d35ed](https://github.com/xinminlabs/espree/commit/b8d35ed9f00bf403670ed7544b40ac7207649101))
* run tests in Node.js 21 ([#585](https://github.com/xinminlabs/espree/issues/585)) ([1584ddb](https://github.com/xinminlabs/espree/commit/1584ddb00f0b4e3ada764ac86ae20e1480003de3))
* run tests on Node.js v20 ([#571](https://github.com/xinminlabs/espree/issues/571)) ([adf478e](https://github.com/xinminlabs/espree/commit/adf478e20d5db2b4607bc11ceef3363b7c7dfffb))
* set up release-please ([#569](https://github.com/xinminlabs/espree/issues/569)) ([abda10f](https://github.com/xinminlabs/espree/commit/abda10f71c9486e84c9a06923b57801eaa839516))
* standardize npm script names ([#582](https://github.com/xinminlabs/espree/issues/582)) ([b0767ef](https://github.com/xinminlabs/espree/commit/b0767ef7ba6979a1005c93c49c41aff1af483e07))
* strict mode enforced in modules (refs [#72](https://github.com/xinminlabs/espree/issues/72)) ([472ad3e](https://github.com/xinminlabs/espree/commit/472ad3e2692d04b7dfc586b7303ac37064d4a692))
* switch from nyc to c8 for ESM coverage ([#534](https://github.com/xinminlabs/espree/issues/534)) ([ea0cf6a](https://github.com/xinminlabs/espree/commit/ea0cf6a7f0ab68ff1ff70bcfad8a10c6bd740da5))
* switch to eslint flat config ([#577](https://github.com/xinminlabs/espree/issues/577)) ([408eabd](https://github.com/xinminlabs/espree/commit/408eabd6eeae0dbcf5aa1791499fc82e391d8797))
* Test on Node 15.x ([#468](https://github.com/xinminlabs/espree/issues/468)) ([2080ce6](https://github.com/xinminlabs/espree/commit/2080ce6cc8bef3057696967e518c87f749da6533))
* update github actions ([#552](https://github.com/xinminlabs/espree/issues/552)) ([bd3b5c6](https://github.com/xinminlabs/espree/commit/bd3b5c66db5569efdf1446ecf1dfd396e4b5689c))
* update linting config ([#406](https://github.com/xinminlabs/espree/issues/406)) ([35623ee](https://github.com/xinminlabs/espree/commit/35623ee07289c9199eef8b735c97cb3d3d08d5b8))
* update package.json ([#550](https://github.com/xinminlabs/espree/issues/550)) ([45fec88](https://github.com/xinminlabs/espree/commit/45fec887c310538ea03b4f758db5fdddd0a4687f))
* upgrade acorn@5.2 (fixes [#358](https://github.com/xinminlabs/espree/issues/358)) ([#360](https://github.com/xinminlabs/espree/issues/360)) ([59c9d06](https://github.com/xinminlabs/espree/commit/59c9d0635115d6b8d5037e03fa27d6ae20f5985a))
* upgrade eslint-visitor-keys@3.2.0 ([#533](https://github.com/xinminlabs/espree/issues/533)) ([9fbe22a](https://github.com/xinminlabs/espree/commit/9fbe22a1297e42dc654520c23acd167810686c41))
* upgrade eslint-visitor-keys@3.4.0 ([#568](https://github.com/xinminlabs/espree/issues/568)) ([91d48e9](https://github.com/xinminlabs/espree/commit/91d48e96a5f1173e7df4c3df15b565598aab7b41))
* upgrade eslint-visitor-keys@3.4.1 ([#574](https://github.com/xinminlabs/espree/issues/574)) ([8e73f11](https://github.com/xinminlabs/espree/commit/8e73f113e019e9a62fd6076c565e9fd4f7f4ff52))
* upgrade eslint-visitor-keys@4.0.0 ([#595](https://github.com/xinminlabs/espree/issues/595)) ([6254a91](https://github.com/xinminlabs/espree/commit/6254a915ac1025e8371a340067d6aba771fe4b11))
* Upgrade to eslint-visitor-keys@3.3.0 ([#535](https://github.com/xinminlabs/espree/issues/535)) ([37f2184](https://github.com/xinminlabs/espree/commit/37f2184f1d7b0097ee7af1a011c0e61500c0d669))
* use actions/setup-node@v2 ([#510](https://github.com/xinminlabs/espree/issues/510)) ([63bd0bc](https://github.com/xinminlabs/espree/commit/63bd0bc46adfbcd3a71d4cc222aa3923b76ebcf2))
* use eslint-config-eslint@9.0.0 ([#584](https://github.com/xinminlabs/espree/issues/584)) ([ec949bc](https://github.com/xinminlabs/espree/commit/ec949bcf381d33377d0b05cecd080e8a3a01b5f3))
* use LTS node version in lint job ([#561](https://github.com/xinminlabs/espree/issues/561)) ([fe89a66](https://github.com/xinminlabs/espree/commit/fe89a6677dbf3c7ce4df3b58c1156eac73b792a4))
* use node `v16` ([#524](https://github.com/xinminlabs/espree/issues/524)) ([1c4a04d](https://github.com/xinminlabs/espree/commit/1c4a04daededd8402723cfd092f77e510fcf5b57))
* use node v16 for `macOS` and `windows` jobs ([#527](https://github.com/xinminlabs/espree/issues/527)) ([1b72d7a](https://github.com/xinminlabs/espree/commit/1b72d7a7e774356dd7119f2239319651d91c37ef))

## [10.0.1](https://github.com/eslint/espree/compare/v10.0.0...v10.0.1) (2024-02-09)


### Chores

* upgrade eslint-visitor-keys@4.0.0 ([#595](https://github.com/eslint/espree/issues/595)) ([6254a91](https://github.com/eslint/espree/commit/6254a915ac1025e8371a340067d6aba771fe4b11))

## [10.0.0](https://github.com/eslint/espree/compare/v9.6.1...v10.0.0) (2024-01-25)


### ⚠ BREAKING CHANGES

* Require Node.js ^18.18.0 || ^20.9.0 || >=21.1.0 ([#589](https://github.com/eslint/espree/issues/589))

### Features

* Require Node.js ^18.18.0 || ^20.9.0 || &gt;=21.1.0 ([#589](https://github.com/eslint/espree/issues/589)) ([e79cfa4](https://github.com/eslint/espree/commit/e79cfa490aa2d23c7d4deda0e99f2190e508a638))


### Bug Fixes

* upgrade acorn v8.11.3 ([#590](https://github.com/eslint/espree/issues/590)) ([6d30382](https://github.com/eslint/espree/commit/6d303829686dd1e3a425438e816025d7193ec915))


### Chores

* Add PRs to triage project ([#580](https://github.com/eslint/espree/issues/580)) ([086555e](https://github.com/eslint/espree/commit/086555ed960bd9cdbe9818cf962eaa1f5f32b737))
* Remove add-to-triage ([#583](https://github.com/eslint/espree/issues/583)) ([3907385](https://github.com/eslint/espree/commit/39073850d82db9f66af5c21017fdf2c250f9b419))
* run tests in Node.js 21 ([#585](https://github.com/eslint/espree/issues/585)) ([1584ddb](https://github.com/eslint/espree/commit/1584ddb00f0b4e3ada764ac86ae20e1480003de3))
* standardize npm script names ([#582](https://github.com/eslint/espree/issues/582)) ([b0767ef](https://github.com/eslint/espree/commit/b0767ef7ba6979a1005c93c49c41aff1af483e07))
* use eslint-config-eslint@9.0.0 ([#584](https://github.com/eslint/espree/issues/584)) ([ec949bc](https://github.com/eslint/espree/commit/ec949bcf381d33377d0b05cecd080e8a3a01b5f3))

## [9.6.1](https://github.com/eslint/espree/compare/v9.6.0...v9.6.1) (2023-07-14)


### Chores

* generate provenance statements when release ([#579](https://github.com/eslint/espree/issues/579)) ([c1ef82c](https://github.com/eslint/espree/commit/c1ef82c8671bca18f13911ff5c6ae40b40b72c87))
* switch to eslint flat config ([#577](https://github.com/eslint/espree/issues/577)) ([408eabd](https://github.com/eslint/espree/commit/408eabd6eeae0dbcf5aa1791499fc82e391d8797))

## [9.6.0](https://github.com/eslint/espree/compare/v9.5.2...v9.6.0) (2023-06-19)


### Features

* Support ES2024 and regexp v flag ([#575](https://github.com/eslint/espree/issues/575)) ([4cfc062](https://github.com/eslint/espree/commit/4cfc0626c534377601d48e8cad38976da6b85964))

## [9.5.2](https://github.com/eslint/espree/compare/v9.5.1...v9.5.2) (2023-05-05)


### Chores

* add `npm install` step to release-please workflow ([#573](https://github.com/eslint/espree/issues/573)) ([d8900c1](https://github.com/eslint/espree/commit/d8900c1598358dec85708ef5373fce4eafa5af1c))
* run tests on Node.js v20 ([#571](https://github.com/eslint/espree/issues/571)) ([adf478e](https://github.com/eslint/espree/commit/adf478e20d5db2b4607bc11ceef3363b7c7dfffb))
* set up release-please ([#569](https://github.com/eslint/espree/issues/569)) ([abda10f](https://github.com/eslint/espree/commit/abda10f71c9486e84c9a06923b57801eaa839516))
* upgrade eslint-visitor-keys@3.4.1 ([#574](https://github.com/eslint/espree/issues/574)) ([8e73f11](https://github.com/eslint/espree/commit/8e73f113e019e9a62fd6076c565e9fd4f7f4ff52))

v9.5.1 - March 28, 2023

* [`91d48e9`](https://github.com/eslint/espree/commit/91d48e96a5f1173e7df4c3df15b565598aab7b41) chore: upgrade eslint-visitor-keys@3.4.0 (#568) (Milos Djermanovic)
* [`37f6b17`](https://github.com/eslint/espree/commit/37f6b17376efc2e93441ef3dc28d347918c475f0) fix: remove useless sourcemap url (fixes #566) (#567) (余腾靖)
* [`5c85ea8`](https://github.com/eslint/espree/commit/5c85ea8a20d505342e48af456108e96edd8e20da) chore: Add `lint-staged` (#565) (coderaiser)

v9.5.0 - March 10, 2023

* [`4368788`](https://github.com/eslint/espree/commit/43687882d30855033ec4db0a11514aa85c0dd8d0) feat: Add parser name (#562) (Nicholas C. Zakas)
* [`fe89a66`](https://github.com/eslint/espree/commit/fe89a6677dbf3c7ce4df3b58c1156eac73b792a4) ci: use LTS node version in lint job (#561) (Nitin Kumar)
* [`5a70a0b`](https://github.com/eslint/espree/commit/5a70a0b361af7b8f04371a5b134c610c2fd9dc0f) chore: Add triage action (#560) (Nicholas C. Zakas)

v9.4.1 - November 6, 2022

* [`ecb6cde`](https://github.com/eslint/espree/commit/ecb6cded6619cf57ce9945793b179323cfdc61f0) ci: add node v19 (#558) (Koichi ITO)
* [`30f5f2f`](https://github.com/eslint/espree/commit/30f5f2fe258fc32bb4d5b4b3bbf4d6aef13b6d1d) docs: update README for ECMAScript 2023 (#557) (Sosuke Suzuki)

v9.4.0 - August 26, 2022

* [`411d697`](https://github.com/eslint/espree/commit/411d697af3e65c92c13921bfb7baa7aad60242eb) feat: Support ES2023 and hashbangs (#556) (Brandon Mills)

v9.3.3 - July 31, 2022

* [`b1eac6d`](https://github.com/eslint/espree/commit/b1eac6d9687b2cb48dd28e8c11626afde22fa6cf) fix: don't recognize directives in ES3, allow parenthesized rest target (#554) (Milos Djermanovic)
* [`bd3b5c6`](https://github.com/eslint/espree/commit/bd3b5c66db5569efdf1446ecf1dfd396e4b5689c) ci: update github actions (#552) (Amaresh  S M)
* [`45fec88`](https://github.com/eslint/espree/commit/45fec887c310538ea03b4f758db5fdddd0a4687f) chore: update package.json (#550) (Deepshika S)

v9.3.2 - May 6, 2022

* [`6c718af`](https://github.com/eslint/espree/commit/6c718af090c1b5dd25d74a2ecfc65fbee0c00716) fix: "use strict" should not trigger strict mode in es3. (#547) (唯然)
* [`e5982ef`](https://github.com/eslint/espree/commit/e5982ef11cc546826fc76467c93dbb33e981550c) chore: lint tool files, add editorconfig, update devDeps. (#545) (Brett Zamir)
* [`75f65eb`](https://github.com/eslint/espree/commit/75f65eb2915438abd3ebd91dd62431456502e1db) build: add node v18 (#546) (唯然)
* [`b578a66`](https://github.com/eslint/espree/commit/b578a66991985d96d5e6ee4f388c4356ad0b3594) chore: remove unused `devDependencies` (#540) (Nitin Kumar)
* [`770b577`](https://github.com/eslint/espree/commit/770b5778a94676fed65b545299d4ace0512859af) chore: add LICENSE file for tests (#539) (Nitin Kumar)
* [`c915190`](https://github.com/eslint/espree/commit/c9151901be91b21a027478d2603862460fccf78f) docs: update Build Status badge (#536) (Milos Djermanovic)

v9.3.1 - February 11, 2022

* [`37f2184`](https://github.com/eslint/espree/commit/37f2184f1d7b0097ee7af1a011c0e61500c0d669) chore: Upgrade to eslint-visitor-keys@3.3.0 (#535) (Milos Djermanovic)
* [`64010de`](https://github.com/eslint/espree/commit/64010de254892c89376f56bd88aa07ef9382dda8) fix: Derive espree.Syntax from espree.VisitorKeys (#532) (Frank Weigel)
* [`ea0cf6a`](https://github.com/eslint/espree/commit/ea0cf6a7f0ab68ff1ff70bcfad8a10c6bd740da5) chore: switch from nyc to c8 for ESM coverage (#534) (Brett Zamir)
* [`9fbe22a`](https://github.com/eslint/espree/commit/9fbe22a1297e42dc654520c23acd167810686c41) chore: upgrade eslint-visitor-keys@3.2.0 (#533) (Milos Djermanovic)

v9.3.0 - December 31, 2021

* [`8655f3d`](https://github.com/eslint/espree/commit/8655f3d4d442da3b170ddbf2a84d29dfc41ba072) feat: support arbitrary module namespace names (#528) (Milos Djermanovic)
* [`1b72d7a`](https://github.com/eslint/espree/commit/1b72d7a7e774356dd7119f2239319651d91c37ef) ci: use node v16 for `macOS` and `windows` jobs (#527) (Nitin Kumar)

v9.2.0 - December 3, 2021

* [`1c4a04d`](https://github.com/eslint/espree/commit/1c4a04daededd8402723cfd092f77e510fcf5b57) ci: use node `v16` (#524) (Nitin Kumar)
* [`e807c20`](https://github.com/eslint/espree/commit/e807c2061f97fb0f8c8db3d2c5981731f9bf4a22) feat: add `allowReserved` for ES3 (#522) (Jordan Harband)
* [`34b9a6a`](https://github.com/eslint/espree/commit/34b9a6a08efe6089748c1a330c0e30b18eaf6785) docs: add private-in syntax (#523) (Milos Djermanovic)

v9.1.0 - November 20, 2021

* [`27713ac`](https://github.com/eslint/espree/commit/27713aca32c73347750f9033841f176f5cb83951) feat: Add sourceType:commonjs support (#520) (Nicholas C. Zakas)
* [`6839389`](https://github.com/eslint/espree/commit/6839389b9c67f0e6cbda00802867e7cf0ccd75eb) feat: support for private-in syntax (#521) (Yosuke Ota)
* [`fe07aae`](https://github.com/eslint/espree/commit/fe07aae683f3c09fe1cd0165a98e11339c22ab7c) feat: support class static blocks (#518) (Milos Djermanovic)
* [`c0a8aa2`](https://github.com/eslint/espree/commit/c0a8aa2cbe5e683dfb416d2cfb3522906b15ba44) build: upgrade eslint-release to v3.2.0 to support conventional commits (#517) (Milos Djermanovic)
* [`6be7bcb`](https://github.com/eslint/espree/commit/6be7bcb43f7bc10cc1f04f53ace3eb1e2d3f11bb) Build: add node v17 (#516) (唯然)
* [`93b24dd`](https://github.com/eslint/espree/commit/93b24dd1817e0678012a8841f70ad8370f64baae) Chore: add class static blocks tests (#515) (薛定谔的猫)

v9.0.0 - September 10, 2021

* [`7952c6f`](https://github.com/eslint/espree/commit/7952c6fd4155ce88ec726eac69cadd3bc5b3f3a5) Breaking: Disallow reserved words in ES3 (#513) (Nicholas C. Zakas)
* [`ee1d3ec`](https://github.com/eslint/espree/commit/ee1d3eca310cab1b1cf1563294434977d26358d4) Fix: 0x2028 and 0x2029 in string literals should increment line number (#514) (Milos Djermanovic)
* [`63bd0bc`](https://github.com/eslint/espree/commit/63bd0bc46adfbcd3a71d4cc222aa3923b76ebcf2) Chore: use actions/setup-node@v2 (#510) (薛定谔的猫)
* [`bf57077`](https://github.com/eslint/espree/commit/bf57077e02dd61f82ab533d6bb0c160e2dfe40b8) Chore: Remove obsolete lib/visitor-keys.js (#509) (Matthias Oßwald)

v8.0.0 - June 29, 2021

* [`c335413`](https://github.com/eslint/espree/commit/c33541363e1cf82346c9b59b253a11fd204d7116) Upgrade: eslint-visitor-keys@3.0.0 (#507) (Milos Djermanovic)
* [`e08c9d7`](https://github.com/eslint/espree/commit/e08c9d78745fcee03136b57f46d09e11cad70861) 8.0.0-beta.1 (ESLint Jenkins)
* [`c8976d6`](https://github.com/eslint/espree/commit/c8976d66ba8c7a711d0150026c64d839ea1cd17b) Build: changelog update for 8.0.0-beta.1 (ESLint Jenkins)
* [`e207bd7`](https://github.com/eslint/espree/commit/e207bd703e761d5565ee59d15253260ae8e90a79) Update: Support top-level await and regexp match indices (#505) (Nicholas C. Zakas)
* [`9eff2c7`](https://github.com/eslint/espree/commit/9eff2c7b8cb18f19504afd8a97cad51d6905dfcf) Update: reset default ecmaVersion to 5 (#506) (Nicholas C. Zakas)
* [`c8ca49a`](https://github.com/eslint/espree/commit/c8ca49a281eb74bb81e9bc3a60300011e8b29e8d) 8.0.0-beta.0 (ESLint Jenkins)
* [`997956b`](https://github.com/eslint/espree/commit/997956bfac74195127ebc2bfd54e42fe8b4184b4) Build: changelog update for 8.0.0-beta.0 (ESLint Jenkins)
* [`d017d38`](https://github.com/eslint/espree/commit/d017d38fc3a113a0a816aa9d21a60ea1850dbb4a) Breaking: drop node v10/13/v15 (fixes #501) (#502) (薛定谔的猫)
* [`e71162c`](https://github.com/eslint/espree/commit/e71162c0842f683ca71bc34b70142496681b3674) Update: add class fields (refs eslint/eslint#14343) (#486) (Toru Nagashima)
* [`b068cea`](https://github.com/eslint/espree/commit/b068cea907ef59fe5681f6acedd30b932d496e0a) Breaking: Implement 'ecmaVersion: latest' (fixes #495) (#499) (Nicholas C. Zakas)
* [`8294427`](https://github.com/eslint/espree/commit/82944270100e3108884f0fa96e691aa1eb82e5dd) Upgrade: eslint-release@3.1.2 (#494) (Milos Djermanovic)
* [`4c1f17d`](https://github.com/eslint/espree/commit/4c1f17ddb49dc2100fdb449462be11c3d03ba6c7) Chore: Refactor `TemplateElement` range fix (#489) (fisker Cheung)
* [`6ffd604`](https://github.com/eslint/espree/commit/6ffd604e1cf5874327dc628181c2394429d88d3c) Chore: Improve readability of `Program` position fix part (#493) (fisker Cheung)
* [`94508b7`](https://github.com/eslint/espree/commit/94508b75f140eafd1a978c48bcfae488907a53e1) Upgrade: acorn to 8.2.2 (fixes #472) (#492) (薛定谔的猫)
* [`864a73e`](https://github.com/eslint/espree/commit/864a73e05c00c90d517aa58d777713db643b7335) Chore: fix incorrect comment (#491) (薛定谔的猫)
* [`34e1ab9`](https://github.com/eslint/espree/commit/34e1ab92abb5685aad859daac8d1edff816b7784) Chore: Add tests and comments (refs #349) (#487) (Nicholas C. Zakas)
* [`dffb7aa`](https://github.com/eslint/espree/commit/dffb7aa72f2cd23d99e36e6c7c1a76c73ff08f16) Breaking: syncing start/end with range (fixes #349) (#461) (Anix)
* [`e86f386`](https://github.com/eslint/espree/commit/e86f386a8ac959f13123d0f02d3f65a2b6f5f42c) Chore: remove --legacy-peer-deps for Node 15 (#485) (Milos Djermanovic)
* [`ecaf510`](https://github.com/eslint/espree/commit/ecaf510e03f5864e546eb7f60728fbc488fc8543) Build: add node v16 (#481) (薛定谔的猫)
* [`b8d35ed`](https://github.com/eslint/espree/commit/b8d35ed9f00bf403670ed7544b40ac7207649101) Chore: rm devdep leche (fixes #480) (#482) (薛定谔的猫)
* [`651e204`](https://github.com/eslint/espree/commit/651e204f5dcbf67b31c3af2bac60d9aed53a1fc7) Chore: Fix/remove tools (fixes #471) (#476) (Nicholas C. Zakas)
* [`671c3aa`](https://github.com/eslint/espree/commit/671c3aa55bd9ece231f2f28417d557d264994107) Docs: Update README with ESM instructions (fixes #474) (#477) (Nicholas C. Zakas)
* [`8209e4e`](https://github.com/eslint/espree/commit/8209e4e4a3302c1b205b248fc3efc264f1411769) Build: Update scripts for release (fixes #475) (#478) (Nicholas C. Zakas)
* [`5dd3dee`](https://github.com/eslint/espree/commit/5dd3dee83616838451adad7183dd3dd8499a7335) Build: Update branch reference in CI (#479) (Nicholas C. Zakas)
* [`995d2a8`](https://github.com/eslint/espree/commit/995d2a87d44461754b691f820abb08c8f525087a) Breaking: acorn to 8.1.0 (fixes #470) (#473) (薛定谔的猫)
* [`8234c48`](https://github.com/eslint/espree/commit/8234c48496dd851ed2a39ce169e517e5927dbfe0) Breaking: provide ESM export (refs eslint/rfcs#72) (#469) (Mike Reinstein)
* [`2080ce6`](https://github.com/eslint/espree/commit/2080ce6cc8bef3057696967e518c87f749da6533) Chore: Test on Node 15.x (#468) (Milos Djermanovic)
* [`fc384a4`](https://github.com/eslint/espree/commit/fc384a4daf4e81c2c389a5cefb6062cbb0937ae4) Upgrade: eslint devDependencies (#467) (Milos Djermanovic)
* [`1a8ec00`](https://github.com/eslint/espree/commit/1a8ec00df416f08381152a9427378bd4bc1bec56) Build: remove browserify script (#466) (Milos Djermanovic)
* [`3b4ca9e`](https://github.com/eslint/espree/commit/3b4ca9e3141514ffac93bb7fef6c1329370df310) Chore: Add test for valid non-string input (#463) (stonegray)
* [`1b99259`](https://github.com/eslint/espree/commit/1b992595340fa28939d291cf2e7cf7571015b155) Upgrade: eslint-visitor-keys@2.0.0 (#462) (Milos Djermanovic)

v8.0.0-beta.1 - June 24, 2021

* [`e207bd7`](https://github.com/eslint/espree/commit/e207bd703e761d5565ee59d15253260ae8e90a79) Update: Support top-level await and regexp match indices (#505) (Nicholas C. Zakas)
* [`9eff2c7`](https://github.com/eslint/espree/commit/9eff2c7b8cb18f19504afd8a97cad51d6905dfcf) Update: reset default ecmaVersion to 5 (#506) (Nicholas C. Zakas)

v8.0.0-beta.0 - June 11, 2021

* [`d017d38`](https://github.com/eslint/espree/commit/d017d38fc3a113a0a816aa9d21a60ea1850dbb4a) Breaking: drop node v10/13/v15 (fixes #501) (#502) (薛定谔的猫)
* [`e71162c`](https://github.com/eslint/espree/commit/e71162c0842f683ca71bc34b70142496681b3674) Update: add class fields (refs eslint/eslint#14343) (#486) (Toru Nagashima)
* [`b068cea`](https://github.com/eslint/espree/commit/b068cea907ef59fe5681f6acedd30b932d496e0a) Breaking: Implement 'ecmaVersion: latest' (fixes #495) (#499) (Nicholas C. Zakas)
* [`8294427`](https://github.com/eslint/espree/commit/82944270100e3108884f0fa96e691aa1eb82e5dd) Upgrade: eslint-release@3.1.2 (#494) (Milos Djermanovic)
* [`4c1f17d`](https://github.com/eslint/espree/commit/4c1f17ddb49dc2100fdb449462be11c3d03ba6c7) Chore: Refactor `TemplateElement` range fix (#489) (fisker Cheung)
* [`6ffd604`](https://github.com/eslint/espree/commit/6ffd604e1cf5874327dc628181c2394429d88d3c) Chore: Improve readability of `Program` position fix part (#493) (fisker Cheung)
* [`94508b7`](https://github.com/eslint/espree/commit/94508b75f140eafd1a978c48bcfae488907a53e1) Upgrade: acorn to 8.2.2 (fixes #472) (#492) (薛定谔的猫)
* [`864a73e`](https://github.com/eslint/espree/commit/864a73e05c00c90d517aa58d777713db643b7335) Chore: fix incorrect comment (#491) (薛定谔的猫)
* [`34e1ab9`](https://github.com/eslint/espree/commit/34e1ab92abb5685aad859daac8d1edff816b7784) Chore: Add tests and comments (refs #349) (#487) (Nicholas C. Zakas)
* [`dffb7aa`](https://github.com/eslint/espree/commit/dffb7aa72f2cd23d99e36e6c7c1a76c73ff08f16) Breaking: syncing start/end with range (fixes #349) (#461) (Anix)
* [`e86f386`](https://github.com/eslint/espree/commit/e86f386a8ac959f13123d0f02d3f65a2b6f5f42c) Chore: remove --legacy-peer-deps for Node 15 (#485) (Milos Djermanovic)
* [`ecaf510`](https://github.com/eslint/espree/commit/ecaf510e03f5864e546eb7f60728fbc488fc8543) Build: add node v16 (#481) (薛定谔的猫)
* [`b8d35ed`](https://github.com/eslint/espree/commit/b8d35ed9f00bf403670ed7544b40ac7207649101) Chore: rm devdep leche (fixes #480) (#482) (薛定谔的猫)
* [`651e204`](https://github.com/eslint/espree/commit/651e204f5dcbf67b31c3af2bac60d9aed53a1fc7) Chore: Fix/remove tools (fixes #471) (#476) (Nicholas C. Zakas)
* [`671c3aa`](https://github.com/eslint/espree/commit/671c3aa55bd9ece231f2f28417d557d264994107) Docs: Update README with ESM instructions (fixes #474) (#477) (Nicholas C. Zakas)
* [`8209e4e`](https://github.com/eslint/espree/commit/8209e4e4a3302c1b205b248fc3efc264f1411769) Build: Update scripts for release (fixes #475) (#478) (Nicholas C. Zakas)
* [`5dd3dee`](https://github.com/eslint/espree/commit/5dd3dee83616838451adad7183dd3dd8499a7335) Build: Update branch reference in CI (#479) (Nicholas C. Zakas)
* [`995d2a8`](https://github.com/eslint/espree/commit/995d2a87d44461754b691f820abb08c8f525087a) Breaking: acorn to 8.1.0 (fixes #470) (#473) (薛定谔的猫)
* [`8234c48`](https://github.com/eslint/espree/commit/8234c48496dd851ed2a39ce169e517e5927dbfe0) Breaking: provide ESM export (refs eslint/rfcs#72) (#469) (Mike Reinstein)
* [`2080ce6`](https://github.com/eslint/espree/commit/2080ce6cc8bef3057696967e518c87f749da6533) Chore: Test on Node 15.x (#468) (Milos Djermanovic)
* [`fc384a4`](https://github.com/eslint/espree/commit/fc384a4daf4e81c2c389a5cefb6062cbb0937ae4) Upgrade: eslint devDependencies (#467) (Milos Djermanovic)
* [`1a8ec00`](https://github.com/eslint/espree/commit/1a8ec00df416f08381152a9427378bd4bc1bec56) Build: remove browserify script (#466) (Milos Djermanovic)
* [`3b4ca9e`](https://github.com/eslint/espree/commit/3b4ca9e3141514ffac93bb7fef6c1329370df310) Chore: Add test for valid non-string input (#463) (stonegray)
* [`1b99259`](https://github.com/eslint/espree/commit/1b992595340fa28939d291cf2e7cf7571015b155) Upgrade: eslint-visitor-keys@2.0.0 (#462) (Milos Djermanovic)

v7.3.1 - December 5, 2020

* [`fef6f4a`](https://github.com/eslint/espree/commit/fef6f4a2803d959304c6961527044bd9da39ac92) Upgrade: acorn-jsx@5.3.1 (#459) (Milos Djermanovic)
* [`0e09d9a`](https://github.com/eslint/espree/commit/0e09d9a4f213cb87073a6a87cb7d6317b77d1a23) Chore: Add tests for ecmaVersion default value (#460) (Milos Djermanovic)
* [`4c70052`](https://github.com/eslint/espree/commit/4c70052df0b0ba903602c1f838918cbc07ee5eca) Docs: Fix some minor typos in the READMEs (#455) (Noah Doersing)

v7.3.0 - August 22, 2020

* [`4ba3eef`](https://github.com/eslint/espree/commit/4ba3eefdc4b32784565822b34f11977e99ca1a19) Chore: move to GitHub Actions (#449) (Kai Cataldo)
* [`bd0a405`](https://github.com/eslint/espree/commit/bd0a405ffbe4962bcf5aa225ed3861a6a15cb827) Update: support logical assignment and numeric separators (#448) (Toru Nagashima)

v7.2.0 - July 17, 2020

* [`91c2d58`](https://github.com/eslint/espree/commit/91c2d5896889042058399cd64de4b218c5add0eb) Docs: Add security policy (#447) (Nicholas C. Zakas)
* [`872645c`](https://github.com/eslint/espree/commit/872645cea0bee08960b93c097f84153d44b44d7f) Update: support optional chaining (#446) (Toru Nagashima)
* [`0cc7800`](https://github.com/eslint/espree/commit/0cc78007c933564f32fd849bd8022992845c3ac1) Docs: Clean up LICENSE file (#445) (Nicholas C. Zakas)

v7.1.0 - June 4, 2020

* [`75e80bc`](https://github.com/eslint/espree/commit/75e80bc1b5a100f64b09b2c7bf47c5168417d890) Update: support `??` operator, `import.meta`, and `export * as ns` (#441) (Toru Nagashima)
* [`ad0543c`](https://github.com/eslint/espree/commit/ad0543c8b9f6981857ebebf23a37589a656e61a6) Chore: added fixlint in Makefile.js (#440) (Anix)

v7.0.0 - May 7, 2020

* [`8fe2efc`](https://github.com/eslint/espree/commit/8fe2efc00902e7f1680af00a6279e1aecb3c5b47) Breaking: drop Node v8 support (#429) (Kai Cataldo)
* [`6048bfe`](https://github.com/eslint/espree/commit/6048bfe3939fa7dc162c0b3c4b043bb410736b0b) Docs: documenting public API (fixes #431) (#442) (Anix)
* [`9a4cff3`](https://github.com/eslint/espree/commit/9a4cff3626d50a88428ca1b66610a2bdedd774dd) Chore: added tests for options normalize (#439) (Anix)
* [`99707f3`](https://github.com/eslint/espree/commit/99707f3f9d337ca719dce5720106f98b65bba7b1) Chore: added lockfiles to .gitignore (#438) (Anix)
* [`9b91bcc`](https://github.com/eslint/espree/commit/9b91bccacea15c75025a62bae828f83598aef5fe) Docs: new site for docs (#436) (Anix)

v6.2.1 - March 10, 2020

* [`d6d7480`](https://github.com/eslint/espree/commit/d6d7480e424960159007caea86f209f696138734) Upgrade: acorn 7.1.1, Regex DOS vuln (fixes #435) (#434) (James)

v6.2.0 - March 2, 2020

* [`ced1b68`](https://github.com/eslint/espree/commit/ced1b6810b991531e6d3788ebd5a322fc5c7d463) Update: update acorn-jsx and fix failing test (#432) (Kai Cataldo)
* [`acb8776`](https://github.com/eslint/espree/commit/acb8776d369abf9e02f79142879e9b1a4774f938) Update: add latestEcmaVersion & supportedEcmaVersions (#430) (Kai Cataldo)

v6.1.2 - October 20, 2019

* [`70c4970`](https://github.com/eslint/espree/commit/70c4970e5eba6f060e1e32a22d231647f2d0e0f8) Fix: misuse token types (fixes #393, refs eslint/eslint#11018) (#426) (Toru Nagashima)

v6.1.1 - August 23, 2019

* [`ba81546`](https://github.com/eslint/espree/commit/ba81546e8552ec0f779aae7e03668c334630484e) Upgrade: dev deps to latest (#424) (薛定谔的猫)
* [`bbe0119`](https://github.com/eslint/espree/commit/bbe01195fb57e24634d18825d39b820ed1767e95) Upgrade: acorn-jsx@5.0.2 (#423) (薛定谔的猫)
* [`c0635ba`](https://github.com/eslint/espree/commit/c0635bac4cd891cb612fb81655012e2579f4e2b1) Docs: update readme to mention ES2020 (#422) (Kai Cataldo)

v6.1.0 - August 18, 2019

* [`9870c55`](https://github.com/eslint/espree/commit/9870c553efd3eb1bd22b4b3bb5220896c5cb6933) Update: improve error messaging when validating ecmaVersion (#421) (Kai Cataldo)
* [`3f49224`](https://github.com/eslint/espree/commit/3f49224eb05f6b8cb1b996ce424a99c40978b389) Fix: tokenize the latest right curly brace (fixes #403) (#419) (finico)
* [`f5e58cc`](https://github.com/eslint/espree/commit/f5e58cc5e9030793baca3426366b8d7286ef5b89) Update: support bigint and dynamic import (#415) (Toru Nagashima)

v6.0.0 - June 21, 2019

* [`a988a36`](https://github.com/eslint/espree/commit/a988a36e436a1ab6c84005ba0adb6cf9c262c1ec) Build: add node 12 (#414) (薛定谔的猫)

v6.0.0-alpha.0 - April 12, 2019

* [`493d464`](https://github.com/eslint/espree/commit/493d464e1564aea0ea33000389771d42ddece2cb) Breaking: validate parser options (fixes #384) (#412) (薛定谔的猫)

v5.0.1 - February 15, 2019

* [`c40e2fc`](https://github.com/eslint/espree/commit/c40e2fcedf81ff06151e82bdf655d2d0d29e71b8) Upgrade: acorn@6.0.7 (#407) (Kai Cataldo)

v5.0.0 - December 5, 2018

* [`1bcd563`](https://github.com/eslint/espree/commit/1bcd563d4eb4b4032d2662cc5ccd3bfd841b39d7) Breaking: remove attachComment (#405) (Kai Cataldo)
* [`35623ee`](https://github.com/eslint/espree/commit/35623ee07289c9199eef8b735c97cb3d3d08d5b8) Chore: update linting config (#406) (Kai Cataldo)
* [`4b86a7d`](https://github.com/eslint/espree/commit/4b86a7dc7c447c11bb6530e46dc43428ce2bd372) Build: add node 11 (#400) (薛定谔的猫)
* [`7c278d6`](https://github.com/eslint/espree/commit/7c278d6acc6b5db86b803d0cd21b830deb6f569e) Fix: build failing due to incorrectly super() call (fixes #398) (#399) (薛定谔的猫)
* [`6ebc219`](https://github.com/eslint/espree/commit/6ebc21947166399a0b4918d4a1beb9d610650336) Upgrade: eslint & eslint-config-eslint (#387) (薛定谔的猫)

v4.1.0 - October 24, 2018

* 8eadb88 Upgrade: acorn 6, acorn-jsx 5, and istanbul (#391) (Toru Nagashima)
* 0f2edb8 Upgrade: eslint-release@1.0.0 (#392) (Teddy Katz)
* 560b6f7 Update: VisitorKeys depend on eslint-visitor-keys (#389) (othree)
* 6bf2ebf Docs: Fix some typos in the README (#386) (Hugo Locurcio)

v4.0.0 - June 21, 2018



v4.0.0-rc.0 - June 9, 2018

* d8224c4 Build: Adding rc release script to package.json (#383) (Kevin Partington)
* 4207773 Build: add node 10 (#381) (薛定谔的猫)
* cd9da7e Update: upgrade acorn to support two ES2019 syntax (#380) (Toru Nagashima)
* 8cb3ceb Chore: remove Object.assign polyfill (#382) (薛定谔的猫)

v4.0.0-alpha.1 - May 28, 2018

* 56c5a9c Fix: remove workarounds for acorn < 4 (#372) (Rouven Weßling)
* fd305e5 Upgrade: eslint-release to v0.11.1 (#376) (Teddy Katz)

v4.0.0-alpha.0 - March 30, 2018

* 95fa890 Build: fix typos in package.json release scripts (#375) (Teddy Katz)
* 6284e09 Breaking: remove experimentalObjectRestSpread option (#374) (Teddy Katz)
* 0df063f Breaking: require Node.js 6+, upgrade acorn-jsx@4.1.1 (fixes #345) (#371) (薛定谔的猫)
* 0252144 Upgrade: acorn 5.5.1 (#370) (Rouven Weßling)

v3.5.4 - March 4, 2018

* 706167b Upgrade: acorn 5.5.0 (#369) (Toru Nagashima)

v3.5.3 - February 2, 2018

* 70f9859 Upgrade: acorn 5.4.0 (#367) (Toru Nagashima)
* cea4823 Chore: Adding .gitattributes file (#366) (Kevin Partington)
* 4160aee Upgrade: acorn v5.3.0 (#365) (Toru Nagashima)

v3.5.2 - November 10, 2017

* 019b70a Fix: Remove blockBindings from docs (fixes #307, fixes #339) (#356) (Jan Pilzer)
* b2016cb Chore: refactoring rest/spread properties (#361) (Toru Nagashima)
* 59c9d06 Chore: upgrade acorn@5.2 (fixes #358) (#360) (Toru Nagashima)
* 06c35c9 Chore: add .npmrc (#359) (Toru Nagashima)

v3.5.1 - September 15, 2017

* 5eb1388 Fix: Fix parsing of async keyword-named object methods (#352) (#353) (Mark Banner)

v3.5.0 - August 5, 2017

* 4d442a1 Update: add initial support for ES2018 (#348) (Teddy Katz)
* d4bdcb6 Fix: Make template token objects adhere to token object structure (#343) (Ian Christian Myers)
* 9ac671a Upgrade: acorn to 5.1.1 (#347) (Teddy Katz)
* 16e1fec Docs: Specify default values of options (fixes #325) (#342) (Jan Pilzer)
* be85b8e Fix: async shorthand properties (fixes #340) (#341) (Toru Nagashima)

v3.4.3 - May 5, 2017

* 343590a Fix: add AwaitExpression to espree.Syntax (fixes #331) (#332) (Teddy Katz)

v3.4.2 - April 21, 2017

* c99e436 Upgrade: eslint to 2.13.1 (#328) (Teddy Katz)
* 628cf3a Fix: don't mutate user-provided configs (fixes #329) (#330) (Teddy Katz)

v3.4.1 - March 31, 2017

* a3ae0bd Upgrade: acorn to 5.0.1 (#327) (Teddy Katz)
* 15ef24f Docs: Add badges (#326) (Jan Pilzer)
* 652990a Fix: raise error for trailing commas after rest properties (fixes #310) (#323) (Teddy Katz)
* 9d86ba5 Upgrade: acorn to ^4.0.11 (#317) (Toru Nagashima)
* a3442b5 Chore: fix tests for Node 6+ (#315) (Teddy Katz)

v3.4.0 - February 2, 2017

* f55fa51 Build: Lock acorn to v4.0.4 (#314) (Kai Cataldo)
* 58f75be Fix:generic error for invalid ecmaVersion(fixes eslint#7405) (#303) (Scott Stern)
* d6b383d Docs: Update license copyright (Nicholas C. Zakas)
* e5df542 Update: To support year in ecmaVersion number (fixes #300) (#301) (Gyandeep Singh)

v3.3.2 - September 29, 2016

* 7d3e2fc Fix: reset `isAsync` flag for each property (fixes #298) (#299) (Toru Nagashima)

v3.3.1 - September 26, 2016

* 80abdce Fix: `}` token followed by template had been lost (fixes #293) (#294) (Toru Nagashima)
* 9810bab Fix: parsing error on `async` as property name. (#295) (Toru Nagashima)

v3.3.0 - September 20, 2016

* 92b04b1 Update: create-test script (fixes #291) (#292) (Jamund Ferguson)

v3.2.0 - September 16, 2016

* 5a37f80 Build: Update release tool (Nicholas C. Zakas)
* 9bbcad8 Update: Upgrade Acorn to support ES2017 (fixes #287) (#290) (Jamund Ferguson)
* 8d9767d Build: Add CI release scripts (Nicholas C. Zakas)

v3.1.7 - July 29, 2016

* 8f6cfbd Build: Add CI release (Nicholas C. Zakas)
* ff15922 Fix: Catch ES2016 invalid syntax (fixes #284) (#285) (Nicholas C. Zakas)

v3.1.6 - June 15, 2016

* a90edc2 Upgrade: acorn 3.2.0 (fixes #279) (#280) (Toru Nagashima)

v3.1.5 - May 27, 2016

* 7df2e4a Fix: Convert ~ and ! prefix tokens to esprima (fixes #274) (#276) (Daniel Tschinder)

v3.1.4 - April 21, 2016

* e044705 Fix: remove extra leading comments at node level (fixes #264) (Kai Cataldo)
* 25c27fb Chore: Remove jQuery copyright from header of each file (Kai Cataldo)
* 10709f0 Chore: Add jQuery Foundation copyright (Nicholas C. Zakas)
* d754b32 Upgrade: Acorn 3.1.0 (fixes #270) (Toru Nagashima)
* 3a90886 Docs: replace a dead link with the correct contributing guide URL (Shinnosuke Watanabe)
* 55184a2 Build: replace optimist with a simple native method (Shinnosuke Watanabe)
* c7e5a13 Fix: Disallow namespaces objects in JSX (fixes #261) (Kai Cataldo)
* 22290b9 Fix: Add test for leading comments (fixes #136) (Kai Cataldo)

v3.1.3 - March 18, 2016

* 98441cb Fix: Fix behavior of ignoring comments within previous nodes (refs #256) (Kai Cataldo)

v3.1.2 - March 14, 2016

* a2b23ca Fix: Ensure 'var let' works (fixes #149) (Nicholas C. Zakas)
* 5783282 Fix: Make obj.await work in modules (fixes #258) (Nicholas C. Zakas)
* d1b4929 Fix: leading comments added from previous node (fixes #256) (Kai Cataldo)

v3.1.1 - February 26, 2016

* 3614e81 Fix: exponentiation operator token (fixes #254) (Nicholas C. Zakas)

v3.1.0 - February 25, 2016

* da35d98 New: Support ecmaVersion 7 (fixes #246) (Nicholas C. Zakas)

v3.0.2 - February 19, 2016

* 0973cda Build: Update release script (Nicholas C. Zakas)
* 106000f Fix: use the plugins feature of acorn (fixes #250) (Toru Nagashima)
* 36d84c7 Build: Add tests (fixes #243) (Nicholas C. Zakas)

v3.0.1 - February 2, 2016

* ecfe4c8 Upgrade: eslint-config-eslint to 3.0.0 (Nicholas C. Zakas)
* ea6261e Fix: Object rest/spread in assign (fixes #247) (Nicholas C. Zakas)
* 7e57ee0 Docs: fix `options.comment` typo (xuezu)
* dd5863e Build: Add prerelease script (Nicholas C. Zakas)
* 0b409ee Upgrade: eslint-release to 0.2.0 (Nicholas C. Zakas)

v3.0.0 - January 20, 2016

* 5ff65f6 Upgrade: Change Esprima version to latest (Nicholas C. Zakas)
* a8badcc Upgrade: eslint-release to 0.1.4 (Nicholas C. Zakas)
* 34d195b Build: Switch to eslint-release (Nicholas C. Zakas)
* a0ddc30 Breaking: Remove binary scripts (Nicholas C. Zakas)
* 02b5284 Build: Fix package.json dependencies (Nicholas C. Zakas)
* b07696f Fix: tests for importing keywords (fixes #225) (Toru Nagashima)
* 2e2808a Build: Add node@5 to CI (fixes #237) (alberto)
* 445c685 Update: Unrecognized license format in package.json (fixes #234) (alberto)
* 61cb5ee Update: Remove duplicated acorn-jsx dep (fixes #232) (alberto)
* df5b71c Upgrade: eslint and eslint-config-eslint (fixes #231) (alberto)
* ef7a06d Fix: lastToken not reset between calls to parse (fixes #229) (alberto)
* cdf8407 New: ecmaFeatures.impliedStrict (fixes: #227) (Nick Evans)

v3.0.0-alpha-2 - December 9, 2015

* 3.0.0-alpha-2 (Nicholas C. Zakas)
* Breaking: move ecmaFeatures into ecmaVersion (fixes #222) (Nicholas C. Zakas)
* New: Export VisitorKeys (fixes #220) (Nicholas C. Zakas)

v3.0.0-alpha-1 - December 1, 2015

* 3.0.0-alpha-1 (Nicholas C. Zakas)
* Fix: parse unicode escapes in identifiers (fixes #181) (Nicholas C. Zakas)
* Fix: Ensur object rest works in destructed arg (fixes #213) (Nicholas C. Zakas)
* Breaking: Switch to Acorn (fixes #200) (Nicholas C. Zakas)
* Update: Add tokens to tests (fixes #203) (Nicholas C. Zakas)
* Docs: Update README (Nicholas C. Zakas)

v2.2.5 - September 15, 2015

* 2.2.5 (Nicholas C. Zakas)
* Fix: Ensure node type is correct for destructured (fixes #195) (Nicholas C. Zakas)

v2.2.4 - August 13, 2015

* 2.2.4 (Nicholas C. Zakas)
* Fix: newlines in arrow functions (fixes #172) (Jamund Ferguson)
* Fix: nested arrow function as default param (fixes #145) (Jamund Ferguson)
* Fix: Rest Params & Arrow Functions (fixes #187) (Jamund Ferguson)
* Fix: trailing commas in import/export (fixes #148) (Jamund Ferguson)
* Build: Added sudo false to Travis to build faster (fixes #177) (KahWee Teng)

v2.2.3 - July 22, 2015

* 2.2.3 (Nicholas C. Zakas)
* Fix: Incorrect error location (fixes #173) (Nicholas C. Zakas)

v2.2.2 - July 16, 2015

* 2.2.2 (Nicholas C. Zakas)
* 2.2.1 (Nicholas C. Zakas)
* Fix: Yield as identifier in arrow func args (fixes #165) (Nicholas C. Zakas)
* Fix: Allow AssignmentExpression in object spread (fixes #167) (Nicholas C. Zakas)

v2.2.1 - July 16, 2015

* 2.2.1 (Nicholas C. Zakas)

v2.2.0 - July 15, 2015

* 2.2.0 (Nicholas C. Zakas)
* New: Add experimental object rest/spread (fixes #163) (Nicholas C. Zakas)
* Fix: npm browserify (fixes #156) (Jason Laster)

v2.1.0 - July 10, 2015

* 2.1.0 (Nicholas C. Zakas)
* Fix: Leading comments for anonymous classes (fixes #155, fixes #158) (Toru Nagashima)
* New: Add newTarget option (fixes #157) (Nicholas C. Zakas)

v2.0.4 - June 26, 2015

* 2.0.4 (Nicholas C. Zakas)
* Docs: added missing `ecmaFeatures.superInFunctions` option from doc (Clément Fiorio)
* Fix: "await" is a future reserved word (fixes #151) (Jose Roberto Vidal)

v2.0.3 - June 2, 2015

* 2.0.3 (Nicholas C. Zakas)
* Fix: Incomplete Switch Statement Hangs (Fixes #146) (Jamund Ferguson)
* Docs: Clarify ecmaFeatures usage (Dan Wolff)

v2.0.2 - April 28, 2015

* 2.0.2 (Nicholas C. Zakas)
* Fix: Allow yield without value as function param (fixes #134) (Nicholas C. Zakas)
* Fix: Allow computed generators in classes (fixes #123) (Nicholas C. Zakas)
* Fix: Don't allow arrow function rest param (fixes #130) (Nicholas C. Zakas)

v2.0.1 - April 11, 2015

* 2.0.1 (Nicholas C. Zakas)
* Fix: Yield should parse without an argument (fixes #121) (Nicholas C. Zakas)

v2.0.0 - April 4, 2015

* 2.0.0 (Nicholas C. Zakas)
* Docs: Update README with latest info (Nicholas C. Zakas)
* Breaking: Use ESTree format for default params (fixes #114) (Nicholas C. Zakas)
* New: Add Super node (fixes #115) (Nicholas C. Zakas)
* Breaking: Switch to RestElement for rest args (fixes #84) (Nicholas C. Zakas)
* Docs: Correct license info on README (fixes #117) (AJ Ortega)
* Breaking: Remove guardedHandlers/handlers from try (fixes #71) (Nicholas C. Zakas)

v1.12.3 - March 28, 2015

* 1.12.3 (Nicholas C. Zakas)
* Fix: Tagged template strings (fixes #110) (Nicholas C. Zakas)

v1.12.2 - March 21, 2015

* 1.12.2 (Nicholas C. Zakas)
* Fix: Destructured arg for catch (fixes #105) (Nicholas C. Zakas)

v1.12.1 - March 21, 2015

* 1.12.1 (Nicholas C. Zakas)
* Fix: Disallow octals in template strings (fixes #96) (Nicholas C. Zakas)
* Fix: Template string parsing (fixes #95) (Nicholas C. Zakas)
* Fix: shorthand properties named get or set (fixes #100) (Brandon Mills)
* Fix: bad error in parsing invalid class setter (fixes #98) (Marsup)

v1.12.0 - March 14, 2015

* 1.12.0 (Nicholas C. Zakas)
* Fix: Update broken tests (Nicholas C. Zakas)
* New: Add sourceType to Program node (fixes #93) (Nicholas C. Zakas)
* Allow spread in more places (fixes #89) (Nicholas C. Zakas)
* Fix: Deeply nested template literals (fixes #86) (Nicholas C. Zakas)
* Fix: Allow super in classes by default (fixes #87) (Nicholas C. Zakas)
* Fix: generator methods in classes (fixes #85) (Jamund Ferguson)
* Remove XJS note from Esprima-FB incompatibilities (Joe Lencioni)

v1.11.0 - March 7, 2015

* 1.11.0 (Nicholas C. Zakas)
* Fix: Don't allow default export class by mistake (fixes #82) (Nicholas C. Zakas)
* Fix: Export default function should be FunctionDeclaration (fixes #81) (Nicholas C. Zakas)
* Fix: Ensure class declarations must have IDs outside of exports (refs #72) (Nicholas C. Zakas)
* Fix: export class expression support (refs #72) (Jamund Ferguson)
* Update: Add tests for sourceType=module (refs #72) (Nicholas C. Zakas)
* Fix: Class name should be id (fixes #78) (Nicholas C. Zakas)
* Fix: disallow import/export in functions (refs #72) (Jamund Ferguson)
* Test: strict mode enforced in modules (refs #72) (Jamund Ferguson)
* New: Add modules feature flag (refs #72) (Nicholas C. Zakas)
* merging upstream and solving conflicts for PR #43 (Caridy Patino)
* New: Add ES6 module support (fixes #35) (Caridy Patino)
* Update: Add TryStatement.handler (fixes #69) (Brandon Mills)
* Fix: Destructured Defaults (fixes #56) (Jamund Ferguson)
* Update: Refactor out comment attachment logic (Nicholas C. Zakas)

v1.10.0 - March 1, 2015

* 1.10.0 (Nicholas C. Zakas)
* New: Support ES6 classes (refs #10) (Nicholas C. Zakas)
* Docs: Update README.md (Jamund Ferguson)

v1.9.1 - February 21, 2015

* 1.9.1 (Nicholas C. Zakas)
* Fix: Allow let/const in switchcase (fixes #54) (Nicholas C. Zakas)

v1.9.0 - February 21, 2015

* 1.9.0 (Nicholas C. Zakas)
* Fix: Extend property method range and loc to include params (fixes #36) (Brandon Mills)
* New: spread operator (refs #10) (Jamund Ferguson)
* Fix: incorrectly parsed arrow fragment (refs #58) (Jamund Ferguson)
* New: Rest Parameter (refs: #10) (Jamund Ferguson)
* New: Destructuring (refs #10) (Jamund Ferguson)

v1.8.1 - February 7, 2015

* 1.8.1 (Nicholas C. Zakas)
* Build: Add Node.js 0.12 testing (Nicholas C. Zakas)
* Fix: Actuall fix tokenization issue with templates (fixes #44) (Nicholas C. Zakas)

v1.8.0 - February 6, 2015

* 1.8.0 (Nicholas C. Zakas)
* New: Support for Arrow Functions (refs #10) (Jamund Ferguson)
* New: Allow super references in functions (refs #10) (Nicholas C. Zakas)
* Update create-test.js (Jamund Ferguson)
* Fix: Tokenization for template strings (fixes #44) (Nicholas C. Zakas)
* New: Allow return in global scope (fixes #46) (Nicholas C. Zakas)

v1.7.1 - January 23, 2015

* 1.7.1 (Nicholas C. Zakas)
* Fix: When ecmaFeatures.forOf is true, check for operater is "undefined" when match keyword is "in" (fixes #39) (Peter Chanthamynavong)

v1.7.0 - January 23, 2015

* 1.7.0 (Nicholas C. Zakas)
* New: Add support for template strings (FredKSchott)
* New: Add support for default parameters (refs #10) (Jamund Ferguson)
* New: Add support for unicode code point escape sequences (FredKSchott)

v1.6.0 - January 10, 2015

* 1.6.0 (Nicholas C. Zakas)
* Update: Make comment attachment tests look at whole AST (Nicholas C. Zakas)
* Docs: Update README to reflect feature flags (Nicholas C. Zakas)
* Docs: Add a couple more FAQs to README (Nicholas C. Zakas)
* New: Add support for duplicate object literal properties (FredKSchott)
* New: Implement generators (refs #10) (Nicholas C. Zakas)

v1.5.0 - December 29, 2014

* 1.5.0 (Nicholas C. Zakas)
* Docs: Update README with compat info (Nicholas C. Zakas)
* Update: Add regex parsing test (Nicholas C. Zakas)
* Update: s/XJS/JSX/g (Nicholas C. Zakas)
* Build: Update release script (Nicholas C. Zakas)
* Update: Move SyntaxTree to ast-node-factory.js (FredKSchott)
* New: Add JSX parsing (fixes #26) (Nicholas C. Zakas)
* Update: Switch location marker logic (fixes #15) (Nicholas C. Zakas)
* 1.4.0 (Nicholas C. Zakas)

v1.4.0 - December 23, 2014

* 1.4.0 (Nicholas C. Zakas)
* Fix: Parsing issues with property methods (fixes #21) (Nicholas C. Zakas)
* New: Add support for shorthand properties (refs #10) (Nicholas C. Zakas)
* New: Add support for object literal method shorthand (refs #10) (Nicholas C. Zakas)
* Fix: Ensure comments are attached for return (fixes #2) (Nicholas C. Zakas)
* Build: Ensure CHANGELOG.md is committed on release (Nicholas C. Zakas)
* 1.3.1 (Nicholas C. Zakas)

v1.3.1 - December 22, 2014

* 1.3.1 (Nicholas C. Zakas)
* Fix: Add all files to npm package (fixes #17) (Nicholas C. Zakas)
* Update: Move Messages to separate file (Nicholas C. Zakas)
* Docs: Removed unnecessary comment (Nicholas C. Zakas)
* 1.3.0 (Nicholas C. Zakas)

v1.3.0 - December 21, 2014

* 1.3.0 (Nicholas C. Zakas)
* Build: Add release scripts (Nicholas C. Zakas)
* New: Add computed object literal properties (refs #10) (Nicholas C. Zakas)
* Build: Fix commands in Makefile.js (Nicholas C. Zakas)
* Docs: Add FAQ to README (Nicholas C. Zakas)
* Fix: Don't allow let/const in for loops (fixes #14) (Nicholas C. Zakas)
* New: Support for-of loops (refs #10) (Nicholas C. Zakas)
* Update: Change .ast.js files to .result.js files (Nicholas C. Zakas)
* New: Support ES6 octal literals (Nicholas C. Zakas)
* New: Ability to parse binary literals (Nicholas C. Zakas)
* Update: More tests for regex u flag (Nicholas C. Zakas)
* Update: Switch to using ecmaFeatures (Nicholas C. Zakas)
* Update: Add comment attachment tests (Nicholas C. Zakas)
* Update README.md (Jamund Ferguson)
* New: Add u and y regex flags (refs #10) (Nicholas C. Zakas)
* Update: Cleanup tests (Nicholas C. Zakas)
* New: Add ecmascript flag (fixes #7) (Nicholas C. Zakas)
* Docs: Update README with build commands (Nicholas C. Zakas)
* Update: Move some things around (Nicholas C. Zakas)
* Update: Read version number from package.json (Nicholas C. Zakas)
* Update: Move AST node types to separate file (Nicholas C. Zakas)
* Update: Remove duplicate file (Nicholas C. Zakas)
* Update: Move token information to a separate file (Nicholas C. Zakas)
* Update: Bring in Makefile.js for linting and browserify (Nicholas C. Zakas)
* Update: Fix ESLint warnings, remove check-version (Nicholas C. Zakas)
* Update: Move Position and SourceLocation to separate file (Nicholas C. Zakas)
* Update: Move syntax checks into separate file (Nicholas C. Zakas)
* Update: Remove UMD format (Nicholas C. Zakas)
* Docs: Update README with more info (Nicholas C. Zakas)
* Update: remove npm-debug.log from tracked files (Brandon Mills)
* Docs: Remove redundant 'features' in readme (Matthias Oßwald)
* Docs: Fix a link to Wikipedia (Ryuichi Okumura)
* Update: Split parsing tests into smaller files (Nicholas C. Zakas)
* Update: Normalize values in tests (Nicholas C. Zakas)
* Update: CommonJSify test file (Nicholas C. Zakas)

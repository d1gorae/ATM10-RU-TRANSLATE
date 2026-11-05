# Аудит 108 модов без одноимённого ru_ru.json

Дата проверки: 05.11.2026  
Цель: определить, каким из 108 mod ID действительно требуется отдельная русская локализация.

## Источники и метод

- Официальный modlist ATM10: `AllTheMods/ATM-10`, `config/crash_assistant/modlist.json`.
- Английская выгрузка: [ATM/LANGUAGES_EN_US](https://github.com/d1gorae/beamng-road-reference/tree/main/ATM/LANGUAGES_EN_US).
- [README выгрузки](https://github.com/d1gorae/beamng-road-reference/blob/main/ATM/README.txt), [mod-list.txt](https://github.com/d1gorae/beamng-road-reference/blob/main/ATM/mod-list.txt), [language-index.csv](https://github.com/d1gorae/beamng-road-reference/blob/main/ATM/language-index.csv).
- Сверка выполнена по точному имени JAR, а не только по mod ID.

README английской выгрузки сообщает: извлечено 412 языковых файлов из 399 JAR; не удалось прочитать 0 JAR. Поэтому отсутствие JAR в `language-index.csv` для JAR, присутствующего в `mod-list.txt`, означает, что в архивной версии не было извлечённого языкового файла. Десять JAR из актуального modlist в исходном списке JAR отсутствуют — их проверяли отдельно по upstream-репозиториям.

## Итоговая классификация

| Категория | Количество |
|---|---:|
| JAR из английской выгрузки без en_us.json | 89 |
| Пустые en_us.json (0 ключей) | 5 |
| Непустые en_us.json, уже полностью покрытые существующим RU | 3 |
| FTB Quests — отложен согласно правилам проекта | 1 |
| JAR отсутствуют в исходной выгрузке; проверены отдельно | 10 |
| **Всего** | **108** |

## 1. Нет собственного языкового JSON — отдельный перевод не требуется (89)

Для перечисленных JAR английская выгрузка не обнаружила `en_us.json`. Внутри архива ATM10 не найдено стандартных Minecraft translation keys для этих модов. Создавать пустые или искусственные русские JSON не нужно.

| Mod ID | Название | JAR |
|---|---|---|
| `ae2jeiintegration` | AE2 JEI Integration | `ae2jeiintegration-1.2.1.jar` |
| `aiimprovements` | AI-Improvements | `AI-Improvements-1.21-0.5.3.jar` |
| `alltheleaks` | All The Leaks | `alltheleaks-1.1.14-1.21.1-neoforge.jar` |
| `architectury` | Architectury | `architectury-13.0.11-neoforge.jar` |
| `athena` | Athena | `athena-neoforge-1.21.1-4.0.6.jar` |
| `atlas_api` | Atlas API | `atlas_api-1.21.1-1.2.0.jar` |
| `attributefix` | AttributeFix | `attributefix-neoforge-1.21.1-21.1.3.jar` |
| `blueflame` | Blue Flame Burning | `blueflame-1.21.1-1.1.1.jar` |
| `botanypotsmystical` | BotanyPots-Mystical | `botanypotsmystical-neoforge-1.21.1-21.1.12.jar` |
| `botanytrees` | BotanyTrees | `botanytrees-neoforge-1.21.1-21.1.7.jar` |
| `byzantine` | Byzantine | `Byzantine-1.21.1-51.1.jar` |
| `catjammies` | CatJammies | `catjammies-1.21-1.7.1.jar` |
| `cleanswing` | Clean Swing | `cleanswing-1.10-1.21.jar` |
| `clumps` | Clumps | `Clumps-neoforge-1.21.1-19.0.0.1.jar` |
| `cobweb` | Cobweb | `cobweb-neoforge-1.21-1.4.0.jar` |
| `connectivity` | Connectivity Mod | `connectivity-1.21.1-7.7.jar` |
| `corgilib` | CorgiLib | `Corgilib-NeoForge-1.21.1-5.0.0.10.jar` |
| `crash_assistant` | Crash Assistant | `CrashAssistant-neoforge-1.20.6-1.21.4-1.11.12.jar` |
| `cryonicconfig` | Cryonic Config | `cryonicconfig-neoforge-1.0.0+mc1.21.11.jar` |
| `cupboard` | Cupboard mod | `cupboard-1.21.1-4.2.jar` |
| `deimos` | Deimos | `deimos-1.21.1-neoforge-2.8.jar` |
| `dungeoncrawl` | Dungeon Crawl | `DungeonCrawl-NeoForge-1.21-2.3.17.jar` |
| `edivadlib` | EdivadLib | `EdivadLib-1.21-3.0.0.jar` |
| `experiencelib` | ExperienceLib | `experiencelib-1.21.1-1.2.1.jar` |
| `explorify` | Explorify | `Explorify v1.6.5.mod.jar` |
| `fastfurnace` | FastFurnace | `FastFurnace-1.21.1-9.0.1.jar` |
| `fastsuite` | Fast Suite | `FastSuite-1.21.1-6.0.7.jar` |
| `ferritecore` | Ferrite Core | `ferritecore-7.0.3-neoforge.jar` |
| `flickerfix` | FlickerFix | `flickerfix-1.21.1-6.1.0.jar` |
| `formationsnether` | Formations Nether | `formationsnether-1.0.5b-mc1.21+.jar` |
| `formationsoverworld` | Formations Overworld | `formationsoverworld-1.0.5c-mc1.21+.jar` |
| `framework` | Framework | `framework-neoforge-1.21.1-0.13.11.jar` |
| `ftbranks` | FTB Ranks | `ftb-ranks-neoforge-2101.1.5.jar` |
| `fuelgoeshere` | Fuel Goes Here | `fuelgoeshere-1.21.1-1.2.0.jar` |
| `geckolib` | GeckoLib 4 | `geckolib-neoforge-1.21.1-4.9.3.jar` |
| `glodium` | Glodium | `Glodium-1.21-2.2-neoforge.jar` |
| `hellish_trials` | Hellish Trials | `HellishTrials-neoforge-1.0.5.jar` |
| `heyberryshutup` | Hey Berry! SHUT UP | `heyberryshutup-1.21.0-2.0.4.jar` |
| `iceberg` | Iceberg | `Iceberg-1.21.1-neoforge-1.3.2.jar` |
| `incontrol` | InControl | `incontrol-1.21-10.3.1.jar` |
| `jumpboat` | Jumpy Boats | `jumpboat-1.21.0-1.0.5.jar` |
| `konkrete` | Konkrete | `konkrete_neoforge_1.9.9_MC_1.21.jar` |
| `kubejs` | KubeJS | `kubejs-neoforge-2101.7.2-build.381.jar` |
| `lithostitched` | Lithostitched | `lithostitched-1.8.1-neoforge-21.1.jar` |
| `lmft` | Load My F***ing Tags | `lmft-1.1.1+1.21.9-neoforge.jar` |
| `melody` | Melody | `melody_neoforge_1.0.10_MC_1.21.jar` |
| `modelfix` | Model Gap Fix | `modelfix-1.21-1.10.jar` |
| `monolib` | MonoLib | `monolib-neoforge-1.21.1-4.1.2.jar` |
| `moredragoneggs` | More Dragon Eggs | `moredragoneggs-5.0.jar` |
| `moreredxcctcompat` | More Red x CC:Tweaked Compat | `MoreRed-CCT-Compat-1.21.1-1.3.0.jar` |
| `mousetweaks` | Mouse Tweaks | `MouseTweaks-neoforge-mc1.21-2.26.1.jar` |
| `mysticalcustomization` | Mystical Customization | `MysticalCustomization-1.21.1-6.0.2.jar` |
| `netherportalfix` | NetherPortalFix | `netherportalfix-neoforge-1.21.1-21.1.1.jar` |
| `novillagerdm` | No Villager Death Messages | `novillagerdm-1.21.1-6.0.0.jar` |
| `nullscape` | Nullscape | `Nullscape_1.21.x_v1.2.14.jar` |
| `observerlib` | ObserverLib | `observerlib-1.10.3.jar` |
| `occultism_kubejs` | Occultism KubeJS | `occultism_kubejs-1.21.1-neoforge-1.11.0.jar` |
| `octolib` | OctoLib | `OctoLib-NEOFORGE-0.6.2+1.21.jar` |
| `ohthetreesyoullgrow` | Oh The Trees You'll Grow | `Oh-The-Trees-Youll-Grow-neoforge-1.21.1-5.3.5.jar` |
| `omegaconfig` | Omega Config Architectury | `omegaconfig-neoforge-1.5.1.jar` |
| `openloader` | OpenLoader | `OpenLoader-neoforge-1.21.1-21.1.5.jar` |
| `overlapless` | Overlapless | `overlapless-1.21.1-1.2.0.jar` |
| `overloadedarmorbar` | OverloadedArmorBar | `overloadedarmorbar-neoforge-1.21-2.jar` |
| `playeranimator` | Player Animator | `player-animation-lib-forge-2.0.4+1.21.1.jar` |
| `polyeng` | Polymorphic Energistics | `polyeng-0.4.1.jar` |
| `ponderjs` | PonderJS | `ponderjs-neoforge-1.21.1-2.4.0.jar` |
| `prickle` | PrickleMC | `prickle-neoforge-1.21.1-21.1.11.jar` |
| `prism` | Prism | `Prism-1.21.1-neoforge-1.0.11.jar` |
| `rebind_narrator` | Rebind Narrator | `rebind_narrator-1.21.1-neoforge-2026.08.31.jar` |
| `resourcefullib` | Resourceful Lib | `resourcefullib-neoforge-1.21-3.0.12.jar` |
| `rhino` | Rhino | `rhino-2101.2.8-build.91.jar` |
| `smartbrainlib` | SmartBrainLib | `SmartBrainLib-neoforge-1.21.1-1.16.11.jar` |
| `sophisticatedbackpackscreateintegration` | Sophisticated Backpacks Create Integration | `sophisticatedbackpackscreateintegration-1.21.1-0.2.3.194.jar` |
| `sophisticatedstoragecreateintegration` | Sophisticated Storage Create Integration | `sophisticatedstoragecreateintegration-1.21.1-0.1.23.246.jar` |
| `spark` | spark | `spark-1.10.124-neoforge.jar` |
| `structory` | Structory | `Structory_26.2_v1.3.7.jar` |
| `structory_towers` | Structory: Towers | `Structory_Towers_26.1_v1.0.16.jar` |
| `stylecolonies` | Stylecolonies | `stylecolonies-1.15.66-1.21.1.jar` |
| `supermartijn642configlib` | SuperMartijn642's Config Library | `supermartijn642configlib-1.1.8-neoforge-mc1.21.jar` |
| `sussysniffers` | Sussy Sniffers | `sussysniffers-1.21.1-0.1.3.jar` |
| `t_and_t` | Towns and Towers | `t_and_t-fabric-neoforge-1.13.11.jar` |
| `theurgy_kubejs` | Theurgy KubeJS | `theurgy_kubejs-1.21.1-neoforge-1.6.0.jar` |
| `towntalk` | Towntalk | `towntalk-1.2.0.jar` |
| `underground_villages` | Underground Villages Mod | `UndergroundVillages-neoforge-1.21.1-4.0.3.jar` |
| `valhelsia_core` | Valhelsia Core | `valhelsia_core-neoforge-1.21.1-1.1.5.jar` |
| `villagesandpillages` | Villages&Pillages | `villagesandpillages-neoforge-2.0.0+mc1.21.1.jar` |
| `wits` | Wits | `wits-neoforge-1.3.1.jar` |
| `yeetusexperimentus` | Yeetus Experimentus | `yeetusexperimentus-neoforge-87.0.0.jar` |
| `yungsextras` | YUNG's Extras | `YungsExtras-1.21.1-NeoForge-5.1.1.jar` |

## 2. Английский JSON существует, но пустой (5)

Во всех пяти файлах JSON — пустой объект, ключей для перевода нет.

- **Accelerated Decay** (`accelerateddecay`) — `accelerated-decay-neoforge-21.0.0.jar`; namespace: `accelerateddecay`.
- **FTB Jei Extras** (`ftbjeiextras`) — `ftb-jei-extras-21.1.7.jar`; namespace: `ftbjeiextras`.
- **FTB XMod Compat** (`ftbxmodcompat`) — `ftb-xmod-compat-neoforge-21.1.14.jar`; namespace: `ftbxmodcompat`.
- **Illager-Warship** (`illagerwarship`) — `illagerwarship-1.0.1-neoforge-1.21.1.jar`; namespace: `illagerwarship`.
- **Rechiseled: Chipped** (`rechiseled_chipped`) — `rechiseled_chipped-2.0-1.21.1.jar`; namespace: `rechiseled_chipped`.

Результат: отдельный RU JSON не требуется.

## 3. Английские ключи уже покрыты существующим русским файлом (3)

Проверено совпадение ключей с актуальными русскими файлами репозитория:

| Мод | Английских ключей | RU-файл | Пропущено |
|---|---:|---|---:|
| ATM: Compat | 10 | `assets/allthemodium/lang/ru_ru.json` | 0 |
| Borderless Window | 21 | `assets/borderless/lang/ru_ru.json` | 0 |
| Cloth Config | 49 | `assets/cloth-config2/lang/ru_ru.json` | 0 |

Новые JSON создавать не нужно.

## 4. FTB Quests — оставить на самый конец

- **FTB Quests** (`ftbquests`) — английский `en_us.json` содержит 774 ключа.
- Не включать в текущую работу по 108 модам: FTB Quests и SNBT остаются отложенными согласно правилам проекта.
- Ранее выполненная локализация глав и SNBT учитывается отдельно; этот аудит не объявляет повторную проверку FTB Quests завершённой.

## 5. JAR отсутствуют в английской выгрузке — отдельная проверка (10)

Эти десять JAR отсутствуют в `ATM/mod-list.txt` английской выгрузки, поэтому их нельзя автоматически считать не имеющими языковых файлов.

### 5.1. Найдены английские языковые файлы — требуется локализация (6)

| Mod ID | Мод | Ключей в проверенном upstream en_us | Примечание |
|---|---|---:|---|
| `bibliobiomes` | Bibliobiomes Legacy | 2 041 | shared namespace bibliocraft; current upstream snapshot |
| `bibliowoods` | Bibliowoods Legacy | 4 553 | shared namespace bibliocraft; current upstream snapshot |
| `iris` | Iris | 73 | assets/iris/lang/en_us.json |
| `iris_search` | IrisSearch | 13 | assets/iris_search/lang/en_us.json |
| `sodium` | Sodium | 105 | assets/sodium/lang/en_us.json |
| `sodium_extra` | Sodium Extra | 422 | assets/sodium-extra/lang/en_us.json |

**Bibliobiomes и Bibliowoods:** оба используют общий namespace `bibliocraft`, поэтому отдельные RU JSON не создавать. В существующем `assets/bibliocraft/lang/ru_ru.json` найдено 23 059 ключей. Сравнение с текущими upstream English-файлами (2 041 + 4 553 = 6 594 ключа) показало 5 495 уже имеющихся ключей и 1 099 отсутствующих. Это предварительная оценка по текущим upstream-файлам: перед добавлением переводов необходимо повторить сравнение именно с содержимым установленных JAR ATM10 (`bibliobiomes 1.6.1`, `bibliowoods 1.6.2`), чтобы не добавить ключи из более новых версий.

Для Iris, IrisSearch, Sodium и Sodium Extra соответствующие русские namespace-файлы в текущем дереве репозитория не обнаружены. Их upstream English-файлы содержат соответственно 73, 13, 105 и 422 ключа. Перед переводом зафиксировать точные версии из ATM10 и сверить ключи именно с ними.

### 5.2. Языковой JSON не обнаружен; отдельный перевод не требуется (4)

| Mod ID | Мод | Основание |
|---|---|---|
| `colorwheel` | Colorwheel | Рендеринговая интеграция Iris/Flywheel; отдельный языковой файл не найден |
| `colorwheel_patcher` | Colorwheel Patcher | Патчи совместимости шейдерпаков; отдельный языковой файл не найден |
| `immediatelyfast` | ImmediatelyFast | Оптимизация рендеринга; настройки находятся в конфигурации, отдельный языковой файл не найден |
| `uranus` | Uranus | Библиотека/API для других модов; отдельный языковой файл не найден |

## 6. Что считать закрытым

- 89 модов: стандартного языкового JSON нет — закрыть без создания RU-файла.
- 5 модов: английские JSON пустые — закрыть без создания RU-файла.
- 3 модов: все английские ключи уже присутствуют в русских общих namespace — закрыть без создания новых файлов.
- 4 модов из отсутствовавших в архиве: отдельная локализация не требуется по назначению и найденным ресурсам.
- FTB Quests: не трогать до финального этапа проекта.
- Шесть модов с языковыми ресурсами: не закрывать; перенести в очередь локализации. Для Biblio сначала подтвердить точное число ключей по установленным JAR.

**Вывод:** по текущим данным 101 из 108 не требуют создания нового самостоятельного RU JSON. Один мод (FTB Quests) отложен. Шесть модов требуют локализации или дополнения общего namespace. В отношении 1 099 Biblio-ключей число предварительное до сверки точных версий JAR.

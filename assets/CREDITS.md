# 받은 에셋 출처

모두 CC0 1.0 (퍼블릭 도메인)이다. 출처 표기 의무는 없지만 여기 남긴다. 게임에 맞게 크기를 줄이거나 밝기를 바꾸고, 소리는 모노 mp3로 바꿨다(앞 무음 자르기, 봉우리 -1 dBFS).

| 파일 | 원본 | 만든 이 | 받은 곳 | 바꾼 것 |
|---|---|---|---|---|
| `s2/dark_rock_*.jpg` | Dark Rock (1K) | Poly Haven | https://polyhaven.com/a/dark_rock | 색 지도 밝기 올림, AO(R)·거칠기(G)를 `arm` 한 장으로 |
| `s2/rock_09/` | Rock 09 (glTF 1K) | Poly Haven | https://polyhaven.com/a/rock_09 | 질감 512로, 버퍼를 넣은 glTF 한 파일(rock_09.json) |
| `s2/lava_*.jpg` | Lava 001 (1K-JPG) | ambientCG | https://ambientcg.com/view?id=Lava001 | 색·빛·노멀 512로 |
| `sfx/swing_*.mp3` | 20 sword sound effects (attacks) | StarNinjas | https://opengameart.org/content/20-sword-sound-effects-attacks-and-clashes | 1, 4, 5, 7번 |
| `sfx/clash_*.mp3` | 같은 묶음 (clashes) | StarNinjas | 같은 곳 | 1~6번 |
| `sfx/soft_*`, `punch_*`, `plate_*`, `metal_*`, `step_*` | Impact Sounds | Kenney (kenney.nl) | https://github.com/Boyquotes/kenney-impact-sounds-for-godot (Kenney 원본의 CC0 사본) | footstep_concrete → step |
| `chars/knight.json`, `mage.json`, `barbarian.json`, `rogue_hooded.json` | KayKit Character Pack: Adventures 1.0 (Knight, Mage, Barbarian, Rogue_Hooded) | Kay Lousberg | https://github.com/KayKit-Game-Assets/KayKit-Character-Pack-Adventures-1.0 (LICENSE.txt: CC0) | 쓰는 동작만 남기고 안 쓰는 손 장비를 뗀 뒤 버퍼·그림을 넣은 glTF 한 파일로 (`tools/glb2json.js`) |
| `chars/skeleton_warrior.json` | KayKit Character Pack: Skeletons 1.0 (Skeleton_Warrior) | Kay Lousberg | https://github.com/KayKit-Game-Assets/KayKit-Character-Pack-Skeletons-1.0 (LICENSE.txt: CC0) | 같음. 칼은 기사 모델의 한손검을 손 뼈에 쥐여 준다 |
| `chars/slime.json`, `bat.json`, `goleling.json` | Pink Slime, Bat, Goleling Evolved | Quaternius | https://poly.pizza/m/AyP8sQmDLh, https://poly.pizza/m/hNO9XvjlKa, https://poly.pizza/m/iHEuXiH6Aj (CC0) | 같음 |
| `props/crystal*.json` | Crystal, Big Crystal | Quaternius | poly.pizza (CC0) | 같음 |
| `floor/slab_tiles_*`, `metal_plate_*`, `stone_tiles_02_*` | Slab Tiles, Metal Plate, Stone Tiles 02 (1K) | Poly Haven | https://polyhaven.com/a/slab_tiles, https://polyhaven.com/a/metal_plate, https://polyhaven.com/a/stone_tiles_02 | 색·노멀 1024, arm 512로 다시 압축 |
| `ph/*.json` (통·상자·양동이·공구 상자·화덕·등·샹들리에·바위·고딕 석상·책장·쇠문·카이트 방패·산업 배관 15종) | wine_barrel_01, wooden_crate_02, old_military_crate, wooden_bucket_01, metal_tool_chest, stone_fire_pit, wooden_lantern_01, lantern_chandelier_01, rock_moss_set_01, rock_07, gothic_statue, wooden_bookshelf_worn, large_iron_gate, kite_shield, modular_industrial_pipes_01 (glTF 1K) | Poly Haven | https://polyhaven.com/models (https://polyhaven.com/license, CC0) | 그림 512로 줄여 glTF 한 파일로 (`tools/gltf2json.py`) |
| `tex/*` (castle_wall_slates, medieval_blocks_02, rusty_metal_02, dark_brick_wall, metal_grate_rusty, large_sandstone_blocks, cobblestone_floor_04, medieval_wall_01, weathered_planks) | 같은 이름 (1K) | Poly Haven | https://polyhaven.com/textures (CC0) | 색·노멀 1024, arm 512로 다시 압축 |

받은 날: 2026-11-02 (캐릭터 모델도 같은 날). 라이선스 원문은 각 받은 곳에 있다 (Poly Haven, ambientCG는 사이트 전체가 CC0).


## 생성 그림 (받은 에셋이 아님)

기사·골렘·슬라임·박쥐·문지기의 `spr/` 동작 시트는 사용자가 GPT 앱·Codex 이미지 생성으로 이 게임을 위해 새로 그린 원본(자산원본/생성/, git 밖)을 `tools/sprsheet.py`로 손질한 것이다. 프롬프트는 자산원본/생성-프롬프트.md.

`spr/town_basin.webp`(석조 수반)과 `tex/town_plaza.webp`(광장 판석)는 Codex에서 생성한 마을 전용 그림이다. 원본 PNG는 자산원본/생성/town/에 보관한다.

기사와 몬스터 네 종은 각 동작의 앞·뒤 4칸을 한 줄에 담았다. 마을 사람 여덟 명의 `spr/npc_*.webp`는 자산원본/생성/npc/의 원본을 같은 도구로 변환했다. 대장장이의 게임용 망치질 그림에는 마을에 이미 놓인 모루를 그려 넣지 않았다.

고목·철제 가로등·수정 군락과 탑·지하도시·성채·균열의 바닥도 이 게임을 위해 생성했다. 원본은 자산원본/생성/의 town, s1, s3, s4, rift 폴더에 있다.

## 소리 2차: 디아블로 2 리저렉션풍 녹음 음악·환경음·몬스터 목소리 (2026-11-02)

모두 OpenGameArt의 CC0 (각 페이지 License(s): CC0). 받은 곳은 https://opengameart.org/sites/default/files/<파일명>. 음악은 스테레오 80 kbps, 환경음·효과음은 모노 mp3로 다시 부호화하고 세기를 맞췄다(loudnorm). 반복이 아닌 곡은 앞뒤를 짧게 페이드.

| 파일 | 원본 (만든 이) |
|---|---|
| `music/town.mp3` | TownTheme.mp3 — Town Theme RPG (cynicmusic) |
| `music/s1.mp3` | cursed_tower_veranda_loop.mp3 — Cursed Tower Veranda (Bobjt) |
| `music/s2.mp3` | qubodup-yd-DarkShrineLoop-OpenGameArt.ogg — Dark Shrine Loop (qubodup, yd) |
| `music/s3.mp3` | Factory.ogg — Factory ambiance (yd) |
| `music/s4.mp3` | dungeon002_0.ogg — Dungeon Ambience (yd), 150초로 자름 |
| `music/rift.mp3` | dark_cavern_ambient_002.ogg — dark cavern ambient 002 (Paul Wortmann) |
| `amb/dungeon.mp3` | dungeon_ambient_1_0.ogg — loopable dungeon ambience (JaggedStone) |
| `amb/lava.mp3`, `sfx/fire_0.mp3` | deep_rumble.ogg (gmason), fire-1_0.ogg (AntumDeluge) |
| `amb/birds.mp3`, `sfx/anvil_0.mp3` | birds-isaiah658_0.ogg (isaiah658), forger_0.ogg (themightyglider) |
| `sfx/steam_*.mp3` | steam_hisses.zip — steam hisses (bart) |
| `sfx/slime_v*`, `sfx/slime_d*` | water-splash-slime-sfx.zip — 40 water/splash/slime SFX (rubberduck): slime_01·05·09·13, splash_02·03 |
| `sfx/bat_v*` | bat.zip — bat screeches (AntumDeluge, 원 소리 polymorpheva freesound 104205, CC0), 0.65초로 자름 |
| `sfx/golem_v*`, `sfx/guard_*` | 80-CC0-creature-SFX_0.zip (rubberduck): roar_01~03, troll_01~03, grunt_01·02 |
| `sfx/level_0.mp3` | jingleSounds_Kenney.zip — jingles_STEEL07 (Kenney) |

2026-11-02 검수 뒤: KayKit Dungeon 소품 28종과 Quaternius 배관 2종은 Poly Haven 모델로 모두 바뀌어 쓰지 않으므로 지웠다.

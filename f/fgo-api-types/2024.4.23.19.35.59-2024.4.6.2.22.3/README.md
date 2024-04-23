# Comparing `tmp/fgo_api_types-2024.4.23.19.35.59.tar.gz` & `tmp/fgo_api_types-2024.4.6.2.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.4.23.19.35.59.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.4.6.2.22.3.tar", max compression
```

## Comparing `fgo_api_types-2024.4.23.19.35.59.tar` & `fgo_api_types-2024.4.6.2.22.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-04-23 19:35:42.548385 fgo_api_types-2024.4.23.19.35.59/LICENSE
--rw-r--r--   0        0        0      449 2024-04-23 19:35:42.548385 fgo_api_types-2024.4.23.19.35.59/README.md
--rw-r--r--   0        0        0        0 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/base.py
--rw-r--r--   0        0        0     4368 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3762 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/common.py
--rw-r--r--   0        0        0    40935 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/enums.py
--rw-r--r--   0        0        0   177949 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    86109 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/nice.py
--rw-r--r--   0        0        0    59051 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19285 2024-04-23 19:35:59.420549 fgo_api_types-2024.4.23.19.35.59/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-04-23 19:35:59.736552 fgo_api_types-2024.4.23.19.35.59/pyproject.toml
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.23.19.35.59/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/LICENSE
+-rw-r--r--   0        0        0      449 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4368 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3762 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py
+-rw-r--r--   0        0        0    40655 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   176026 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    85618 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59051 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19285 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-04-06 02:22:03.705703 fgo_api_types-2024.4.6.2.22.3/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.6.2.22.3/PKG-INFO
```

### Comparing `fgo_api_types-2024.4.23.19.35.59/LICENSE` & `fgo_api_types-2024.4.6.2.22.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/basic.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/common.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/enums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,17 +356,14 @@
     salemAbby = "salemAbby"
     uOlgaMarie = "uOlgaMarie"
     uOlgaMarieAlienGod = "uOlgaMarieAlienGod"
     beast = "beast"
     beastVI = "beastVI"
     beastVIBoss = "beastVIBoss"
     uOlgaMarieFlare = "uOlgaMarieFlare"
-    uOlgaMarieAqua = "uOlgaMarieAqua"
-    uOlgaMarieFlareCollection = "uOlgaMarieFlareCollection"
-    uOlgaMarieAquaCollection = "uOlgaMarieAquaCollection"
     atlasUnmappedClass = "atlasUnmappedClass"
     # OTHER = "OTHER"
     ALL = "ALL"
     # EXTRA = "EXTRA"
     # MIX = "MIX"
 
 
@@ -403,31 +400,28 @@
     30: SvtClass.beastILost,
     31: SvtClass.uOlgaMarieAlienGod,
     32: SvtClass.uOlgaMarie,
     33: SvtClass.beast,
     34: SvtClass.beastVI,
     35: SvtClass.beastVIBoss,
     36: SvtClass.uOlgaMarieFlare,
-    37: SvtClass.uOlgaMarieAqua,
     97: SvtClass.unknown,
     # 98
     # 99
     # 100
     107: SvtClass.agarthaPenth,
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
     # 1000: SvtClass.OTHER,
     # For Support List
     1001: SvtClass.ALL,
     # 1002: SvtClass.EXTRA,
     # 1003: SvtClass.MIX,
     # 1004: SvtClass.EXTRA1,
     # 1005: SvtClass.EXTRA2,
-    9001: SvtClass.uOlgaMarieFlareCollection,
-    9002: SvtClass.uOlgaMarieAquaCollection,
 }
 
 
 def get_class_name(class_id: int) -> SvtClass | str:
     if class_id in CLASS_NAME:
         return CLASS_NAME[class_id]
     else:
```

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/gameenums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,16 +258,14 @@
     SUB_FIELD_BUFF = 131
     EVENT_FORTIFICATION_POINT_UP = 132
     GAIN_NP_INDIVIDUAL_SUM = 133
     SET_QUEST_ROUTE_FLAG = 134
     LAST_USE_PLAYER_SKILL_COPY = 135
     CHANGE_ENEMY_MASTER_FACE = 136
     DAMAGE_VALUE_SAFE_ONCE = 137
-    ADD_BATTLE_VALUE = 138
-    SET_BATTLE_VALUE = 139
 
 
 class NiceFuncType(StrEnum):
     """Function Type Enum"""
 
     none = "none"
     addState = "addState"
@@ -366,16 +364,14 @@
     subFieldBuff = "subFieldBuff"
     eventFortificationPointUp = "eventFortificationPointUp"
     gainNpIndividualSum = "gainNpIndividualSum"
     setQuestRouteFlag = "setQuestRouteFlag"
     lastUsePlayerSkillCopy = "lastUsePlayerSkillCopy"
     changeEnemyMasterFace = "changeEnemyMasterFace"
     damageValueSafeOnce = "damageValueSafeOnce"
-    addBattleValue = "addBattleValue"
-    setBattleValue = "setBattleValue"
 
 
 FUNC_TYPE_NAME: dict[int, NiceFuncType] = {
     0: NiceFuncType.none,
     1: NiceFuncType.addState,
     2: NiceFuncType.subState,
     3: NiceFuncType.damage,
@@ -472,16 +468,14 @@
     131: NiceFuncType.subFieldBuff,
     132: NiceFuncType.eventFortificationPointUp,
     133: NiceFuncType.gainNpIndividualSum,
     134: NiceFuncType.setQuestRouteFlag,
     135: NiceFuncType.lastUsePlayerSkillCopy,
     136: NiceFuncType.changeEnemyMasterFace,
     137: NiceFuncType.damageValueSafeOnce,
-    138: NiceFuncType.addBattleValue,
-    139: NiceFuncType.setBattleValue,
 }
 
 
 class FuncTargetType(IntEnum):
     SELF = 0
     PT_ONE = 1
     PT_ANOTHER = 2
@@ -1760,15 +1754,14 @@
     EUQIP_SKILL_USE_ITEM = 28
     SVT_COIN = 29
     FRIENDSHIP_UP_ITEM = 30
     PP = 31
     TRADE_AP = 32
     RI = 33
     STORMPOD = 34
-    BATTLE_ITEM = 35
 
 
 class NiceItemType(StrEnum):
     """Item Type Enum"""
 
     qp = "qp"
     stone = "stone"
@@ -1800,15 +1793,14 @@
     euqipSkillUseItem = "euqipSkillUseItem"
     svtCoin = "svtCoin"
     friendshipUpItem = "friendshipUpItem"
     pp = "pp"
     tradeAp = "tradeAp"
     ri = "ri"
     stormpod = "stormpod"
-    battleItem = "battleItem"
 
 
 ITEM_TYPE_NAME: dict[int, NiceItemType] = {
     1: NiceItemType.qp,
     2: NiceItemType.stone,
     3: NiceItemType.apRecover,
     4: NiceItemType.apAdd,
@@ -1838,15 +1830,14 @@
     28: NiceItemType.euqipSkillUseItem,
     29: NiceItemType.svtCoin,
     30: NiceItemType.friendshipUpItem,
     31: NiceItemType.pp,
     32: NiceItemType.tradeAp,
     33: NiceItemType.ri,
     34: NiceItemType.stormpod,
-    35: NiceItemType.battleItem,
 }
 
 
 class GiftType(IntEnum):
     SERVANT = 1
     ITEM = 2
     FRIENDSHIP = 3
@@ -1858,15 +1849,14 @@
     COSTUME_RELEASE = 9
     COSTUME_GET = 10
     COMMAND_CODE = 11
     EVENT_POINT_BUFF = 12
     EVENT_BOARD_GAME_TOKEN = 13
     EVENT_COMMAND_ASSIST = 14
     EVENT_HEEL_PORTRAIT = 15
-    BATTLE_ITEM = 16
 
 
 class NiceGiftType(StrEnum):
     """Gift Type Enum"""
 
     servant = "servant"
     item = "item"
@@ -1879,15 +1869,14 @@
     costumeRelease = "costumeRelease"
     costumeGet = "costumeGet"
     commandCode = "commandCode"
     eventPointBuff = "eventPointBuff"
     eventBoardGameToken = "eventBoardGameToken"
     eventCommandAssist = "eventCommandAssist"
     eventHeelPortrait = "eventHeelPortrait"
-    battleItem = "battleItem"
 
 
 GIFT_TYPE_NAME: dict[int, NiceGiftType] = {
     1: NiceGiftType.servant,
     2: NiceGiftType.item,
     3: NiceGiftType.friendship,
     4: NiceGiftType.userExp,
@@ -1898,15 +1887,14 @@
     9: NiceGiftType.costumeRelease,
     10: NiceGiftType.costumeGet,
     11: NiceGiftType.commandCode,
     12: NiceGiftType.eventPointBuff,
     13: NiceGiftType.eventBoardGameToken,
     14: NiceGiftType.eventCommandAssist,
     15: NiceGiftType.eventHeelPortrait,
-    16: NiceGiftType.battleItem,
 }
 
 
 class ShopType(IntEnum):
     NONE = 0
     EVENT_ITEM = 1
     MANA = 2
@@ -3831,20 +3819,14 @@
     COUNT_PLAYER_SKILL_EQUAL_INCLUDE_MASTER_SKILL = 190
     TOTAL_TURN_HIGHER = 191
     TOTAL_TURN_LOWER = 192
     TOTAL_TURN_EQUAL = 193
     CHECK_WAR_BOARD_SQUARE_INDIVIDUALITY = 194
     CHECK_PT_HIGHER_NPGAUGE = 195
     CHECK_SELF_HIGHER_NPGAUGE = 196
-    CHECK_BATTLE_VALUE_ABOVE = 197
-    CHECK_BATTLE_VALUE_EQUAL = 198
-    CHECK_BATTLE_VALUE_NOT_EQUAL = 199
-    CHECK_BATTLE_VALUE_BELOW = 200
-    CHECK_BATTLE_VALUE_BETWEEN = 201
-    CHECK_BATTLE_VALUE_NOT_BETWEEN = 202
 
 
 class NiceAiCond(StrEnum):
     """AI Cond Enum"""
 
     none = "none"
     hpHigher = "hpHigher"
@@ -4015,20 +3997,14 @@
     countPlayerSkillEqualIncludeMasterSkill = "countPlayerSkillEqualIncludeMasterSkill"
     totalTurnHigher = "totalTurnHigher"
     totalTurnLower = "totalTurnLower"
     totalTurnEqual = "totalTurnEqual"
     checkWarBoardSquareIndividuality = "checkWarBoardSquareIndividuality"
     checkPtHigherNpgauge = "checkPtHigherNpgauge"
     checkSelfHigherNpgauge = "checkSelfHigherNpgauge"
-    checkBattleValueAbove = "checkBattleValueAbove"
-    checkBattleValueEqual = "checkBattleValueEqual"
-    checkBattleValueNotEqual = "checkBattleValueNotEqual"
-    checkBattleValueBelow = "checkBattleValueBelow"
-    checkBattleValueBetween = "checkBattleValueBetween"
-    checkBattleValueNotBetween = "checkBattleValueNotBetween"
 
 
 AI_COND_NAME: dict[int, NiceAiCond] = {
     0: NiceAiCond.none,
     10: NiceAiCond.hpHigher,
     11: NiceAiCond.hpLower,
     20: NiceAiCond.actcount,
@@ -4181,20 +4157,14 @@
     190: NiceAiCond.countPlayerSkillEqualIncludeMasterSkill,
     191: NiceAiCond.totalTurnHigher,
     192: NiceAiCond.totalTurnLower,
     193: NiceAiCond.totalTurnEqual,
     194: NiceAiCond.checkWarBoardSquareIndividuality,
     195: NiceAiCond.checkPtHigherNpgauge,
     196: NiceAiCond.checkSelfHigherNpgauge,
-    197: NiceAiCond.checkBattleValueAbove,
-    198: NiceAiCond.checkBattleValueEqual,
-    199: NiceAiCond.checkBattleValueNotEqual,
-    200: NiceAiCond.checkBattleValueBelow,
-    201: NiceAiCond.checkBattleValueBetween,
-    202: NiceAiCond.checkBattleValueNotBetween,
 }
 
 
 class AiActType(IntEnum):
     NONE = 0
     RANDOM = 1
     ATTACK = 2
@@ -4696,15 +4666,14 @@
     CHECK_TARGET_SKILL_THISTURN = 34
     CHECK_SELECT_CHAIN = 35
     COUNT_PLAYER_NP = 36
     COUNT_PLAYER_SKILL = 37
     COUNT_PLAYER_SKILL_INCLUDE_MASTER_SKILL = 38
     TOTAL_TURN = 39
     WAR_BOARD_SQUARE_INDIVIDUALITY = 40
-    CHECK_BATTLE_VALUE = 41
 
 
 class NiceAiCondParameter(StrEnum):
     """Ai Condition Parameter"""
 
     none = "none"
     turn = "turn"
@@ -4743,15 +4712,14 @@
     checkTargetSkillThisturn = "checkTargetSkillThisturn"
     checkSelectChain = "checkSelectChain"
     countPlayerNp = "countPlayerNp"
     countPlayerSkill = "countPlayerSkill"
     countPlayerSkillIncludeMasterSkill = "countPlayerSkillIncludeMasterSkill"
     totalTurn = "totalTurn"
     warBoardSquareIndividuality = "warBoardSquareIndividuality"
-    checkBattleValue = "checkBattleValue"
 
 
 AI_COND_PARAMETER_NAME: dict[int, NiceAiCondParameter] = {
     0: NiceAiCondParameter.none,
     1: NiceAiCondParameter.turn,
     2: NiceAiCondParameter.space,
     3: NiceAiCondParameter.prevActid,
@@ -4788,15 +4756,14 @@
     34: NiceAiCondParameter.checkTargetSkillThisturn,
     35: NiceAiCondParameter.checkSelectChain,
     36: NiceAiCondParameter.countPlayerNp,
     37: NiceAiCondParameter.countPlayerSkill,
     38: NiceAiCondParameter.countPlayerSkillIncludeMasterSkill,
     39: NiceAiCondParameter.totalTurn,
     40: NiceAiCondParameter.warBoardSquareIndividuality,
-    41: NiceAiCondParameter.checkBattleValue,
 }
 
 
 class AiRefineTarget(IntEnum):
     ANY = 0
     ALL = 1
     HIGHER = 2
@@ -4827,42 +4794,36 @@
     NONE = 0
     EQUAL = 1
     EQUAL_NOT = 2
     HIGHER = 3
     LOWER = 4
     MULTIPLE = 5
     EXIST = 6
-    BETWEEN = 7
-    BETWEEN_NOT = 8
 
 
 class NiceAiCondCheck(StrEnum):
     """Ai Condition Check"""
 
     none = "none"
     equal = "equal"
     equalNot = "equalNot"
     higher = "higher"
     lower_ = "lower"
     multiple = "multiple"
     exist = "exist"
-    between = "between"
-    betweenNot = "betweenNot"
 
 
 AI_COND_CHECK_NAME: dict[int, NiceAiCondCheck] = {
     0: NiceAiCondCheck.none,
     1: NiceAiCondCheck.equal,
     2: NiceAiCondCheck.equalNot,
     3: NiceAiCondCheck.higher,
     4: NiceAiCondCheck.lower_,
     5: NiceAiCondCheck.multiple,
     6: NiceAiCondCheck.exist,
-    7: NiceAiCondCheck.between,
-    8: NiceAiCondCheck.betweenNot,
 }
 
 
 class TreasureDeviceEffectFlag(IntEnum):
     SUPPORT = -1
     ATTACK_ENEMY_ALL = 1
     ATTACK_ENEMY_ONE = 2
@@ -5585,31 +5546,7 @@
     1: NiceSvtDeadType.escape,
     2: NiceSvtDeadType.stand,
     3: NiceSvtDeadType.effect,
     4: NiceSvtDeadType.wait,
     5: NiceSvtDeadType.energy,
     6: NiceSvtDeadType.crystal,
 }
-
-
-class AiAllocationSvtFlag(IntEnum):
-    ALL = 0
-    OWN = 1
-    FRIEND = 2
-    NPC = 4
-
-
-class NiceAiAllocationSvtFlag(StrEnum):
-    """AI Allocation Svt Flag"""
-
-    all = "all"
-    own = "own"
-    friend = "friend"
-    npc = "npc"
-
-
-AI_ALLOCATION_SVT_FLAG_NAME: dict[int, NiceAiAllocationSvtFlag] = {
-    0: NiceAiAllocationSvtFlag.all,
-    1: NiceAiAllocationSvtFlag.own,
-    2: NiceAiAllocationSvtFlag.friend,
-    4: NiceAiAllocationSvtFlag.npc,
-}
```

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/nice.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     StageLimitActType,
     SvtClass,
 )
 from .gameenums import (
     NiceAiActNum,
     NiceAiActTarget,
     NiceAiActType,
-    NiceAiAllocationSvtFlag,
     NiceAiCond,
     NiceBattleFieldEnvironmentGrantType,
     NiceBuffType,
     NiceCardType,
     NiceClassBoardSkillType,
     NiceClassBoardSquareFlag,
     NiceCombineAdjustTarget,
@@ -2466,20 +2465,14 @@
     id: int
     type: NiceBattleFieldEnvironmentGrantType
     priority: int
     individuality: list[NiceTrait]
     imageId: int
 
 
-class NiceAiAllocation(BaseModelORJson):
-    aiIds: list[int]
-    individuality: NiceTrait
-    applySvtType: list[NiceAiAllocationSvtFlag]
-
-
 class NiceStage(BaseModelORJson):
     wave: int
     bgm: NiceBgm
     startEffectId: int
     fieldAis: list[FieldAi] = []
     call: list[int] = Field([], title="Summon these NPC IDs")
     enemyFieldPosCount: int | None = None
@@ -2488,15 +2481,14 @@
     limitAct: StageLimitActType | None = Field(
         None, title="Action after turn countdown is over"
     )
     battleBg: NiceBattleBg | None = None
     NoEntryIds: list[int] | None = None
     waveStartMovies: list[NiceStageStartMovie] = []
     cutin: NiceStageCutIn | None = None
-    aiAllocations: list[NiceAiAllocation] | None = None
     originalScript: dict[str, Any]
     enemies: list[QuestEnemy] = []
 
 
 class NiceQuestMessage(BaseModelORJson):
     idx: int
     message: str
@@ -2600,35 +2592,30 @@
     detail: QuestEnemy | None = None
     aiIds: list[int]
 
 
 class NiceQuestPhaseOverwriteEquipSkill(BaseModelORJson):
     lv: int
     id: int
-    condId: int | None = None
 
 
 class NiceQuestPhaseOverwriteEquipSkills(BaseModelORJson):
-    iconId: int | None = None
-    cutInView: int | None = None  # 1: ShowMasterSkillCutIn
-    notDispEquipSkillIconSplit: int | None = None
+    iconId: int
     skills: list[NiceQuestPhaseOverwriteEquipSkill]
 
 
 class NiceQuestPhaseExtraDetail(BaseModelORJson):
     questSelect: list[int] | None = None
     singleForceSvtId: int | None = None
     hintTitle: str | None = None
     hintMessage: str | None = None
     aiNpc: NiceQuestPhaseAiNpc | None = None
     aiMultiNpc: list[NiceQuestPhaseAiNpc] | None = None
     overwriteEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
-    addEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
     waveSetup: int | None = None  # U Olga Marie Quest
-    interruptibleQuest: int | None = None
     masterImageId: int | None = None
 
 
 class NiceRestriction(BaseModelORJson):
     id: int
     name: str
     type: NiceRestrictionType
```

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/raw.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/rayshift.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/fgo_api_types/search.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.23.19.35.59/pyproject.toml` & `fgo_api_types-2024.4.6.2.22.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.04.23.19.35.59"
+version = "2024.04.06.02.22.03"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.4.23.19.35.59/PKG-INFO` & `fgo_api_types-2024.4.6.2.22.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.4.23.19.35.59
+Version: 2024.4.6.2.22.3
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


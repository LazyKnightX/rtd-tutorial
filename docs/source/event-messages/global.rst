================
全局事件 | enums.msg
================

----------------
游戏事件 | enums.msg.game
----------------

游戏启动 | enums.msg.game_boot
----------------

参数：

    ()

游戏开始 | enums.msg.game_start
----------------

参数：

    ()

游戏超出缓冲时间 | enums.msg.game_out_of_buffer_time
----------------

参数：

    ()

游戏模式选择完成 | enums.msg.game_mode_selected
----------------

参数：

    (id: integer)

游戏难度选择完成 | enums.msg.game_diff_selected
----------------

参数：

    (id: integer)

游戏英雄选择完成 | enums.msg.game_hero_selected
----------------

参数：

    (plr: cls_player, gid_s: string)

----------------
单位事件 | enums.msg.unit
----------------

单位进入地图 | enums.msg.unit_enter_map
----------------

参数：

    (u: cls_unit)

单位出生 | enums.msg.unit_birth
----------------

参数：

    (u: cls_unit)

单位死亡 | enums.msg.unit_die
----------------

参数：

    (u: cls_unit, u_killer)

单位被摧毁 | enums.msg.unit_destroy
----------------

参数：

    (u: cls_unit)

单位复活 | enums.msg.unit_revive
----------------

参数：

    (u: cls_unit)

单位提升等级 | enums.msg.unit_levelup
----------------

参数：

    (u: cls_unit, plr: cls_player, changed_levels: integer)

单位击杀敌人 | enums.msg.unit_kill
----------------

参数：

    (u: cls_unit, u_die: cls_unit)

单位攻击敌人 | enums.msg.unit_attack
----------------

参数：

    (u: cls_unit, u_attacked: cls_unit)

单位被攻击 | enums.msg.unit_attacked
----------------

参数：

    (u: cls_unit, u_attack: cls_unit)

单位造成伤害前演算伤害 | enums.msg.unit_damage_calc
----------------

在事件内直接修改 data.damage 可以修改最终伤害值

参数：

    (u: cls_unit, u_damaged: cls_unit, data: damage_event_data)

单位造成伤害 | enums.msg.unit_damage
----------------

警告：不要在这个事件里改变伤害数值

参数：

    (u: cls_unit, u_damaged: cls_unit, data: damage_event_data)

单位受到伤害前演算伤害 | enums.msg.unit_damaged_calc
----------------

在事件内直接修改 data.damage 可以修改最终伤害值

参数：

    (u: cls_unit, u_damage_source: cls_unit, data: damage_event_data)

单位受到伤害 | enums.msg.unit_damaged
----------------

警告：不要在这个事件里改变伤害数值

参数：

    (u: cls_unit, u_damage_source: cls_unit, data: damage_event_data)

单位被点击 | enums.msg.unit_clicked
----------------

参数：

    (u: cls_unit, plr: cls_player)

单位被取消点击 | enums.msg.unit_clicked_off
----------------

参数：

    (u: cls_unit, plr: cls_player)

单位获得技能 | enums.msg.unit_gain_skill
----------------

参数：

    (u: cls_unit, skl: cls_skill)

单位失去技能 | enums.msg.unit_drop_skill
----------------

参数：

    (u: cls_unit, skl: cls_skill)

单位获得技能卡 | enums.msg.unit_gain_skill_card
----------------

参数：

    (u: cls_unit, key: string, card: cls_skill_card)

单位失去技能卡 | enums.msg.unit_drop_skill_card
----------------

参数：

    (u: cls_unit, key: string, card: cls_skill_card)

单位使用技能卡 | enums.msg.unit_use_skill_card
----------------

参数：

    (u: cls_unit, index: integer)

单位获得英雄卡 | enums.msg.unit_gain_hero_card
----------------

参数：

    (u: cls_unit, key: string, card: cls_hero_card)

单位失去英雄卡 | enums.msg.unit_drop_hero_card
----------------

参数：

    (u: cls_unit, key: string, card: cls_hero_card)

单位使用英雄卡 | enums.msg.unit_use_hero_card
----------------

参数：

    (u: cls_unit, index: integer)

单位获得物品 | enums.msg.unit_gain_item
----------------

参数：

    (u: cls_unit, itm: cls_item)

单位失去物品 | enums.msg.unit_drop_item
----------------

参数：

    (u: cls_unit, itm: cls_item)

单位摧毁物品 | enums.msg.unit_destroy_item
----------------

参数：

    (u: cls_unit, itm: cls_item)

单位使用物品 | enums.msg.unit_use_item
----------------

参数：

    (u: cls_unit, itm: cls_item)

单位移动物品 | enums.msg.unit_move_item
----------------

参数：

    (u: cls_unit, itm: cls_item, slot: integer)

单位右键双击物品 | enums.msg.unit_double_click_item_right
----------------

参数：

    (u: cls_unit, itm: cls_item)

单位发布点目标指令 | enums.msg.unit_issue_order_point
----------------

参数：

    (u: cls_unit, point: cls_point, order, order_id)

单位开始被建造 | enums.msg.unit_build_start
----------------

参数：

    (u: cls_unit)

单位完成被建造 | enums.msg.unit_build_finish
----------------

参数：

    (u: cls_unit)

单位注意到攻击目标 | enums.msg.unit_acquired_target
----------------

参数：

    (u: cls_unit, u_target: cls_unit)

单位使用治疗药水F | enums.msg.unit_use_heal_potion_F
----------------

参数：

    (u: cls_unit)

单位发动技能效果 | enums.msg.unit_cast_skill_effect
----------------

参数：

    (u: cls_unit, gid_s: string)

----------------
单位 (马甲) | enums.msg.dummy
----------------


马甲造成伤害 | enums.msg.dummy_damage
----------------

参数：

    (u: cls_unit, u_damaged: cls_unit)

----------------
单位 (召唤物) | enums.msg.summoned
----------------

召唤物出生 | enums.msg.summoned_birth
----------------

参数：

    (u: cls_unit)

召唤物死亡 | enums.msg.summoned_die
----------------

参数：

    (u: cls_unit, u_killer: cls_unit)

召唤物复活 | enums.msg.summoned_revive
----------------

参数：

    (u: cls_unit)

----------------
刷怪 | enums.msg.atkwave
----------------

进攻波次-波次来临 | enums.msg.atkwave_wave
----------------

参数：

    (wave)

进攻波次-最后一波刷完 | enums.msg.atkwave_final
----------------

参数：

    ()

进攻波次-刷出单个怪物并应用属性时 | enums.msg.atkwave_spawn_monster___apply_attr
----------------

参数：

    (u: cls_unit, info: atkwave_river4_spawn_apply_attr_info)

----------------
系统 | enums.msg.sys
----------------

单位演算暴击前 (before) | enums.msg.sys_dmg_calc_crit_before
----------------

参数：

    (u_source: cls_unit, u_target: cls_unit, data: damage_crit_data)

单位演算伤害流程结束 | enums.msg.sys_dmg_calc_finish
----------------

参数：

    (u_source: cls_unit, u_target: cls_unit, data: damage_event_data)

单位伤害流程结束 | enums.msg.sys_dmg_finish
----------------

参数：

    (u_source: cls_unit, u_target: cls_unit, data: damage_event_data)

基地受到伤害 | enums.msg.sys_base_damaged
----------------

参数：

    (u_base: cls_unit, u_damage_source: cls_unit)

基地死亡 | enums.msg.sys_base_die
----------------

参数：

    (u_base: cls_unit, u_damage_source: cls_unit)

游戏逻辑帧更新 (0.1s) | enums.msg.sys_tick
----------------

参数：

    ()

游戏渲染帧更新 (1/60s) --TODO remove -> 真正的渲染帧在 hardware | enums.msg.sys_fps
----------------

参数：

    ()

游戏时间更新 | enums.msg.sys_past_time
----------------

参数：

    (past_time)

游戏时间更新 (半秒) | enums.msg.sys_past_time_half
----------------

参数：

    (past_time)

----------------
玩家 | enums.msg.player
----------------

玩家发送聊天信息 | enums.msg.player_chat
----------------

参数：

    (plr: cls_player, msg: string)

玩家按下键盘按键 | enums.msg.player_keyboard_down
----------------

参数：

    (plr: cls_player, key) - key: KEY - KEY.*

玩家抬起键盘按键 | enums.msg.player_keyboard_up
----------------

参数：

    (plr: cls_player, key) - key: KEY - KEY.*

玩家离开游戏 | enums.msg.player_leave_game
----------------

参数：

    (plr: cls_player)

玩家胜利 | enums.msg.player_win
----------------

参数：

    (plr: cls_player)

玩家失败 | enums.msg.player_fail
----------------

参数：

    (plr: cls_player)

玩家成长装备初始化 | enums.msg.growth_equip_init
----------------

参数：

    (plr: cls_player, itm: cls_item, u: cls_unit)

玩家成长装备升级 | enums.msg.growth_equip_upgrade
----------------

参数：

    (plr: cls_player, itm: cls_item, u: cls_unit)

玩家成长装备进阶 | enums.msg.growth_equip_promote
----------------

参数：

    (plr: cls_player, itm: cls_item, u: cls_unit)

玩家购买技能书 | enums.msg.player_buy_skill_book
----------------

参数：

    (plr: cls_player, itm: cls_item)

玩家使用英雄卡 | enums.msg.player_use_hero_card
----------------

参数：

    (plr: cls_player, name: string) - name: 英雄卡名称

玩家购买物品 | enums.msg.player_buy_item
----------------

参数：

    (plr: cls_player, itm: cls_item)

----------------
英雄 | enums.msg.hero - 特指玩家英雄
----------------

玩家英雄进入练功房 | enums.msg.hero_enter_troom
----------------

参数：

    (hero: cls_unit, plr: cls_player, troom_id: integer)

玩家英雄离开练功房 | enums.msg.hero_leave_troom
----------------

参数：

    (hero: cls_unit, plr: cls_player, troom_id: integer)

玩家英雄进入自己的练功房 | enums.msg.hero_enter_troom_self
----------------

参数：

    (hero: cls_unit, plr: cls_player)

玩家英雄离开自己的练功房 | enums.msg.hero_leave_troom_self
----------------

参数：

    (hero: cls_unit, plr: cls_player)

玩家英雄进入别人的练功房 | enums.msg.hero_enter_troom_other
----------------

参数：

    (hero: cls_unit, plr: cls_player)

玩家英雄离开别人的练功房 | enums.msg.hero_leave_troom_other
----------------

参数：

    (hero: cls_unit, plr: cls_player)

玩家英雄提升等级 | enums.msg.hero_levelup
----------------

参数：

    (hero: cls_unit, plr: cls_player, changed_levels: integer) | changed_levels - 提升的等级数量

玩家英雄提升等级前 | enums.msg.hero_levelup_before
----------------

参数：

    (hero: cls_unit, plr: cls_player, changed_levels: integer) | changed_levels - 提升的等级数量

----------------
硬件 | enums.msg.hardware
----------------

enums.msg.hardware_mouse_enter_skill_slot
----------------

async 异步事件

enums.msg.hardware_mouse_leave_skill_slot
----------------

async 异步事件

enums.msg.hardware_mouse_enter_item_slot
----------------

async 异步事件

enums.msg.hardware_mouse_leave_item_slot
----------------

async 异步事件

enums.msg.hardware_mouse_enter_item
----------------

async 异步事件

enums.msg.hardware_mouse_leave_item
----------------

async 异步事件

enums.msg.hardware_mouse_enter_unit
----------------

async 异步事件

enums.msg.hardware_mouse_leave_unit
----------------

async 异步事件

鼠标滚轮滑动 | enums.msg.hardware_mouse_wheel_delta
----------------

async 异步事件

参数：

    (b_forward: boolean)

enums.msg.hardware_console_update
----------------

async 异步事件

enums.msg.hardware_frame_update
----------------

async 异步事件

取消选择单位 (Real Select Unit) | enums.msg.hardware_deselect_unit
----------------

async 异步事件

参数：

    (player_self: cls_player, unit: cls_unit)

选择单位 (Real Select Unit) | enums.msg.hardware_select_unit
----------------

async 异步事件

参数：

    (player_self: cls_player, unit: cls_unit)

清除选择单位 (Real Select Unit) | enums.msg.hardware_select_unit_clean
----------------

async 异步事件

参数：

    (player_self: cls_player)

----------------
物品 | enums.msg.item
----------------

物品被创建 | enums.msg.item_create
----------------

参数：

    (itm: cls_item)

物品被摧毁 | enums.msg.item_destroy
----------------

参数：

    (itm: cls_item)

物品被拾取 | enums.msg.item_gain
----------------

参数：

    (itm: cls_item)

物品被丢弃 | enums.msg.item_drop
----------------

参数：

    (itm: cls_item)

物品被使用 | enums.msg.item_use
----------------

参数：

    (itm: cls_item)

----------------
爬塔 | enums.msg.tower
----------------

爬塔挑战成功 | enums.msg.tower_clg_success
----------------

参数：

    (plr: cls_player, id: integer)

爬塔挑战失败 | enums.msg.tower_clg_failed
----------------

参数：

    (plr: cls_player, id: integer)

----------------
回收 | enums.msg.recycle
----------------

回收物品 | enums.msg.recycle_item
----------------

参数：

    (itm: cls_item)

----------------
头目死亡 | enums.msg.bossdie
----------------

进攻波次BOSS死亡 | enums.msg.bossdie_atkwave
----------------

参数：

    ()

转生BOSS死亡 | enums.msg.bossdie_promote
----------------

参数：

    ()

----------------
商店 | enums.msg.store
----------------

商店出售物品（消费前） | enums.msg.store_sell_item_consume
----------------

@see enums.msgu.buy_store_item_consume

参数：

    (store: cls_unit, sold_to: cls_unit, consume_data: consume_event_data)

----------------
单位事件 | enums.msg.unit
----------------

单位攻击敌人 | enums.msgu.unit_attack
----------------

参数：

    (u: cls_unit, u_attacked: cls_unit)

单位被攻击 | enums.msgu.unit_attacked
----------------

参数：

    (u: cls_unit, u_attacker: cls_unit)

单位发布点目标指令 | enums.msgu.unit_issue_order_point
----------------

参数：

    (u: cls_unit, point: cls_point, order: string, order_id: integer)

单位死亡 | enums.msgu.unit_die
----------------

参数：

    (u: cls_unit, u_killer: cls_unit)

单位提升等级 | enums.msgu.unit_levelup
----------------

参数：

    (u: cls_unit, plr: cls_player, levels: integer)

单位击杀敌人 | enums.msgu.unit_kill
----------------

参数：

    (u: cls_unit, u_die: cls_unit)

单位被摧毁 (回收) | enums.msgu.unit_destroy
----------------

参数：

    (u: cls_unit)

单位复活 | enums.msgu.unit_revive
----------------

参数：

    (u: cls_unit)

马甲造成伤害 | enums.msgu.dummy_damage
----------------

参数：

    (u: cls_unit, u_damaged: cls_unit)

单位造成伤害前演算伤害 | enums.msgu.unit_damage_calc
----------------

在事件内直接修改 data.damage 可以修改最终伤害值

参数：

    (u: cls_unit, u_damaged: cls_unit, data: damage_event_data)

单位造成伤害 | enums.msgu.unit_damage
----------------

警告：不要在这个事件里改变伤害数值

参数：

    (u: cls_unit, u_damaged: cls_unit, data: damage_event_data)

单位受到伤害前演算伤害 | enums.msgu.unit_damaged_calc
----------------

在事件内直接修改 data.damage 可以修改最终伤害值

参数：

    (u: cls_unit, u_damage_source: cls_unit, data: damage_event_data)

单位受到伤害 | enums.msgu.unit_damaged
----------------

警告：不要在这个事件里改变伤害数值

参数：

    (u: cls_unit, u_damage_source: cls_unit, data: damage_event_data)

单位双重施法 | enums.msgu.unit_double_cast
----------------

参数：

    (u: cls_unit, result: boolean)

单位格挡 | enums.msgu.unit_block
----------------

参数：

    (u: cls_unit, result: boolean)

单位被点击 | enums.msgu.unit_clicked
----------------

参数：

    (u: cls_unit, plr: cls_player)

单位被取消点击 | enums.msgu.unit_clicked_off
----------------

参数：

    (u: cls_unit, plr: cls_player)

玩家英雄提升等级 | enums.msgu.hero_levelup
----------------

参数：

    (hero: cls_unit, plr: cls_player, levels: integer) - levels - 提升的等级数量

玩家英雄提升等级前 | enums.msgu.hero_levelup_before
----------------

参数：

    (hero: cls_unit, plr: cls_player, levels: integer) - levels - 提升的等级数量

单位注意到攻击目标 | enums.msgu.unit_acquired_target
----------------

参数：

    (u: cls_unit, u_target: cls_unit)

伤害流程结束 (source as listener) | enums.msgu.sys_dmg_finish___source
----------------

参数：

    (u_source: cls_unit, u_target: cls_unit, data: damage_event_data)

伤害流程结束 (target as listener) | enums.msgu.sys_dmg_finish___target
----------------

参数：

    (u_target: cls_unit, u_source: cls_unit, data: damage_event_data)

购买商店物品（消费前） | enums.msgu.buy_store_item_consume
----------------

参数：

    (store: cls_unit, consume_data: consume_event_data, info: ItemSellDataInfo)

单位使用终极技能 | enums.msgu.cast_final_skill
----------------

参数：

    ()

单位使用治疗药水F | enums.msgu.unit_use_heal_potion_F
----------------

参数：

    (u: cls_unit)

单位发动技能效果 | enums.msgu.unit_cast_skill_effect
----------------

参数：

    (u: cls_unit, gid_s: string)

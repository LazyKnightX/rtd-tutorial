Sample
============================

..  toctree::
    :maxdepth: 2
    :caption: 对象属性

    /object-attributes/index

..  toctree::
    :maxdepth: 2
    :caption: 游戏事件

    /event-messages/index

数据类型
----------------------------

**动态整数 Dynamic Integer**

动态整数：根据输入的玩家不同而有可能有不同返回值的整数。

..  code-block:: lua
    @alias dynamic_integer integer|fun(plr: cls_player):integer
    method: read_dynamic_integer

**访问KEY Access Key**

访问KEY：可能为整数也可能为字符串的字典KEY。

..  code-block:: lua
    @alias access_key integer|string

**固定Tip Stable Tip**

固定Tip：预设的、固定槽位的Tip。

..  code-block:: lua
    --@hook stable-tip


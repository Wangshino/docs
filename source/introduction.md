title: 介绍
---------

## What kind of game is Screeps

Screeps is a massive multiplayer online real-time strategy game. Each player can create his or her own colony in a **single persistent world** shared by all the players. Such a colony can mine **resources**, build **units**, conquer **territory**. As you conquer more territory, your influence in the game world grows, as well as your abilities to expand your footprint. However, it requires a lot of effort on your part, since multiple players may aim at the same territory.


## 关于Screeps
Screeps 是一款 MMO RTS 游戏，每个玩家都可以在同一个单一持久的游戏世界中，创造属于自己的领地。在领地中，你可以开采矿物，建造单位，开拓疆土。当你开拓了更广阔的疆土，你的影响力和能力会随着你开拓疆土的脚步逐步扩大。然而，暗中潜伏的敌人也会看上你的领地，你需要付出更多的精力用来巩固自己的领土。

Screeps is developed for people with **programming skills**. Unlike some other RTS games, your units in Screeps can react to events without your participation – provided that you have programmed them properly. And, unlike other MMO, you do not have to play Screeps constantly to play well. It is quite enough just to check once in a while to see if everything goes well.

Screeps 是一个针对拥有编程能力的群体开发的。不同于其他 RTS 游戏，只要你提供了正确的代码，你的单位可以在你没有参与的情况下作出反应。并且也不同于其他的 MMO 游戏，你不必一直保持在线，只需要偶尔上去看一下是否一切运转正常即可。

## 游戏世界观

The game world consists of interconnected **rooms**. A room is a closed space 50x50 cells in size. It may have 1-4 exits to other rooms. A number of rooms in the world is limited, but increases as new players join the game. So the single game world is really huge and constantly expanding, like the Universe itself.

游戏中的世界包含着许多个房间。一个房间是一个由50x50格子的组成的封闭空间。每一个房间可能有1-4个通往其他房间的出口，房间的总数是有限制的，但是房间的数量会随着新玩家的加入而增加。所以这个单一游戏世界像宇宙一样的庞大并且持续增长。

[![](img/world-map.png)](http://static.screeps.com/map.png)

[Download full map image](http://static.screeps.com/map.png) (9100x9100 PNG, 17.7 MB)

Each room landscape is unique. The view of each room is generated procedurally and consists of three types of surface:

每一个房间都是独一无二的，所有房间会生成三种类型的表面:

*   **平原** – 移动力消耗为2的普通土地。
*   **沼泽** - 移动力消耗为10。
*   **墙壁** - 所有单位不能通过。

你可以使用下面给出的设施来改变房间的地形：

*   **道路** 在道路上消耗的移动力为1。 道路会随着使用次数的增加而损坏，但可以修理。
*   **墙壁** 墙可以被人为建造。不同于原生存在的墙，人造墙可以被小兵破坏和摧毁。
*   **堡垒** 是你的防御设施。只有你的小兵可以进入堡垒。此外，进入堡垒的小兵不可以被攻击，除非堡垒被摧毁。（尽管它可以攻击别人）。堡垒在每个游戏时钟周期会有损坏，需要持续修理。

在刚进入游戏时，你可以免费选择一个可以使用的区域建造你的初始殖民地。在你的第一个主基地建造之后，你所在的房间会进入安全模式，用这段时间巩固自己的防御，不然任何玩家都可以毁灭你的殖民地。


## 殖民地

**![](img/colony-center.png)**

**能源** 是这个世界中最重要的资源之一。能源可以被小兵开采。每个能源点的产出是有限的，但是在每三百个游戏周期时钟会恢复。

**基地** 基地是你殖民地的中心。基地可以收集开采的能源，并且使用能源建造单位。一个房间里不能超过3个基地，所以，当一个房间里你如果有3个基地的话，你就完全占领了一个房间。尽管如此，在你控制的房间中，你仍然可以拥有多个基地。

一个基地只能建造最基本的单位，如果你需要建造更加复杂的单位，你可以在基地上建造**拓展组件**。
在一下节中，会有对此的详细介绍。

A spawn itself can build only basic units. In order to build more complex ones, you have to construct one or more spawn **extensions**. Read more about that in the next article.

.. _h2c3f2925614a6b706a49586d6334e:

ACFinger
########

.. _hb79795d3e46b47696c7c5b6d3a41e:

Introduction
************

ACFinger is an MacOS application to rescue our fingers and health. It helps to count how many keyboard strokes for every fingers. With statistic charts from counting, we would have better idea about fingers care. We would also have better balance of working and relaxing.

.. _h6897050511836763421463e2b4b685:

Features
********

#. Counting strokes and their distribution in time for every fingers.

#. Chart of strokes by fingers and by time.

#. Chart of hitting-speed for fingers.

.. _h207a62d776879664a3fd11584e807f:

Left/Right - How many touches made by every fingers
===================================================

Chart1: Total touches for every hours. 

Chart2: Total touches of every fingers in a given hour.

Usages:

#. Knowing that if you are torturing your fingers.

#. Which fingers are mostly used.

.. _h47284c6d511a2cee7756625f61762:

Speed - How fast are you typing
===============================

Chart1: Maximum and average speed in "touches per minute" for every hours.

Chart2: Maximum and minimum speed in a given hour.

Usages:

#. Knowing that if you are torturing your fingers.

#. Knowing how fast are your tendons stretching and shrinking.

.. _h2f47553d312e828565f5363167339:

Balance - How balance between your right and left fingers
=========================================================

Chart1: Touches by right/left fingers for every hours.

Chart2: Proportion of right to left fingers for a given hour.

.. _h3976135538341a87f293655287581c:

Working/Relaxing 
=================

This measure is for helping you not to work too much. By watching keyboard activity, the app calculates your accumulated continuous working time and relaxing time. It would help you to have better idea on how to improve your health.

Chart 1: Accumulated working time and relaxing time in a day.

Chart 2: Proportion of working to relaxing for a given moment.

.. _h3839cd5c27d27979386951331f28:

Body Power
==========

假設：

    每天早上初始狀態是100％（類似電力100）

    最長連續工作時間是50分鐘，消耗80％的電力。

    警戒值自動設定為20％（100 - 80）

    則每個工作分鐘消耗率是80/50 = 1.6%,

    過度工作，仍繼續消耗到0為止，低於0仍然是0

    最短連續休息時間是10分鐘，可恢復80％的電力，

    則每個休息分鐘恢復率是80/10 = 8%，超過100％仍算100％

目標：

一、工作的時候，電力會消耗，休息的時候，電力充回來

二、超時工作的時候，電力低於警戒值，會顯示紅色

.. _h194a2a535534212f506e5031782e44b:

Stage Animation
***************

.. _h15631b70527c72177371b506c7f507e:

Configurations
**************

* Show body power or key touches count

* Show or hide stage animation

* Working/Relaxing

    * Minimum touches in a minute to count as a working time. If number of touches in a given minute is bigger than this number, that minute is a working minute. Otherwise it is a relaxing minute.

    * Minimum continuous minutes to count as a relaxing time. If number of continuous relaxing minutes is bigger that this number, that interval would contribute to relaxing time, otherwise it is stil contributing to working time. If this number is 0, which mean every relaxing minute contributes to accumulated relaxing time.


.. bottom of content

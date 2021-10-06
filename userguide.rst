
.. _h7a6941666312412f5d33487d7c4f3d7:

User Guide
##########

Health is simply belance between working and taking break. This app is mainly for office workers who are sitting on computer all day long. This app help them to be aware of their own working and break tempo. By managing balance, they are able to keep healthy and productive for their careers.

.. _h24263c4b755f1b4e49342c321267514d:

Synopsis
********

.. _h1f7e585de5397451c6b6391b7a0:

Terminology
***********

.. _h373c2b1564c323c6d545e4952435b25:

Working Minute and Break Minute
===============================

\ |IMG1|\ 

The Typing Counter takes a minute as a working minute or a break minute by a threshold value (default to 5 keystrokes).  For a minute with keystrokes count over the threshold value, it is a working minute. Otherwise it is a break minute.

.. _h372630646e56301561a1a371134181b:

Break Interval
==============

\ |IMG2|\ 

A working interval is a continuous chunk of working minutes. But the Typing Counter recognizes a continuous chunk of break minutes as a break interval only if its length is more than a threshold value (default to 10 minutes). If its length is less than the threshold value. The Typing Counter takes it as a working interval. This is for encouraging you to have enough time for a break.

.. _h7d27c1759465b14283e39615c302058:

Overworking Interval
====================

\ |IMG3|\ 

The Typing Counter checks length of every continuous working interval. If its length is longer than a threshold value (default to 50 minutes), The Typing Counter takes those exceeding minutes as an overworking interval. 

.. _h286272113e3f7c2f29363693b2f42:

Power Calculation
=================

\ |IMG4|\ 

Human body is like a battery. It looses power during working interval and restores power back by taking breaks. The Typing Counter considers your body power as a score from 0% to 100%. At day beginning, your power is set to 100%. Alone with you are working, your power has reduced. You have to take breaks for restoring power. There is an expenditure value (defaults to 80%) associates with the maximum working interval (defaults to 50 minutes), which also implies the reducing rate (1.6% per working minute) as well as the charging rate (8% per break minute).

\ |IMG5|\ 

By the default reducing rate. Your power score would become zero after overworking for 12.5 minutes.

\ |IMG6|\ 

The power lose in a maximum working interval would be totally recovered after a minimum break interval. That is to say, if you work for 50 minutes and take a break for 10 minutes, your power score would be 100% again. The charging rate is 8% per break minute under default values.

.. _h7015777b347a33c5e481931d625040:

Tabs
****

.. _h431d5061723751203410681c45363038:

Stress
======

This is a diagram of keypress count by left and right fingers.

\ |IMG7|\ 

This diagram reads:

At 13:43, your left fingers has pressed keyboard for 6,568 times.  And your right fingers has pressed keyboard for 8,469 times.

--------

\ |IMG8|\ 

This diagram reads:

In number of 6,568 keypress by your left fingers, litter finger(L5) counts 853, ring finger(L4) counts 1,725, middle finger(L3) counts 2,125, forefinger counts 1,864 and thumb(L1) counts 0. 

In number of 8,496 keypress by your right fingers, thumb(R1) counts 1,420, forefinger(R2) counts 3,193, middle finger(R3) counts 794, ring finger(R4) counts 1,091 and little finger(R5) counts 1,998.

From 0:00 to 13:43, your left middle finger and right forefinger are mostly hard-working fingers.

.. _h2c1d74277104e41780968148427e:




You can read more information from this kind of diagram. For example: A casual day would be like this below. It has smooth lines.

\ |IMG9|\ 

But for this diagram below:

.. _h73207a20436b676b595165b4e243d46:

\ |IMG10|\ ===========

This reads that you start typing on your computer around AM8:00, and you are very hard working, almost without any break till 12:00. Maybe you are in an unusually emergent state or you have to adjust working-behavior for better health.

.. _h67588282f612229e44437f7063305:

Balance
=======

This tab shows your balance of working and break. 

\ |IMG11|\ 

This diagram reads:  from 7:48 to 22:46, you spent 9 hours and 34 minutes for working, 5 hours and 24 minutes for break. In all of working time, 49% (aka 4 hours and 41 minutes) is overworking. It's not good.

Below the chart, a color bar shows break/working/overworking tempo. Green section is break interval, blue section is working interval and dark blue section is  overworking interval.

\ |IMG12|\ 

At the lower part is a percentage comparison of working and break interval in total, aka "9hr 34m" vs. "5hr 24m". This diagram shows that you spent 64% for working and 36% for breaks from 07:48 to 22:46.

\ |IMG13|\ 

.. _h234f20346f3f70460477d1f5d2e7b22:

Power
=====

.. _h175e5034f3d2b2d704737456d2e7562:

Data Format
***********

Data is generated every minute an entry (row). Usually, recorded values are written in next minute. If the computer goes to sleep, recording duration is less than 1 minute but entry's timestamp is the time before sleeping, though that entry is written after computer has waken up.

.. _h1f544f2c4950c11396e127c3e292e3b:

Simple Format
=============

For every raw of a single file. Below is meaning for every column

+------+---------------------------------------------------------------------------------------------------------------------------------+
|Column|Meaning                                                                                                                          |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|0     |Timestamp, this is the time of recording start.                                                                                  |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|1     |counts of unset (ignored) keys.                                                                                                  |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|2     |counts of left hand little finger (L5)                                                                                           |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|3     |counts of left hand ring finger (L4)                                                                                             |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|4     |counts of left hand middle finger (L3)                                                                                           |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|5     |counts of left hand index finger / forefinger (L2)                                                                               |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|6     |counts of left hand thumb (L1)                                                                                                   |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|7     |counts of right hand thumb (R1)                                                                                                  |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|8     |counts of right hand index finger / forefinger (R2)                                                                              |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|9     |counts of right hand middle finger (R3)                                                                                          |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|10    |counts of right hand ring finger (R4)                                                                                            |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|11    |counts of right hand little finger (R5)                                                                                          |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|12    |duration of unset keys (L5)                                                                                                      |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|13    |duration of left hand little finger (L5)                                                                                         |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|14    |duration of left hand ring finger (L4)                                                                                           |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|15    |duration of left hand middle finger (L3)                                                                                         |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|16    |duration of left hand index finger / forefinger (L2)                                                                             |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|17    |duration of left hand thumb (L1)                                                                                                 |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|18    |duration of right hand thumb (R1)                                                                                                |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|19    |duration of right hand index finger / forefinger (R2)                                                                            |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|20    |duration of right hand middle finger (R3)                                                                                        |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|21    |duration of right hand ring finger (R4)                                                                                          |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|22    |duration of right hand little finger (R5)                                                                                        |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|23    |counts of left mouse button                                                                                                      |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|24    |counts of middle mouse button                                                                                                    |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|25    |counts of right mouse button                                                                                                     |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|26    |counts of composite keys (shift, control,...)                                                                                    |
+------+---------------------------------------------------------------------------------------------------------------------------------+
|27    |counts of hand moving from keyboard to mouse. (beliving this is very close to the counts of hand moving from mouse to keyboard). |
+------+---------------------------------------------------------------------------------------------------------------------------------+

Remarks:

#. "Empty String" value is 0.

#. If both "left mouse click" and "right mouse click" are mapping to "unset" . The field 27 is always 0.

.. _h7d4c3277791e387f322d4d676f136037:

Academic Format
===============

Since (part of) Keystroke Dynamic Studies are focusing on working fatigue recognition, we decide to support the academic format for helping on improving public health.

This format adds extra 25 fields for researches on Keystroke Dynamic. They are measured by the theoratical model below:

\ |IMG14|\ 

+--+-----------------------+
|28|Arithematic mean of  PH|
+--+-----------------------+
|29|Arithematic mean of  PP|
+--+-----------------------+
|30|Arithematic mean of  PR|
+--+-----------------------+
|31|Arithematic mean of  RP|
+--+-----------------------+
|32|Arithematic mean of  RR|
+--+-----------------------+
|33|Geometric mean of  PH  |
+--+-----------------------+
|34|Geometric mean of  PP  |
+--+-----------------------+
|35|Geometric mean of  PR  |
+--+-----------------------+
|36|Geometric mean of  RP  |
+--+-----------------------+
|37|Geometric mean of  RR  |
+--+-----------------------+
|38|Harmonic mean of  PH   |
+--+-----------------------+
|39|Harmonic mean of  PP   |
+--+-----------------------+
|40|Harmonic mean of  PR   |
+--+-----------------------+
|41|Harmonic mean of  RP   |
+--+-----------------------+
|42|Harmonic mean of  RR   |
+--+-----------------------+
|43|Sample size of PH      |
+--+-----------------------+
|44|Sample size of PP      |
+--+-----------------------+
|45|Sample size of PR      |
+--+-----------------------+
|46|Sample size of RP      |
+--+-----------------------+
|47|Sample size of RR      |
+--+-----------------------+

Remarks:

#. Field 28-39 are calculated by the same kind of keystrokes in a minute.

#. Special keys (mostly are composite keys), such as Shft, Control, Caplock, Command, Option/Alt are excluded from statistics.

#. Mouse clicks are excluded, too.

#. Because users might press next key before releasing the already pressed key, the sequence of key pressing and releasing could be press-press-release-release instead of press-release-press-release. It can be can be observed from Field 40-43. Usually, PR, RP and RR are of the same number, when it happened, RR would has different number from PP and RP. When it happened, these values are measured as blow:\ |IMG15|\ 

Visualization Key-Finger Mappings

\ |IMG16|\ 

#. Copy the raw data into clipboard.

#. Open browser to the Keyboard Layout Editor(KLE)

\ |IMG17|\ 

#. In KLE, from the menuitem "Preset", choose "Blank Layout" 

\ |IMG18|\ 

#. Paste the raw data into the blank textarea blow the tab "Raw data".


.. bottom of content

.. |IMG1| image:: static/User_Guide_1.png
   :height: 174 px
   :width: 420 px

.. |IMG2| image:: static/User_Guide_2.png
   :height: 306 px
   :width: 697 px

.. |IMG3| image:: static/User_Guide_3.png
   :height: 112 px
   :width: 520 px

.. |IMG4| image:: static/User_Guide_4.png
   :height: 226 px
   :width: 572 px

.. |IMG5| image:: static/User_Guide_5.png
   :height: 173 px
   :width: 609 px

.. |IMG6| image:: static/User_Guide_6.png
   :height: 186 px
   :width: 605 px

.. |IMG7| image:: static/User_Guide_7.png
   :height: 264 px
   :width: 377 px

.. |IMG8| image:: static/User_Guide_8.png
   :height: 294 px
   :width: 341 px

.. |IMG9| image:: static/User_Guide_9.png
   :height: 282 px
   :width: 428 px

.. |IMG10| image:: static/User_Guide_10.png
   :height: 284 px
   :width: 424 px

.. |IMG11| image:: static/User_Guide_11.png
   :height: 357 px
   :width: 413 px

.. |IMG12| image:: static/User_Guide_12.png
   :height: 120 px
   :width: 425 px

.. |IMG13| image:: static/User_Guide_13.png
   :height: 357 px
   :width: 405 px

.. |IMG14| image:: static/User_Guide_14.png
   :height: 352 px
   :width: 697 px

.. |IMG15| image:: static/User_Guide_15.png
   :height: 265 px
   :width: 568 px

.. |IMG16| image:: static/User_Guide_16.png
   :height: 292 px
   :width: 281 px

.. |IMG17| image:: static/User_Guide_17.png
   :height: 184 px
   :width: 221 px

.. |IMG18| image:: static/User_Guide_18.png
   :height: 77 px
   :width: 222 px

---
layout: post
title: GDB Debug With MCU
---

{{ page.title }}
================

<p class="meta">14 May 2015 - Leo Zhang</p>

* Print Register
This can be done with "print ((Sercom *)hw)->USART.CTRLA", use some pre-defined
Register macro, All bit or Byte value can be shown. But the enum value cannot
be resolved, still need some way TODO it.

(gdb) print ((Sercom *)hw)->USART.CTRLA 
$4 = {bit = {SWRST = 0, ENABLE = 0, MODE = 0, RUNSTDBY = 0, IBON = 0, SAMPR = 0, 
  TXPO = 0, RXPO = 0, SAMPA = 0, FORM = 0, CMODE = 0, CPOL = 0, DORD = 0}, 
  reg = 0}


* autoconf
http://www.laruence.com/2009/11/18/1154.html
--

[Online GDB Manual](http://www.gnu.org/software/gdb/documentation/) 
[Example](http://www.yolinux.com/TUTORIALS/src/dbinit_stl_views-1.03.txt)
[Example](http://www.opensource.apple.com/source/emacs/emacs-70/emacs/src/.gdbinit)

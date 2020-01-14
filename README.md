# 终端模拟器设置

## 配置文件

```
cat .Xresources

!-- for xterm configurations --
! xterm does not support transparency so you may like rxvt-unicode instead
!
! Setting xterm font with 'DejaVu Sans Mono Book', Note here Book is the font style
!
!xterm*faceName: DejaVu Sans Mono Book
!
! 'facesize' for font size
!
!xterm*faceSize: 11
!
! 'faceNameDoublesize' for double wide character only
! So xterm can show unicode chars with such setting.
!xterm*faceNameDoublesize: Noto Sans CJK SC:antialias=true:pixelsize=20
!
!-- rxvt-unicode --
! transparent setting
URxvt*transparent: true
! tranparent ratio
URxvt*shading:40
! set fonts! You can set many fonts here, font in font is used with high priority
URxvt*font: xft:DejaVu Sans Mono:style=Relular:pixalsize=10:antialias=true,\
	    xft:Noto Sans CJK SC:style=Relular:pixalsize=10:antialias=true
! charater space setting
URxvt*letterSpace: -1
! color setting
URxvt*background: Black
URxvt*foreground: White
! scroll setting
URxvt*scrollBar: true
URxvt*scrollBar_right: true
URxvt*saveLines: 12000
! Because 'ls' show dir cant see clearly so set new blue here
URxvt*color4: RoyalBlue
URxvt*color12: RoyalBlue
! set scrolltype: rxvt or next or plan or xterm
URxvt*scrollstyle: plain

URxvt*perl-ext-common: default,font-size
```
## 加载修改

```
xrdb -merge .Xresources
```


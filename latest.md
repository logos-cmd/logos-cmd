You first have to copy the code then paste it in [Logos](https://calormen.com/jslogo)

```
to \cmd_displayname :label :length
  cs
  ct
  hideturtle
  rt 90
  setlabelheight :length
  label :label
end
to \cmd_print :label
    cs
  ct
  hideturtle
  rt 90
  Print :label
end
to \cmd_wave
  cs
  ct
  hideturtle
  repeat 31 [print [1]wait 2]
  wait 3.25
 repeat 31 [print [2]wait 2]
  wait 3.25
  repeat 31 [print [3]wait 2]
  wait 3.25
  repeat 31 [print [4]wait 2]
End
to \cmd_square :length
  cs
  ct
  hideturtle
  repeat 4[fd :length rt 90]
end
to \cmd_pentagon :length
  cs
  ct
  hideturtle
  repeat 5[fd :length rt 72]
end
to \cmd_hexagon :length
  cs
  ct
  hideturtle
  repeat 6[fd :length rt 60]
end
to \cmd_decagon :length
  cs
   ct
  hideturtle
  repeat 10[fd :length rt 36]
end
to \cmd_hideturtle
  hideturtle
end
to \cmd_clearscreen
  clearscreen
end
to \cmd_cs
  cs
end
to \cmd_ct
  ct
end
to \cmd_cleartext
  cleartext
end
to \cmd_showturtle
  showturtle
end
to \cmd_logo :label :repcount :rt1
  
  repeat 144 [
    cmd_cleartext
    setlabelheight repcount
    penup
    fd repcount * repcount / :repcount
    label :label
    bk repcount * repcount / :repcount
    pendown
    rt :rt1
  ]
end
TO \cmd_setcolor :color
  setpc :color
end
to \cmd_fill :color
  pd
  setpc :color
  fill
end
to \cmd_resetcolor
   setcolor 0
End
to \cmd_help
  cs
  ct
  hideturtle
  print[=--= Help =--=]
  print[]
  print[\cmd_cs]
  print[\cmd_clearscreen]
  print[\cmd_ct]
  print[\cmd_cleartext]
  print[\cmd_displayname [name] number]
  print[\cmd_decagon length]
  print[\cmd_fill color]
  print[\cmd_help]
  print[\cmd_hexagon length]
  print[\cmd_hideturtle]
  print[\cmd_logo label number rt]
  print[\cmd_pentagon length]
  print[\cmd_resetcolor]
  print[\cmd_setcolor color]
  print[\cmd_showturtle]
  print[\cmd_square length]
  print[\cmd_wave]
  print[\move_fd length]
  print[\move_bk length]
  print[\move_rt length]
  print[\move_lt length]
  print[]
  print[Help Command]
  print[/help]
  print[/cmd_help]
end

to \help
  cs
  ct
  hideturtle
  print[=--= Help =--=]
  print[]
  print[\cmd_cs]
  print[\cmd_clearscreen]
  print[\cmd_ct]
  print[\cmd_cleartext]
  print[\cmd_displayname [name] number]
  print[\cmd_decagon length]
  print[\cmd_fill color]
  print[\cmd_help]
  print[\cmd_hexagon length]
  print[\cmd_hideturtle]
  print[\cmd_logo label number rt]
  print[\cmd_pentagon length]
  print[\cmd_resetcolor]
  print[\cmd_setcolor color]
  print[\cmd_showturtle]
  print[\cmd_square length]
  print[\cmd_wave]
  print[\move_fd length]
  print[\move_bk length]
  print[\move_rt length]
  print[\move_lt length]
  print[]
  print[Help Command]
  print[/help]
  print[/cmd_help]
end

to \move_fd :length
  fd :length
end

to \move_bk :length
  bk :length
end

to \move_rt :length
  rt :length
end

to \move_lt :length
  lt :length
end
```

@startgantt

printscale daily zoom 2
ganttscale daily
<style>
ganttDiagram {
  timeline {
    LineColor transparent
 }
}
arrow {
    LineStyle 1
    LineThickness 1
    LineColor blue
}
</style>

<style>
ganttDiagram {
task {
FontName Helvetica
FontColor blue
FontSize 12
PlantUML Language Reference Guide (1.2021.2) 268 / 415
16.18 Using style 16 GANTT DIAGRAM
FontStyle normal
BackGroundColor GreenYellow
LineColor blue
}
note {
FontColor DarkGreen
FontSize 10
LineColor OrangeRed
}
arrow {
FontName Helvetica
FontColor red
FontSize 12
FontStyle normal
BackGroundColor #0FF
LineColor blue
}
separator {
LineColor White
BackGroundColor Blue
FontSize 12
FontStyle bold
FontColor Yellow
}
}
</style>

Project starts 2021-10-27
today is colored in #CAF

'Closed days
sundays are closed
2021/11/01 is closed
2021/11/11 is closed

-- Pavel --
[112 Montare usi (4buc)] as [T112] lasts 4 days and is 0% completed
[105 Carrelage general 1er 2eme etage] as [T105] starts 2021-10-27 and lasts 2 days and is 0% completed
[14 Montage WC suspendu et 1 et 2] as [T14] starts 2021-11-26 and lasts 2 days and is 0% completed
[120 Repose 4 radiateurs] as [T120] starts 2021-10-29 and lasts 1 day

' ET1
[108 Scoatere geamuri bucatarie] as [T108] starts 2021-11-03 and lasts 1 days
[15 Ajout petit evier dans la chambre WC] as [T15] lasts 1 day
[122 Hotte cuisine] as [T122] starts 2021-11-02 and lasts 1 day
[Reparation apres montage plafonds fenetres living/cuisine] as [T999] lasts 1 day
[Poncage cuisine] as [T1000] lasts 1 day

'ET2
[118 Montage systeme pour roulleaux fenetres] as [T118] lasts 1 day and starts 2021-10-30
[119 Poncage SDB] as [T119] starts 2021-10-27 and lasts 1 day
[110 Montage radiateur SDB] as [T110] starts 2021-10-29 and lasts 1 day
[121 Cada ilot] as [T121] lasts 2 days
[105.2 Carrelage SDB finalizat] as [T105.2] lasts 1 day
[Usa glisanta] as [T998] starts 2021-10-28 and lasts 2 days

'ET3
[123 Reparation Infiltration Grenier] as [T123] starts 2021-10-27 and lasts 2 days

-- Dan & Pavel --
[83 Montage vasque et mobilier SDB] as [T83] lasts 1 day
[117 Montage mobilier cuisine] as [T117] lasts 1 day

-- Dan & Monica --
[992 Peinture cuisine] as [T992] lasts 1 day
[993 Peinture living] as [T993] starts 2021-11-04 and lasts 1 day
[994 Peinture SDB] as [T994] starts 2021-11-02 and lasts 2 day
[996 Parquet] as [T996] starts 2021-11-08 and lasts 3 days

-- Altii --
[990 Livrare usi 4 BV] as [T990] starts 2021-11-22 and lasts 1 day
[991 Montage fenetres living/cuisine] as [T991] starts 2021-11-10 and lasts 1 day
[995 Livrare cada] as [T995] starts 2021-11-17 and lasts 1 day
[997 Livrare carrelage] as [T997] starts 2021-11-15 and lasts 1 day

'Adding constraint
[T108] -> [T991]
[T991] -> [T992]
[T117] starts 1 day after [T992]'s end
[T14] starts 1 day after [T112]'s end
[T105] -> [T15]
[T994] starts 1 day before [T119]'s end
[T121] starts 1 day before [T995]'s end
[T112] starts 1 day before [T990]'s end
[T105.2] starts 1 day before [T997]'s end
[T121] -> [T83]
[T991] -> [T999]
[T991] -> [T994]

@endgantt

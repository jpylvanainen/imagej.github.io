{{Infobox
| software               = Fiji
| name                   = Find Maxima Detector for TrackMate
| author                 = {{Person|Twagner}}, {{Person|JeanYvesTinevez}}
| maintainer             = {{Person|Twagner}},
| filename               = TrackMate_FindMaxima.jar [https://github.com/thorstenwagner/ij-trackmate-findmaxima/releases/latest [1]]
| source                 = Github [https://github.com/thorstenwagner/ij-trackmate-findmaxima [2]]
| latest version         = v1.0.0 (13 May 2016)
| status                 = active 
}}
== Purpose ==
This plugin implements the find maxima detection algorithm for [[TrackMate]]. It was tried to resample the approach as for the ''Process -> Find Maxima...'' command. 
The results are almost the same. Subpixel accuracy is activated by default.

==Installation==
Copy the jar file into your fiji plugins folder. If you start TrackMate it is detected automatically and you can choose it as detector.

==Parameters==
[[File:Findmaxima gui.png|400px|thumb]]

'''Estimated blob diameter:''' To achieve subpixel accuracy this region is used for refining the positions.

'''Tolerance:''' As for the ''Process -> Find Maxima...'' command: "Maxima are ignored if they do not stand out from the surroundings by more than this value. In other words, a threshold is set at the maximum value minus noise tolerance and the contiguous area around the maximum above the threshold is analyzed. For accepting a maximum, this area must not contain any point with a value higher than the maximum. Only one maximum within this area is accepted."

==Example==
The example shows a typical image of scattering nanoparticles. The detection was done with a '''estimated blob diameter''' of 10 and '''tolerance''' of 10: 
[[File:Findmax result.png]]
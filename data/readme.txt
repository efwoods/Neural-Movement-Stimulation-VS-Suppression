Social Competition Task

*Task design
There were two monkeys sitting around a table. ECoG data and eye tracking
data were recorded from one monkey. Motion data were captured from both monkeys
and experimenter. For each trial, one food reward was placed on the table.
If one monkey was dominant to the other, he could take the reward withouthesitation.
But, if he was submissive, he could not take the reward because of social suppression.
ECoG data were obtained from one monkey under different hierarchycal conditions by
pairing with multiple monkeys.
ECoG data were sampled at 1KHz. Motion data and eye tracking data were sampled at 120Hz.
Start and stop point of all data were synchronized.

*Event Discription
'Low' Opponent monkey was submissive and monkey with ECoG was dominant in competitive condition.
'LowNC' Opponent monkey was submissive and monkey with ECoG was dominant in no-competitive condition.
'High' Opponent monkey was dominant and monkey with ECoG was submissive in competitive condition.
'HighNC' Opponent monkey was dominant and monkey with ECoG was submissive in no-competitive condition.
'Rest' There was no opponent monkey. Monkey with ECoG relaxed.

*Data Format
A. ECoG_chN.mat
ECoGData_chN: ECoG signal (μV) recorded from electrodeN (1‐128), sampled at 1kHZ.
The Location of electrode is documented in "K2.png".


B. ECoG_time.mat
ECoGTime: ECoGTime is a one row-vector contains Time-stamps with the same length as ECoGData_chN.

C. Event.mat
EventData: EventData is a one row-vector contains event id.
*event_name,id
- start_Low, 1
- end_Low, 2
- start_LowNC, 3
- end_LowNC, 4
- start_High, 5
- end_High, 6
- start_HighNC, 7
- end_HighNC, 8
- start_rest, 9
- end_restt, 10
EventTime: EventTime is a one row-vector contains corresponding time-stamp.

D. Eyetrack.mat
EyeTrackData: EyeTrackData is a time × variable matrix containing various variable
 describing eye motion.
― Column 1: Index (120Hz sampling rate)
― Column 2: ‐‐‐‐‐‐‐‐
― Column 3: Angle of x‐axis (deg)
― Column 4: Angle of y‐axis (deg)
― Column 5: Speed of eye movement
― Column 6: Gaze time
― Column 7: Pupil size (X)
― Column 8: Pupil size (Y)
― Column 9: Eye blink
EyeTrackTime: EyeTrackTime is a one row-vector contains the corresponding time-stamps.

E. Motion.mat
MotionData: MotionData is a time × marker matrix containing 3-D position of marker
-index 1, Kuma10mks_HeadSquare:LSHO
-index 2, Kuma10mks_HeadSquare:LELB
-index 3, Kuma10mks_HeadSquare:LWRI
-index 4, Kuma10mks_HeadSquare:RSHO
-index 5, Kuma10mks_HeadSquare:RELB
-index 6, Kuma10mks_HeadSquare:RWRI
-index 7, Kuma10mks_HeadSquare:FLHD
-index 8, Kuma10mks_HeadSquare:FRHD
-index 9, Kuma10mks_HeadSquare:BLHD
-index 10, Kuma10mks_HeadSquare:BRHD
-index 11, Human2Hands2Shoulders2Heads:LHD
-index 12, Human2Hands2Shoulders2Heads:LSHO
-index 13, Human2Hands2Shoulders2Heads:LHND
-index 14, Human2Hands2Shoulders2Heads:RHD
-index 15, Human2Hands2Shoulders2Heads:RSHO
-index 16, Human2Hands2Shoulders2Heads:RHND
-index 17, Kuma6mks:LSHO
-index 18, Kuma6mks:LELB
-index 19, Kuma6mks:LWRI
-index 20, Kuma6mks:RSHO
-index 21, Kuma6mks:RELB
-index 22, Kuma6mks:RWRI
MotionTime: MotionTime contains the corresponding time-stamps.

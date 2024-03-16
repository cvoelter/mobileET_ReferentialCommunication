# mobileET_ReferentialCommunication
Data analysis of "Using mobile eye tracking to study dogs’ understanding of human referential communication""

## Structure
|   02_mobileET_ostension_data_analysis.Rmd: Markdown file including the analyses.
|   README.md
|   
+---data: folder containing data files
|       aoi_transition_frequency_data.csv: data file regarding the frequencies of transitions between areas of interest
|       latency_first_look_into_aoi.csv: latencies of first look into different areas of interest
|       mobile_ET_combined_data_20230427.csv: combined eye-tracking and behavioral data
|       mobile_ET_ostension_counterbalancing_20230201.csv: counterbalancing and behavioral data
|       mobile_ET_yarbus_agg_data_20230427.csv: the aggregated Yarbus data containing information about the descriptive stats regarding the gaze coordinates for the different interest periods.
|       mobile_ET_yarbus_raw_data_20230427.csv: the raw Yarbus data containing information about the gaze coordinates of each fixation.
|
+---functions: helper functions
|       
+---graphics: data visualisations
|       
+---saves: output of the analyses
|       
\---workspaces: R images of the analyses


### Variables Description: aoi_transition_frequency_data.csv

1. **X**: Index variable.
2. **subject.x**: Identifier for the subject (dog).
3. **session**: Session number.
4. **trial**: Trial number.
5. **condition**: Condition of the trial (e.g., gazing).
6. **transition_category**: Category of gaze transition between areas of interest (e.g., Face-Hand).
7. **n**: Count of transitions within the specified category.
8. **transition_binary**: Binary indicator for the presence of a transition (1 for present, 0 for absent).


### Variables Description: latency_first_look_into_aoi.csv

1. **X**: Index variable.
2. **yarbus_file**: Name of the Yarbus file.
3. **subject**: Identifier for the subject (dog).
4. **interest_period**: Period of interest during the trial (e.g., signaling).
5. **session**: Session number.
6. **trial**: Trial number.
7. **aoi3**: Area of interest where the first look occurred.
8. **condition**: Condition of the trial (e.g., pointing).
9. **first_look**: Latency to the first look into the area of interest, measured in milliseconds.


### Variables Description: mobile_ET_combined_data_20230427.csv

1. **X**: Index variable.
2. **yarbus_file**: Name of the Yarbus file.
3. **trial**: Trial number.
4. **interest_period**: Period of interest during the trial.
5. **subject**: Identifier for the subject (dog).
6. **session**: Session number.
7. **aoi**: Area of interest.
8. **fixation_time**: Time spent in fixation (milliseconds).
9. **breed**: Breed of the dog.
10. **age**: Age of the dog in months.
11. **sex**: Sex of the dog.
12. **neutering_status**: Neutering status of the dog.
13. **birth_date**: Birth date of the dog.
14. **test_date**: Date of the test.
15. **condition**: Condition of the trial (e.g., gazing, pointing).
16. **baited_side**: Side where the food is baited (left or right).
17. **correct**: Indicator for correct choice (1 = correct, 0 = incorrect).
18. **chosen_side**: Side chosen by the dog.
19. **dark_green_bowl_side**: Side of the dark green bowl.
20. **ET_data**: Eye tracking data indicator.
21. **comment**: Additional comments.
22. **chosen_bowl**: Bowl chosen by the dog.
23. **correct_bowl**: Correct bowl.
24. **ip_duration**: Interest period duration (milliseconds).
25. **prop_fixation_time**: Proportion of fixation time.


### Variables Description: mobile_ET_ostension_counterbalancing_20230201.csv

1. **subject**: Identifier for the subject (dog).
2. **breed**: Breed of the dog.
3. **age**: Age of the dog in months.
4. **sex**: Sex of the dog.
5. **neutering_status**: Neutering status of the dog.
6. **birth_date**: Date of birth of the dog.
7. **test_date**: Date of the test session.
8. **trial_number**: Number of the trial.
9. **session**: Session number.
10. **condition**: Condition of the trial (e.g., gazing).
11. **baited_side**: Side where the food reward is baited (e.g., left or right).
12. **correct**: Whether the choice made by the dog was correct (0 for incorrect, 1 for correct).
13. **chosen_side**: Side chosen by the dog.
14. **dark_green_bowl_side**: Side where the dark green bowl is located.
15. **ET_data**: Eye-tracking data indicator.
16. **session_new**: Session number (only valid sessions considered).
17. **yarbus_file**: Name of the Yarbus file.


### Variables Description: mobile_ET_yarbus_agg_data_20230427.csv

1. **X**: Index variable.
2. **subject**: Identifier for the subject (dog).
3. **sex**: Sex of the dog.
4. **age**: Age of the dog in months.
5. **session**: Session number.
6. **trial**: Trial number.
7. **condition**: Condition of the trial (e.g., gazing).
8. **baited_side**: Side where the food is baited (left or right).
9. **interest_period**: Period of interest during the trial (e.g., addressing, baiting).
10. **max_x**: Maximum x-coordinate of gaze.
11. **min_x**: Minimum x-coordinate of gaze.
12. **median_x**: Median x-coordinate of gaze.
13. **mean_x**: Mean x-coordinate of gaze.
14. **baitedX**: max X-coordinate toward baited side.


### Variables Description: mobile_ET_yarbus_raw_data_20230427.csv

1. **X**: Index variable.
2. **yarbus_file**: Name of the Yarbus file.
3. **trial**: Trial number.
4. **movie_time**: Time in milliseconds within the movie.
5. **recordFrameCount**: Record frame count.
6. **sceneFrameCount**: Scene frame count.
7. **avg_fps**: Average frames per second.
8. **sceneQTtime.d.h.m.s.tv.ts.**: Scene camera QT time.
9. **porQTtime.d.h.m.s.tv.ts.**: POR (eye camera) QT time.
10. **porX**: X-coordinate of the point of regard.
11. **porY**: Y-coordinate of the point of regard.
12. **pupilX**: X-coordinate of the pupil.
13. **pupilY**: Y-coordinate of the pupil.
14. **cornealRefX**: X-coordinate of the corneal reflection.
15. **cornealRefY**: Y-coordinate of the corneal reflection.
16. **diameterW**: Pupil diameter width.
17. **diameterH**: Pupil diameter height.
18. **subject_yarbus**: Identifier for the subject (dog).
19. **scene_time_ms**: Scene time in milliseconds.
20. **interest_period**: Interest period.
21. **subject**: Identifier for the subject (dog).
22. **breed**: Breed of the dog.
23. **age**: Age of the dog in months.
24. **sex**: Sex of the dog.
25. **neutering_status**: Neutering status of the dog.
26. **birth_date**: Date of birth of the dog.
27. **test_date**: Date of the test session.
28. **condition**: Condition of the trial (e.g., gazing).
29. **baited_side**: Side where the food reward is baited (e.g., left or right).
30. **correct**: Whether the choice made by the dog was correct (0 for incorrect, 1 for correct).
31. **chosen_side**: Side chosen by the dog.
32. **dark_green_bowl_side**: Side where the dark green bowl is located.
33. **ET_data**: Eye-tracking data indicator.
34. **session**: Session number.
35. **comment**: Comments or additional notes.
36. **chosen_bowl**: Bowl chosen by the dog.
37. **correct_bowl**: Correct bowl according to the experiment.


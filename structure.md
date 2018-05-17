# Structure of the educational "container" repositories

The basic layout is as follows:
```
repo
├─── README.md
├─── presentation
│    ├─── README.md
│    └─── meetup.pptx
└─── workshop
     ├─── README.md
     └─── Lab1
	      └─── README.md
```

Details:
* At the root of each directory should be a README.md file describing
  the purpose of its contents. The top-most README.md file should
  provide a high-level overview of the entire repository without
  doing a deep-dive.
* The `presentation` directory contains all of the information needed
  for meetup style of event - typically scheduled for around one hour in
  length.  It should contain a presenation and any additional material
  needed, such as demo scripts. The presentation should include lots of
  detailed speaker notes so that other people can re-use it if they wish
  and know what the main talking points are for each slide.
* The `workshop` directory contains all of the material needed for either
  a self-directed workshop/lab, or a moderated one. In either case, the
  README.md file in each of the `Lab` directories should be written such
  that they can be followed by a student reading it on their own.
  In cases where there will be a presentor walking through the exercises
  with them, then they can either use the `meetup.pptx` from the
  `presentation` directory, or if that doesn't align perfectly, a
  workshop-specific presentation file can be included in the `workshop`
  directory.
* The `workshop` material should include as much "hands-on" exercises
  as possible, without overwhelming the students. Each step of the
  exercises should include some explanatory text describing what
  they are learning, why are they doing it, and what is happening
  behind the scenes - but, again, without overwhelming them. If the
  explanatory text is valuable, but distrupts the flow of the exercises,
  consider moving the text into secondary md files and adding a 
  "for more information see here" type of reference from the README.md.
  Then the student can choose whether they want to learn more at their
  own pace.
* Ideally, the `presentation` and the `workshop` material should be
  aligned such that the `presentation` is considered a shorter version of
  the longer `workshop` material. People leaving a meetup presenation
  should be encouraged to walk through the `workshop` on their own and
  feel comfortable with the concepts because most of them have been
  briefly touched on during the live presentation.


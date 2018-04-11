# Birds sound recognition review

Recognising birds by their songs is a globally known task. Sounds can travel long distances through vegetation and other obstacles, and they can be recorded without a human being present any time of the day. Thanks to that bird songs might be the best way to monitor avian counts and migrations. To automate this process, we need a system that can detect different birds by their voices.

[BirdCLEF contest](http://www.imageclef.org/lifeclef/2017/bird) offers scientists to test their findings in the bird recognition sounds field.
It uses [xeno-canto](https://www.xeno-canto.org/) dataset.

Another challenge is run by [DCASE](http://dcase.community/challenge2018/task-bird-audio-detection).
There are quite a few projects in the birds' identification area. Some of them are:

* https://www.hackster.io/teamscc/identifying-birds-using-machine-learning-9dd03f

* https://arxiv.org/ftp/arxiv/papers/1609/1609.08408.pdf

* https://peerj.com/articles/488/#supplemental-information

* https://arxiv.org/pdf/1505.06443v1.pdf

* https://experiments.withgoogle.com/ai/bird-sounds

All of this projects and challenges are aimed at creating a better algorithm that can be applied to a big data sets gathered by different means in different places but kept in a one database.

All these models are learned on the data gathered outside of New Zealand. As the New Zealand bird population differes a lot from the rest of the world, there is no value in using existing models.

To be able to create an app that can detect a bird located in New Zealand we need to use locally gathered data for the "cold start" step and/or add other parameteres beside the sound recording (such as geo coordinates, altitude and time of the day).
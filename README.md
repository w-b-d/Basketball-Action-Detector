# Basketball Action Detector (in progress)

Turns broadcast basketball video into player tracking data and detects game actions.

**Pipeline:** detect players → track with BoT-SORT → assign teams by jersey color → read jersey numbers →
project positions onto a top-down court → detect shots and on-ball screens.

**Status:** working on a 45-second NBA clip; currently improving tracking through screens and camera pans.

**Built with:** Roboflow's pretrained player, court keypoint and jersey-number models, the `sports`,
`supervision` and `trackers` libraries, scikit-learn and OpenCV.

**My additions:** jersey-color team classifier, track stitching,
trajectory cleaning, and the on-ball screen detector.

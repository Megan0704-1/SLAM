camera calibration [link https://youtu.be/qByYk6JggQU?si=JWw9ctEhyRZx1N7g]
1. In camera calibration, we need to estimate two matricies, one from camera position to image plane, one from world coordinate to camera coordinate.
2. first we evaluate the one from camera to plane. Given a point P in camera coordinate ($x_c, y_c, z_c$) we aim to find projecion matrix that leads to image coordinate: ($x_i, y_i$). While image plane is measured using unit (mm) we need to tranformed it into what image sensor use (pixel unit), where pixel length may differ in x axis and y axis. Additionally, the center of image sensor are usually at the upper left corner, thus we developed intrinsic matrix $M_{intrin}$, which transform the
   camera coordinate of point P, ($x_c, y_c, z_c$), to image coordinate ($x_i, y_i$).
3. Next, we evaluate the tranformation from world coordinate($x_w, y_w, z_w$), to camera coordinate($x_c, y_c, z_c$), denote as $M_{extern}$.
4. Hence, we conclude: for point P in world coordinate ($x_w, y_w, z_w$), to image plane -> $(x_i, y_i, 1) = M_{intern}*(M_{extern}*(x_w, y_w, z_w))$

## Euler Angles
Explained by UPenn engineering Professor, link: [https://youtu.be/3Zjf95Jw2UE?si=_8DwyzLceRrJRq-l]

If we know the order of the rotations (e.g ZXY), and the $R_{33}$ is neither 1 nor -1: then we have 2 sets of possible Euler angles
Yet if ${R_{33}}$ is +-1: then there might have infinite set of possible Euler anlges.

## Groups
Explained by 3b1b, link [https://www.youtube.com/watch?v=mvmuCPvRoWQ]

Groups of symmetries are composite, combining symmetries can generate another symmetries in a group.

## Gimbal Lock
Explained by yt, link[https://www.youtube.com/watch?v=zc8b2Jo7mno]

The key is to find the rotation order of an object with the least chance hitting Gimbal Lock
> Practice finidng Euler angle representation [https://www.youtube.com/watch?app=desktop&v=8FD1jgb3Df4]

## Quarternions
Explained by 3b1b, link[https://www.youtube.com/watch?v=d4EgbgTm0Bg]

real number + 3 imaginary parts = 4 hypershere
we should comprehend the hypershpere in 3 dimensional space as a projection
E.g. 
    i*j = k
    thumb points from origin to i (unit sphere)
    imagine a circle draw from j
    scale line with the thumb position meanwhile rotate the point lies on j: reaches k! 

## Axis-Angle and Quarternion
1. Axis-Angle
    - A method represents rotation by a unit vector (rotation axis) and an angle
    - With a vector $v = (x, y, z)$ as rotation axis, $v$ is a unit vector,
    - an angle $\theta$ as the rotation regree along with $v$.
2. Quarternion
    - $q = w+xi+yj+zk$, where q is quarternion, w is real part
    - pros: avoid the Gimbal lock problem when using Euler angle representation

3. 1 to 2
    - Given a angle-axis $(v, \theta)$, and $v = (x, y, z)$ is a unit vector, we can transform it to quarternion representation by the follwoing formula:
        - $w = cos(\theta/2)$
        - $x = sin(\theta/2)*v_{x}$
        - $y = sin(\theta/2)*v_{y}$
        - $z = sin(\theta/2)*v_{z}$
4. 2 to 1
    - GIven a quaternion $q=w+xi+yj+zk$
    - calculate angle $\theta = 2arccos(w)$
    - $v=v(v_x, v_y, v_z)$
    - $v_x = \frac{x}{\sqrt(1-w^2)}$
    - $v_y = \frac{y}{\sqrt(1-w^2)}$
    - $v_z = \frac{z}{\sqrt(1-w^2)}$

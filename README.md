# Gravity Duck

Game made by C++ OpenGL

Content:
======

Image:
------

![Image](https://lh3.googleusercontent.com/GHZhGiho1tM76SRA1NMiv6PaYWi7sNeT20V-wbPrQPa5NK20x-zn6Sa0BZVKjE35nK7lsPWQHPf9o8jNiVOI3q3XUmYbK5bOzz80RNS52Z-NWFUrALIJpozuPNtbfgxRYnosJ0N7MmTdwbelQ-91kMNegP3SrXVBfW4X-VXfFkcWWPYVXvhbm9jcAeu88JtdPO6ojhvABpQp7PJXUqUTcWnGRt-JWoACWqpcGqVMxrPPmGraoEAaGYK0GActeVn29KvCF8lVHanSvggFK9sZlVz1IyeYQ17HZkJJLmCwmZbefcEaoaIB98773jbTF3-zEfWNUUcaAbE-KWJERM8ZIZpbHwFCwQmLnL7mQTyHNiZxyRWPL9XU4pmwfi-x0XWiOMgdZtzfmIfvqrKr3wvRZgQPHe5IkZ-8EjwN6M_eujILu9Dg3KwUvbzpmmAClXw1CVQ1RmfWjGm3XzEqirpHIR47w_ijqM6HyEViT4JF-FcwKwnR6HPWVfG-z1bNQa4hHxKYfu4uzYLEdJ5O0sL2opbF87NAR6W7vqFK-bo8giNjFKNh3QpIY0yC26Fo9WkEhJ_89IgJ2aZgbC_w4s4uLdppv1fP_RGGoVpCjtUZlje0IZe_C34bHqor_bPNwbMGJT-C7qfUjo44gtYKjBoMUofoehyEB7Ytg27sddQwt3Xbyn0a-bLJSmPeN1TJmbpxLPXwQHbezQ6DTl3LK6XYGmqXuf5tFH4vZjBfP01mYdkXi7k=w640-h480-no)

In Map_18<br />
Enemy_1: Move 0 Move_Max 81<br />
Enemy_2: Move 29 Move_Max 81<br />
Reason:<br />
Move_Max = Move_Max + 9 = 90 (Stt = 3, Stt Change Every 3 Time (Enemy_Time = 3) => +9 Offset For Move_Max)<br />
=> Move = Move_Max / 2 = 45 (Balance Bullet For 2 Enemies)<br />
But Enemy_1_X (17) > Enemy_2_X (15) = 2 * 32 = 64 (32 Is Size Of Tile)<br />
Offset_Bullet = 4 => Enemy_1_Latency = 64 / 4 = 16<br />
=> Enemy_1_Move = 45 - 16 = 29<br />

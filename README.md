
# DARP: Divide Areas Algorithm for Optimal Multi-Robot Coverage Path Planning

# Motivation

In order to cover a region of interest with previously identified obstacles, this project works with the path planning problem for a group of mobile robots. The DARP algorithm divides the territory into a number of equal regions, each corresponding to a particular robot, in order to ensure total coverage, a non-backtracking solution, and a minimal coverage path while requiring no prior planning. 

# Requirements
run this command
```
pip install -r requirements.txt
```
after going inside the directory.

# To setup the environment install requirements.text file beforehand.
numpy==1.20
opencv-python==4.5.4.60
pygame==2.1.0
scipy==1.7.3
jupyter==1.0.0
numba==0.54.1
nose==1.3.7
parameterized==0.8.1
sklearn
Pillow
Python 3.6
PyQt


# To run the code, use:

run this command for the simulation DARP-STM for 2 robots
```
python PathPlanner.py -vis -nep -obs_pos 507 479 451 423 395 367 339 311 283 255 227 199 172 173 202 230 258 286 314 342 370 398 426 454 482 510 486 515 516 489 461 433 405 377 349 348 347 346 318 290 262 234 206 179 180 209 185 213 241 269 297 325 353 381 409 437 465 493 522 523 524 497 469 441 413 385 357 329 301 273 245 217 189  -in_pos 177 487 -portions 0.51 0.49
```
for 3 robots
```
python PathPlanner.py -vis -nep -obs_pos 507 479 451 423 395 367 339 311 283 255 227 199 172 173 202 230 258 286 314 342 370 398 426 454 482 510 486 515 516 489 461 433 405 377 349 348 347 346 318 290 262 234 206 179 180 209 185 213 241 269 297 325 353 381 409 437 465 493 522 523 524 497 469 441 413 385 357 329 301 273 245 217 189  -in_pos 177 239 487 -portions 0.33 0.34 0.33
```

for 4 robots 
```
python PathPlanner.py -vis -nep -obs_pos 507 479 451 423 395 367 339 311 283 255 227 199 172 173 202 230 258 286 314 342 370 398 426 454 482 510 486 515 516 489 461 433 405 377 349 348 347 346 318 290 262 234 206 179 180 209 185 213 241 269 297 325 353 381 409 437 465 493 522 523 524 497 469 441 413 385 357 329 301 273 245 217 189  -in_pos 177 239 487 163 -portions 0.25 0.25 0.24 0.26

```
for 5 robots
``` 
python PathPlanner.py -vis -nep -obs_pos 507 479 451 423 395 367 339 311 283 255 227 199 172 173 202 230 258 286 314 342 370 398 426 454 482 510 486 515 516 489 461 433 405 377 349 348 347 346 318 290 262 234 206 179 180 209 185 213 241 269 297 325 353 381 409 437 465 493 522 523 524 497 469 441 413 385 357 329 301 273 245 217 189  -in_pos 177 239 487 163 -portions 0.20 0.20 0.20 0.185 0.215

```
To retriev the graphs run. 
Before running this please ensure to place my_numpy.npz and np_plot.py in the same folder 
python np_plot.py

To tune the hyper parameters. this file will also run a simulation but doesn't report execution time and robot cell divison. 
python GD_voronoi.py

Here is the video implemenmtation of tge algorithm 


https://user-images.githubusercontent.com/87424679/215304472-3284e983-49c6-4548-a3d0-62f03ba6a675.mp4


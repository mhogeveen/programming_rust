# Mandelbrot

## `mandel_1.png`

Optimized release build, but no use of concurrence.

![mandel 1](./mandel_1.png)

### Command used

```sh
time mandelbrot mandel_1.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 96%      | cpu         |
| 3.54s    | user        |
| 0.02s    | system      |
| 3.697    | total       |

## `mandel_2.png`

Optimized release build, 8 threads.

![mandel 2](./mandel_2.png)

### Command used

```sh
time mandelbrot mandel_2.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 296%     | cpu         |
| 3.81s    | user        |
| 0.02s    | system      |
| 1.292    | total       |

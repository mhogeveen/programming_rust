# Mandelbrot

## Optimized release build, but no use of concurrency.

![mandel](./mandel.png)

### Command used

```sh
time mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 96%      | cpu         |
| 3.54s    | user        |
| 0.02s    | system      |
| 3.697    | total       |

## Optimized release build, 8 threads.

Image: see above

### Command used

```sh
time mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 296%     | cpu         |
| 3.81s    | user        |
| 0.02s    | system      |
| 1.292    | total       |

## Optimized release build, all available threads (using `num_cpus` crate).

Image: see above

### Command used

```sh
time mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 297%     | cpu         |
| 3.80s    | user        |
| 0.01s    | system      |
| 1.286    | total       |
